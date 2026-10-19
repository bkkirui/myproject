# Response to independent adversarial review, round 1

**Plan:** `Business plan.md` revised from draft v1.1 to **v2.0** (19 October 2026).
**Model:** `model/model.py` re-run after every change. `outputs.md`, `financial_model.xlsx` (now 13 sheets) and all CSVs are regenerated, including the new `voi_draws.csv`.
**New evidence:** `research/round1_evidence.md`.

## Summary

All 13 issues are accepted and addressed. None is disputed. The five major issues together reverse the plan's conclusion.

| Measure | v1.1 | v2.0 |
|---|---|---|
| Equity IRR, conditional on survival | 28.9% | **15.5%** |
| Equity IRR, survival-weighted | 22.3% | **8.9%** (founder, after GM dilution and shareholder tax: 7.6%) |
| Project IRR vs WACC | 26.1% vs 23% ("Clears") | **15.3% vs 32.3% (Fails)** |
| Senior debt | KES 416m, at exactly 1.30x | **0** on the lender downside test |
| Phase 2 | GO | **NO-GO** |
| Survival-weighted after-tax NPV at the 12.25% bond | not computed (+3.43bn survival-conditional) | **−KES 479m** |
| Recommendation | Fund USD 0.8m Phase 0 now | **Stop.** At most a USD 50k desk check; every Phase 0 policy has negative value of information |

Plan §9.8 bridges v1.1 to v2.0 step by step.

## Responses by issue

| ID | Severity | Action taken |
|---|---|---|
| **R1-01** | major | **Accepted and fixed.** See detail below |
| **R1-02** | major | **Accepted and fixed.** See detail below |
| **R1-03** | major | **Accepted and fixed.** See detail below |
| **R1-04** | major | **Accepted and fixed.** See detail below |
| **R1-05** | major | **Accepted and fixed.** See detail below |
| **R1-06** | minor | **Fixed.** Plan §1 and §10.3, and outputs.md §6 ("The ask, by stage, at stated FX"), now show each stage net of Phase 0 at a stated FX year: Phase 0a KES 41m (USD 0.30m at 2027 FX of 136.9); Phase 0b KES 75m including the expected pilot seed loss; FID equity net of Phase 0 KES 1,525m (USD 10.7m at 2028 FX of 142.4); standby KES 210m (USD 1.5m); peak equity KES 1,646m in 2030 (USD 10.7m at 2030 FX of 154.0). The reviewer's arithmetic on v1.1 (USD 12.0m at 2032 FX) was correct |
| **R1-07** | minor | **Fixed.** The [CONFLICT] is flagged and reconciled in plan §2.1 and round1_evidence.md §2.1. The feedstock file used the Indonesian reference price and omitted IDF/RDL and port costs; the market file's FOB was high. Reconciled CPO landed price: KES 177k/t. **The base crude price is set at the lower parity (KES 175k/t)** |
| **R1-08** | minor | **Fixed.** The minimum tax (1% of turnover where it exceeds CIT) is in the model at a 25% probability from 2028, as an expected value. It is in the tornado (certain: equity IRR 15.1%, minimum DSCR 0.67x) and in the risk register (risk 11), with court history, the MTRS commitment and its absence from Finance Bill 2026 cited |
| **R1-09** | minor | **Fixed.** Capex VAT is apportioned by the exempt (feed) turnover share: 35% for Phase 1 capex, using the 2029–31 mix. KES 93m is now an irrecoverable up-front cost. The 2% leakage is relabelled as operating inputs only. A tornado row tests zero-rated against exempt |
| **R1-10** | minor | **Fixed.** `calibrate_gates()` derives every † threshold in plan §12.2 from the re-run model: K1 24 kt, K2 KES 124/kg, K2b 15%, K3 KES 58k/t, K6 USD 9.9m, K11 KES 212k/t. G1(b) is raised from 20% to at least 9 kt at a margin of 30% or more, calibrated to the bull path, the only case in which Phase 2 is live (`g1_calibration()`). G1(e) now also requires no cure. Tripwires are updated, including "any covenant cure" |
| **R1-11** | minor | **Fixed.** A late-failure branch is added: base Phase 1 operations to 2034, liquidation in 2035, at 10% of survivors, for a total failure probability of 37%. Founder flows include the guarantee call and GM dilution. **The bond comparison now uses survival-weighted founder flows after dividend WHT and CGT: −KES 479m at 12.25%,** against +KES 397m on the old survival-conditional basis. A failure-probability sweep is reported. The plan states that no Kenyan base rate for the 30% exists (round1_evidence.md §5) |
| **R1-12** | minor | **Fixed.** The GM's 4% equity is modelled as dilution of the founder group (equity IRR 15.0% against 15.5%). The founder's personal guarantee is modelled in the failure branches and appears in the risk register (risk 12), with 125–150% collateral cover, and in the founder's downside (§10.1). On the modelled 20–35% recoveries the guarantee is not called; it bites only in a fire sale. Appendix B now discloses that `financing_capital.md` rests on one search, with most terms [PK-UNVERIFIED]. The TCX-hedged 14% is flagged as optimistic. AgDevCo Ventures (USD 49m first close, GBP 0.75–2.5m tickets) is cited as fitting the mezzanine ticket, with mezzanine appetite unconfirmed |
| **R1-13** | minor | **Fixed.** Plan §9.1 now calls 2030 the first full operating year and 2031 the first steady-state year (COD April 2029) |

