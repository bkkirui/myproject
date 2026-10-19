# Financial model: oilseed crushing + extruded aquafeed mill (Kisumu, Kenya)

One Python script (`model.py`) holds every assumption and every calculation. Running it writes the workbook, a markdown summary and CSVs for Stata. The Excel file is an output, not the model: it contains values, not live formulas. To change a result, change an input and re-run.

```bash
cd "business_plans/Oilseed crushing and feed mill/model"
python3 model.py            # about 10 seconds; needs numpy and openpyxl only
```

## Files produced

| File | Content |
|---|---|
| `financial_model.xlsx` | 11 sheets (listed below) |
| `outputs.md` | Paste-ready tables for the plan writer: configuration, capex, funding, annual summary, unit economics, returns, Phase 2 gate, scenarios, tornado, seed x oil grid, survival view, checks, caveats |
| `pnl_annual.csv` | Annual P&L, one row per year 2027-2038, KES m nominal; volumes in tonnes; USD memo columns |
| `cashflow_annual.csv` | Annual cash flow, funding, debt balances, DSCR, project and equity flows (KES m and USD m) |
| `mass_balance_annual.csv` | Every tonnage line (seed, oil, cake, meal, hulls, losses, feed ingredients, energy) |
| `scenarios_annual.csv` | EBITDA, equity and project flows for each scenario |

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
| Cash flow & funding | Operating/investing/financing flows, equity injections and distributions, debt schedules (senior KES, USD mezzanine, Phase 2 DFI loan, revolver, DSRA), CFADS and DSCR, Phase 1 sources and uses |
| Returns | Project and equity IRR in KES and USD (with and without terminal value; equity also after dividend WHT and CGT); NPVs at WACC, infrastructure-bond, established and greenfield hurdles; payback; peak funding. Columns: plan with auto gate, full plan, Phase 1 only. Also the Phase 2 gate tests |
| Scenarios | Bear / base / bull, an all-adverse stress case, and Phase 2 at the technical file's original 150 t/d spec, with definitions, key inputs and annual EBITDA/equity flows |
| Sensitivities | Tornado of 26 one-at-a-time drivers on equity IRR (KES and USD), project IRR and NPV, plus a two-way grid of seed cost x oil price |
| Survival-weighted | Three-branch tree (failure / survive without Phase 2 / survive with Phase 2). Gives expected-cash-flow equity IRR and NPV against the 35-40% greenfield hurdle, the survivor IRR the screening report's formula requires, and the break-even failure probability |
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

**Price linkages.**
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
- Phase 1 senior KES loan (15.5%, 7 years, 18-month grace, quarterly instalments). It is sized by `size_senior()` to a 1.30x minimum DSCR over 2030-34 on the Phase 1 standalone case, capped at USD 4.5m.
- USD mezzanine (13% + 15% WHT gross-up, 2 PIK years, 3-year grace, 5-year amortisation, FX loss on repayment).
- Grants.
- Phase 2 KES DFI loan for 55% of Phase 2 capex (14%, 9 years, 2-year grace).
- DSRA of 6 months of senior debt service.
- Equity covers any shortfall above minimum cash. Excess cash is distributed only when DSCR is at or above 1.30x (lock-up). When Phase 2 goes ahead, cash in the gate year (2031) is retained to part-fund the Phase 2 build rather than distributed and re-injected. Exit EV is floored at zero.
- Debt sizing is set once on the base case and held fixed in scenarios and sensitivities.

**Tax.**
- 30% CIT.
- 100% investment deduction in the year an asset enters service (`inv_ded` = 0.5 switches to the 50% + 25% reducing-balance regime). Vehicles: 25% wear-and-tear.
- Five-year loss expiry.
- Foreign (mezz) interest capped at 30% of EBITDA, with a 3-year carry-forward.
- Irrecoverable VAT on exempt feed (2% of feed revenue) and an expected-value feed levy (0.5%).
- IDF + RDL on imported equipment (in capex). VAT on capex is paid and recovered the following year.
- Unlevered tax for project returns is computed separately, with no interest deductions.

**Phase 2 gate** (`run_model(mode="auto")`). Phase 2 goes ahead only if all of these hold:
- (a) seed secured for 2035 >= 80% of Phase 2 nameplate;
- (b) 2031 feed sales >= 8 kt at >= 20% gross margin;
- (c) >= 70% of crude for sale is refined under the own brand;
- (d) Phase 2's incremental project NPV at the 16.5% steady-state WACC > 0.

Use `mode="go"` or `mode="no"` to force the decision.

**Survival view.**
- Failure (p = 30%): bear-case operations to 2030, then liquidation in 2031 at 35% of gross capex plus 70% of WC, less net debt.
- Otherwise: Phase 1 only or the full plan, with P(go) = 50%.
- The expected equity cash flow gives the expected IRR, which is compared with the 35-40% hurdle. The hurdle holds in expectation, not conditional on survival.

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
5. **Hurdles and survival.** These are `wacc_p1`, `wacc_ss`, `hurdle_*`, `infra_bond`, `p_fail`, `p_go`, `recovery_*` and `fail_year`.

Re-run `python3 model.py` after any change. Every output, including `outputs.md` and the CSVs, is regenerated.

## Main judgement calls (see outputs.md section 11 for all caveats)

- **Phase 2 is resized** to 100 t/d crush, +3 t/h extrusion and +20 t/d refinery, against the technical file's 150 t/d, +6 t/h and 60 t/d. Seed supply (feedstock_supply.md s9) and the merchant aquafeed market (market_demand.md s5) do not fill the larger plant; scenario `p2_research_spec` shows its returns.
- **The Phase 1 refinery is 15 t/d, not 20 t/d,** because 30% of the seed is soy, which yields only 12% oil.
- **The feed price list is treated as retail.** A 5% dealer margin and 0.5% bad debts are deducted.
- **Senior debt is sized to DSCR,** not taken at the financing file's USD 4.5m. The plant cannot carry USD 4.5m at a 1.30x minimum DSCR, so equity fills the gap.
- **The seed safety stock is calibrated** (1.5 months) so that peak stock (~41% of annual crush) falls inside feedstock_supply.md's 7-12 kt per 20 kt range.
