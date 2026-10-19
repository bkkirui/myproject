# Financial model: oilseed crushing + extruded aquafeed mill (Kisumu, Kenya)

One Python script (`model.py`) holds every assumption and every calculation. Running it writes the workbook, a markdown summary and CSVs for Stata. The Excel file is an output, not the model: it contains values, not live formulas. To change a result, change an input and re-run.

```bash
cd "business_plans/Oilseed crushing and feed mill/model"
python3 model.py            # about 3 minutes (VOI Monte Carlo and gate calibration); needs numpy and openpyxl only
```

## Files produced

| File | Content |
|---|---|
| `financial_model.xlsx` | 13 sheets (listed below) |
| `outputs.md` | Paste-ready tables for the plan writer: configuration, capex, funding, annual summary, unit economics, returns, Phase 2 gate, scenarios, tornado, seed x oil grid, survival view, checks, caveats |
| `pnl_annual.csv` | Annual P&L, one row per year 2027-2038, KES m nominal; volumes in tonnes; USD memo columns |
| `cashflow_annual.csv` | Annual cash flow, funding, debt balances, DSCR, project and equity flows (KES m and USD m) |
| `mass_balance_annual.csv` | Every tonnage line (seed, oil, cake, meal, hulls, losses, feed ingredients, energy) |
| `scenarios_annual.csv` | EBITDA, equity and project flows for each scenario |
| `voi_draws.csv` | One row per Phase 0 value-of-information draw (inputs drawn, survival-weighted founder NPVs at 35%/40% and p_fail 30%/20%, with full and Phase-0a-only information) for both prior correlations |

CSV variable names are lower-case, Stata-safe and no longer than 32 characters. In Stata:

```stata
import delimited "pnl_annual.csv", clear
tsset year
list year revenue ebitda net_income if year>=2029
```

## Workbook sheets