### R1-01 (major): SAM rebase, K1 and competitor response

- **Victory Farms reconciled with KNBS.** Victory Farms runs at more than 1,400 t a month ([The Star, Jul 2026](https://www.the-star.co.ke/counties/nyanza/2026-07-03-victory-farms-bets-on-tech-and-talent-to-boost-fish-production)). Its Rwandan arm, Kivu Choice, runs at about 800 t a month ([New Times, 2026](https://www.newtimes.co.rw/article/36743/National/cepgel-governors-meet-in-gisenyi/amp)). Together these imply Victory Farms Kenya at about 13–16 kt in 2025, or about 45–60% of KNBS cage output. One KNA extract reads the 1,400 t as group-wide, which would put Victory Farms Kenya near 7 kt; that conflict is flagged.
- **SAM rebased.** `sam_2026` moves from 45 kt to **25 kt (15–37)**. It is now the contestable Kenyan merchant market: non-VF cage output × FCR, net of SamakGro's VF-linked share, plus ponds. The build-up is in round1_evidence.md §1.2 and plan §2.3.
- **Uganda and Tanzania are now an upside scenario only** (`sam_regional` 0 / 0 / 12 kt; scenario `regional_upside` gives 19.9%).
- **Competitor response.** The base now has a **1% a year real decline in feed prices** from 2029 (`feed_real_decline`). A **competitor-response scenario** at 3% a year plus a 10% entrant discount gives equity IRR 5.2% and minimum DSCR 0.04x.
- **K1 reset in model units.** It is now "contestable Kenyan merchant demand below **24 kt**", the hurdle-calibrated kill threshold (others at bull, p_fail 20%). The covenant break-even, with others at base, is 26.7 kt. Both are reported in §12.2.
- Feed in 2031 is now 5.5 kt, against 9.9 kt in v1.1.

### R1-02 (major): Covenants and debt sizing

- **Sizing.** `size_senior()` now sizes on a **lender downside case**: CFADS × 0.80 at 1.30x. The base carries **no senior debt**.
- **Default consequences are modelled** in a converging iteration (`run_fixed`):
  - below 1.10x, cure equity equal to the CFADS shortfall is injected and applied to prepay senior, plus a 1% waiver fee;
  - below 1.30x, distributions stop and 50% of excess cash is swept to prepay senior;
  - later instalments shrink pro rata.
- **Cure equity counts** in peak equity and in every IRR.
- **Reporting.** Every scenario, every tornado row (both sides), the joint cases and the VOI states report **minimum DSCR, cure equity and peak equity** (outputs.md §7, §8, §11; plan §9.5–9.6).
- **What it shows.** The base breaches 1.10x in 2030 on mezzanine alone (0.92x, KES 9m cure), as does every adverse tornado setting. Seed ×1.26 needs a KES 741m cure. A third PIK year on the mezzanine removes the base breach.
- **New FID test D1** (merged with K8): the lender's own downside sizing must give senior debt of at least KES 300m, with no cure in the base.
- **Alternative lender structures** are reported: testing from 2031 with a 24-month grace gives KES 177m of senior debt and an unchanged 15.4% equity IRR, because the project IRR roughly equals the cost of debt.

### R1-03 (major): Refined-oil price

- **Landed-parity table** in plan §2.1 and round1_evidence.md §2.2, covering:
  - RBD olein at three duty readings: "25% or USD 500/t" (the specific floor binds), 35%, and 25%;
  - duty-free (KNTC-type) and misdeclared imports;
  - imported refined sunflower oil;
  - local refiners' cost-plus from CPO;
  - the 2022 jerrican cross-check.
- The band is **KES 219–269k/t delivered to Kisumu**.
- **[CONFLICT] on the refined-oil duty.** Our reading of a USD 500/t specific floor (search extracts from The Standard and MPOB 2026) puts parity *higher* than the reviewer's 25% ad valorem estimate. The KRA tariff line is made a due-diligence item. **We do not use this to dispute the finding:** v1.1's 264k sat at the top of the band, with no premium evidenced.
- **Base refined price = crude + refining spread = KES 240k/t (KES 218/L ex-VAT)**, with a range of 215–265k. This matches the reviewer's jerrican-derived ~KES 220/L ex-VAT.
- **The refined price is now linked to crude** via `refine_spread`, so crude, refined oil and the parity-linked seed price move together. The "lower crude raises returns" flaw is gone: the tornado's oil-index row now runs 13.7% to 17.5% in the right direction.
- **K11 (refined oil below KES 212k/t) is a new kill test.** 20 L wholesale and institutional quotes in Kisumu are a Phase 0a/S0 deliverable.
- **No 2026 jerrican quote was found;** the plan says so.

### R1-04 (major): WACC and gate (d)

- **WACC is computed from the modelled structure** (`wacc_model`): 87% equity at 35%, 13% mezzanine post-tax and grossed up, giving **32.3%**. The 23% is kept as a memo only.
- **Headline reversed.** The plan's §1 verdict now reads "Fails": project NPV is −KES 976m at 32.3%, and −635m even at 23%.
- **Gate (d)** now requires a **positive incremental equity NPV at the 35% hurdle**, because existing shareholders fund Phase 2. The Phase 2 funding-mix WACC (21.1%) is reported for the project view.
- **Phase 2 is now a no-go** in the base: incremental equity IRR 0.6%, incremental equity NPV −KES 413m. The survival tree gives Phase 2 a zero probability when the base gate fails.
- **Outside-equity variation.** Phase 2 equity priced by an outside investor is kept as G1(f). It is not modelled, because Phase 2 is live only in the bull case.

### R1-05 (major): Value of information and Phase 0 design

- **`voi_analysis()`** runs 150 Monte Carlo states for each of two priors:
  - triangular priors on SAM, feed price, share, feed decline, capex, oil index and refining spread, which Phase 0a reveals;
  - the same on seed cost and supply, which Phase 0b reveals;
  - independent priors, and a Gaussian copula with ρ = 0.5 among favourable outcomes.
- **Policies valued:** stop, invest without information, Phase 0a only, staged 0a then 0b, and perfect information. Each is valued as the survival-weighted founder NPV at 35% and 40%, at p_fail 30% and 20%.
- **Result.**
  - Every Phase 0 policy is worse than stopping.
  - P(pass G0) is 0% under independent priors and 2–3% under correlated ones.
  - The gross value of perfect information is at most KES 12m, against KES 41m for Phase 0a.
  - Results are in plan §12.6, outputs.md §10 and `voi_draws.csv`.
- **Phase 0 restaged** (§12.5): an optional **S0 desk check (≤ USD 50k)**, then 0a (USD 0.3m), then 0b (USD 0.5m plus USD 0.05m expected seed loss), each with a stop gate.
- **Pilot re-sized** to 500–600 ha (about 500 t of seed), with a signed back-to-back resale contract with a named crusher before planting. The seed working capital (about KES 26–30m, revolving) and the expected loss are budgeted.
- **Restructure options are first-class alternatives** (§9.5, §12.7):
  - feed-mill-first (9.6%) and crusher-only (1.5%) are modelled through `config`;
  - acquisition and JV are assessed qualitatively;
  - redeploying to bonds or higher-ranked opportunities is compared.
- **The recommendation changes to stop.**