| Sheet | What it shows |
|---|---|
| Assumptions | Every scalar input with low, base and high values, unit and source (research file section, plus the original URL where one exists). Tags: `[ESTIMATE]` = analyst judgement with reasoning; `[DATED]` = pre-2025 source; `[UNVERIFIED]` / `[CONFLICT]` = weak or disputed source. Below the scalars: path and table inputs (seed-supply path, seed-cost path, sourcing mix, ramps, purchase seasonality, feed formulas with calculated crude protein) |
| Mass balance | Seed -> oil + cake/meal + hulls + losses; oil routing (to feed, to refinery, crude sold); cake routing; feed mash -> feed; merchant aquafeed SAM and the share won; energy and storage. Includes closure check rows |
| Capex & phasing | Phase 1 and Phase 2 items in USD m (low/base/high), with IDF/RDL and contingency shown separately; nominal KES phasing; VAT timing on capex; book depreciation; tax allowances |
| Operating P&L | Ten operating years (2029-2038) plus 2027-28 pre-operating, in nominal KES m. Revenue by product, variable/fixed/selling costs, levies, EBITDA, interest, tax and net income; USD memo at the explicit FX path; unit economics |
| Working capital | Monthly seed-stock profile (% of annual crush), December/average/peak ratios, year-end WC components, intra-year peak, revolver |
| Cash flow & funding | Operating/investing/financing flows, equity injections (incl. covenant cure equity), senior prepayments (cure and sweep), distributions, debt schedules (senior KES, USD mezzanine, Phase 2 DFI loan, revolver, DSRA), CFADS and DSCR, Phase 1 sources and uses |
| Returns | Project and equity IRR in KES and USD (with and without terminal value; equity also after dividend WHT and CGT); WACC computed from the modelled Phase 1 structure and NPV at it (the financing file's 23% kept as a memo); NPVs at infrastructure-bond, established and greenfield hurdles; payback; peak funding; minimum DSCR, cure equity, breach and lock-up years. Columns: plan with auto gate, full plan, Phase 1 only. Also the Phase 2 gate tests |
| Scenarios | Bear / base / bull, all-adverse stress, competitor response, Uganda/Tanzania upside, Phase 2 at the 150 t/d spec, a v1.1-market bridge case, and two restructure alternatives (feed-mill-first, crusher-only), with definitions, key inputs and annual EBITDA/equity flows |
| Sensitivities | Tornado of 32 one-at-a-time drivers on equity IRR (KES and USD), project IRR, minimum DSCR, cure equity and peak equity, plus a two-way grid of seed cost x oil price index |
| Survival-weighted | Four-branch tree (early failure / late failure / survive without Phase 2 / survive with Phase 2). Expected equity IRR and NPV against the 35-40% hurdle; founder flows with the personal-guarantee call and GM dilution; bond comparison on survival-weighted after-shareholder-tax flows; failure-probability sweep |
| Phase 0 VOI | Value of information for Phase 0: stop now, invest now, Phase 0a only, staged 0a then 0b, perfect information; probability of passing G0; under independent and correlated priors |
| Gates & break-evens | Calibrated kill thresholds (covenant, hurdle and kill-with-others-at-bull), and joint favourable cases |
| Checks | Mass-balance closure, capacity limits, market-share cap, and benchmark checks against the research files (crush margin per t, feed raw-material cost, energy, EBITDA, seasonal WC peak, DSCR) |

## How the model works

**Timeline.** 2027 is Phase 0 (outgrower pilot, FEED, ESIA, offtake LOIs) with FID in Q4. 2028 is construction. COD falls in 2029 (`ops_months_y1` = 9, i.e. about April). The Phase 2 gate is tested on 2031 results; Phase 2 is built in 2032 and operates from 2033. The model values flows at 2027 using end-year discounting, and takes terminal value at end-2038 as an exit multiple of 2038 EBITDA.

**Prices and inflation.**
- Prices are entered in 2026 KES, ex-VAT.
- Tradables (oil, cake, seed, feed, ingredients, imported capex) are escalated by USD drift (2%) times the FX path. The FX path starts at KES 129.8, depreciates 4%/yr, and takes an extra 1.5 pp in the election year 2027.
- KES CPI follows PPP, (1 + USD drift)(1 + depreciation) - 1, plus an explicit real-drift input. Local costs follow CPI; wages follow CPI + 1%.

**Policy risk in the base case.** Each shock enters at its probability from regulatory_tax_risk.md s7:
- CPO duty removal: 60% x KES 15k/t off oil prices.
- GM feed imports allowed: 40% x 25% off protein-meal prices.
- Feed-ingredient duty waivers: one year in three x 7.5%.
- Tanzanian seed export levy: 70% x 10%.

Bear and stress set these to certain. Bull removes them.

**Market (round 1).** `sam_2026` is the contestable KENYAN merchant aquafeed market (25 kt in 2026, net of Victory Farms' captive feed and SamakGro's VF-linked sales; build-up in research/round1_evidence.md s1). Uganda/Tanzania demand (`sam_regional`) is 0 in the base and an upside scenario. `feed_real_decline` (1%/yr base) lowers feed prices in real terms from 2029 for competitor response; `feed_px_mult` scales both feed list prices.

**Price linkages.**
- Crude oil (`p_crude`, KES 175k/t = reconciled CPO landed parity) is the oil price index. Refined oil = crude + `refine_spread` (KES 65k/t, so 240k/t), so the two cannot drift apart.
- Delivered seed absorbs `seed_passthrough` (50%) of any change in oil + cake value per tonne of seed, measured against today's research prices. This is the floating, parity-linked contract recommended in feedstock_supply.md s4.2.
- Aquafeed prices absorb `feed_cost_passthrough` (70%) of the change in a competitor's formula cost.

**Mass balance.**
- Crush = min(capacity x 90%, seed-supply path) x operating fraction. Seed is 70% sunflower and 30% non-GM soy.
- Sunflower: full press until Phase 2, then prepress + solvent with dehulling. Hulls fire the boiler.
- Soy: extruder-expeller.
- Feed sold = min(extrusion capacity, ramped share x merchant aquafeed SAM). The grow-out and starter formulas use own cake and oil first; any shortfall is bought (SBM, cake). Surplus cake and meal are sold.
- Crude oil goes first to feed, then to the refinery up to a ramped own-brand share; the remainder is sold crude to refiners.
- Every balance is checked on the Checks sheet.

**Working capital.**
- A monthly purchase profile (70% of seed bought June-October) with even crushing and a safety stock gives December, average and peak stock ratios.
- Year-end seed stock is the December ratio x next year's crush. Other WC is days-based.
- Outgrower seed credit is outstanding March-August.
- A seasonal revolver advances 65% of seed stock. Its interest runs on the average draw.

**Funding.**
- Phase 1 senior KES loan (15.5%, 7 years, 18-month grace, quarterly instalments). `size_senior()` sizes it to a 1.30x minimum DSCR over `dscr_first_year`-2034 on the **lender downside case** (CFADS x (1 - `sizing_haircut`) = x0.80), Phase 1 standalone, capped at USD 4.5m. On the round 1 base this gives **zero** senior debt.
- **Covenant consequences.** Below the 1.10x default covenant (`default_dscr`) the sponsor injects cure equity equal to the CFADS shortfall to 1.10x, which prepays senior, and pays a waiver fee (`waiver_fee`, 1% of opening senior). Below the 1.30x lock-up, distributions stop and `sweep_share` (50%) of excess cash prepays senior. Later instalments shrink pro rata. `run_fixed()` iterates the debt schedule and the waterfall until prepayments converge.
- USD mezzanine (13% + 15% WHT gross-up, 2 PIK years, 3-year grace, 5-year amortisation, FX loss on repayment).
- Grants.
- Phase 2 KES DFI loan for 55% of Phase 2 capex (14%, 9 years, 2-year grace).
- DSRA of 6 months of senior debt service.
- Equity covers any shortfall above minimum cash. Excess cash is distributed only when DSCR is at or above 1.30x (lock-up). When Phase 2 goes ahead, cash in the gate year (2031) is retained to part-fund the Phase 2 build rather than distributed and re-injected. Exit EV is floored at zero.
- Debt sizing is set once on the base case and held fixed in scenarios and sensitivities; the VOI and joint-case analyses re-size debt for each state.
- **WACC** is computed from the modelled 2027-29 sources (equity at 35%, senior and mezzanine post-tax, mezzanine grossed up for WHT and KES drift) and reported as `wacc_model`.
- `gm_equity` (4%) dilutes the founder group's share of distributions and exit; `pg_cover` (100%) is the founder's personal guarantee of any senior shortfall on liquidation.

**Tax.**
- 30% CIT.
- 100% investment deduction in the year an asset enters service (`inv_ded` = 0.5 switches to the 50% + 25% reducing-balance regime). Vehicles: 25% wear-and-tear.
- Five-year loss expiry.
- Foreign (mezz) interest capped at 30% of EBITDA, with a 3-year carry-forward.
- Irrecoverable VAT on exempt feed's operating inputs (2% of feed revenue) and an expected-value feed levy (0.5%).
- IDF + RDL on imported equipment (in capex). VAT on capex is paid and recovered the following year, except the exempt (feed) share of turnover when finished feed is VAT-exempt (`p_feed_exempt`), which is an up-front cash cost.
- Minimum tax: `p_min_tax` (25%) x max(0, 1% of turnover - CIT) from 2028.
- Unlevered tax for project returns is computed separately, with no interest deductions.

**Phase 2 gate** (`run_model(mode="auto")`). Phase 2 goes ahead only if all of these hold:
- (a) seed secured for 2035 >= 80% of Phase 2 nameplate;
- (b) 2031 feed sales >= 8 kt at >= 20% gross margin;
- (c) >= 70% of crude for sale is refined under the own brand;
- (d) Phase 2's incremental **equity** NPV at the 35% greenfield hurdle > 0 (existing shareholders fund it). The incremental project NPV at the Phase 2 funding-mix WACC (55% DFI debt post-tax, rest equity at 35% = 21.1%) is reported alongside.

Use `mode="go"` or `mode="no"` to force the decision.

**Survival view.**
- Early failure (p = 30%): bear-case operations to 2030, then liquidation in 2031 at 35% of gross capex plus 70% of WC, less net debt.
- Late failure (10% of survivors): base Phase 1 operations to 2034, then liquidation in 2035.
- Otherwise: Phase 1 only or the full plan, with P(go) = 50% only when the base gate says GO (0 otherwise).
- The expected equity cash flow gives the expected IRR, which is compared with the 35-40% hurdle. Founder flows add the guarantee call and GM dilution; the bond comparison uses survival-weighted founder flows after dividend WHT and CGT.

**Phase 0 value of information** (`voi_analysis()`). 150 draws from triangular(low, base, high) priors on the market, price and capex inputs (revealed by Phase 0a) and seed cost and supply (revealed by Phase 0b), with a Gaussian copula (rho 0 or 0.5). Each draw is valued as the survival-weighted founder NPV at 35%/40%. Policies compared: stop, invest without information, Phase 0a only, staged 0a then 0b, and perfect information.

**Gate calibration** (`calibrate_gates()`, `g1_calibration()`, `joint_cases()`). Single-driver values at which the minimum DSCR hits 1.10x, the conditional equity IRR hits 35%, and (the kill rule) the survival-weighted founder IRR hits 35% at p_fail 20% with every other driver at its bull value.

**Restructure alternatives.** `config` = 1 (feed-mill-first, buys all protein) or 2 (crusher + refinery only) applies the capex and fixed-cost scaling in `CONFIG_CAPEX` and `CONFIG_FIXED` [ESTIMATE].

## How to change assumptions

1. **Scalar inputs.** Edit the `base` value (4th number) of the relevant tuple in `_A` near the top of `model.py`. Keep `low` and `high` meaningful, because scenarios and the tornado use them.
2. **Quick overrides without editing code.** Create `assumptions_override.csv` in this folder, then re-run; the console confirms each override.
   ```
   key,value
   p_feed_grow,115000
   seed_passthrough,0
   p2_tpd,150
   ```
3. **Paths and tables.** These live in `VECTORS` (supply path, sunflower seed-cost path, sourcing mix, ramps, purchase seasonality), `FORM_GROW` / `FORM_START` (feed formulas), and `CAPEX_P1` / `CAPEX_P2_REF` (capex items in USD m at 2026 prices). Phase 2 items are scaled from the 150 t/d reference with exponent `scale_exp`.
4. **Scenarios.** Edit `scenario_params()` and `SCEN_DESC`. Edit the tornado drivers and their low/high settings in `TORNADO`.
5. **Hurdles and survival.** These are `hurdle_*`, `infra_bond`, `p_fail`, `p_late_fail`, `late_fail_year`, `p_go`, `recovery_*` and `fail_year`. `wacc_p1` and `wacc_ss` are memo items only.

Re-run `python3 model.py` after any change. Every output, including `outputs.md` and the CSVs, is regenerated.

## Main judgement calls (see outputs.md section 11 for all caveats)

- **Phase 2 is resized** to 100 t/d crush, +3 t/h extrusion and +20 t/d refinery, against the technical file's 150 t/d, +6 t/h and 60 t/d. Seed supply (feedstock_supply.md s9) and the merchant aquafeed market (market_demand.md s5) do not fill the larger plant; scenario `p2_research_spec` shows its returns.
- **The Phase 1 refinery is 15 t/d, not 20 t/d,** because 30% of the seed is soy, which yields only 12% oil.
- **The feed price list is treated as retail.** A 5% dealer margin and 0.5% bad debts are deducted.
- **Senior debt is sized to DSCR on a lender downside case,** not taken at the financing file's USD 4.5m. On the round 1 base the plant cannot carry any senior debt on that test, because the 2030 ramp year's CFADS barely covers mezzanine interest; equity fills the gap. If lenders fund 2030 interest from the budget and test from 2031 (24-month grace), capacity is about KES 177m, and equity IRR does not improve, because project IRR is about equal to the cost of debt.
- **Round 1 rebase (see the plan's revision log).** SAM 45 kt to 25 kt Kenya-only; crude 190k to 175k; refined 264k (independent) to crude + 65k = 240k; 1%/yr real feed price decline; minimum tax at 25% probability; capex VAT apportioned. Scenario `v1_market` restores the v1.1 market inputs for a bridge.
- **The seed safety stock is calibrated** (1.5 months) so that peak stock (~41% of annual crush) falls inside feedstock_supply.md's 7-12 kt per 20 kt range.
