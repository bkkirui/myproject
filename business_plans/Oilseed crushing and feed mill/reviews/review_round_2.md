# Independent adversarial review, round 2

**Plan reviewed:** `Business plan.md` draft v2.0, with `model/model.py`, `model/outputs.md`, `model/README.md`, `research/round1_evidence.md` and `reviews/response_round_1.md` (all dated 19 October 2026).
**Reviewer stance:** sceptical DFI investment-committee member, forensic model auditor and Kenyan agribusiness operator. I have no stake in the plan.
**Date:** 19 October 2026.

## Verdict: APPROVE (no open major issues)

v2.0 reverses v1.1's conclusion. It now recommends **not building and not funding Phase 0 as designed**, with at most a USD 50k desk check. On the evidence, that conclusion is correct and robust.

**Model re-run.** I copied the model to a scratch directory and ran it (2 min 42 s). The regenerated `outputs.md` is byte-identical to the committed file, so every model figure in the plan reproduces.

**Why the stop verdict holds.** It does not depend on the contestable judgement calls: the 30% failure probability, the bear-case failure branch, the VOI priors or the 35% discount rate.
- The base equity IRR **conditional on survival** is 15.5%. That is below even the 25–30% hurdle for an *established* business.
- No single driver within its research range reaches 35%. The best is seed ×0.79, at 26.0%.
- The SAM high case (37 kt) gives 19.9%. Adding Uganda and Tanzania demand also gives 19.9%. v1.1's Case A gives 28.1%.
- Only the joint bull case clears the 35% survival-weighted hurdle, and only at a 20% failure probability.

**Remaining problems.** All are minor:
- one kill threshold (K11, refined oil) is converted into the wrong units;
- one executive-summary sentence about the kill thresholds is not true in the model;
- the risk register's probability of a feed price war is inconsistent with the base case;
- the minimum-tax risk omits the 2025 statutory repeal;
- a few disclosure gaps.

None of them changes the decision. Each would matter only if the case were reopened.

## Prior-issue status (verified against the current files, not the reviser's summary)

| ID | Sev. (R1) | Status | Verification note |
|---|---|---|---|
| R1-01 | major | **Resolved** | `sam_2026` is 25 kt (range 15–37), built up in round1_evidence.md §1.2 net of Victory Farms (VF) captive feed and SamakGro's VF-linked sales. Uganda and Tanzania are upside only (`sam_regional` = 0 in the base). The base has a 1%/yr real feed-price decline (model.py l.702) and a competitor-response scenario (3%/yr plus a 10% entrant discount: 5.2% IRR, min DSCR 0.04x). K1 is recalibrated in model units (23.7 kt kill; 26.7 kt covenant). My own search supports the base Kenya-only reading of VF: a July 2026 search extract of The Star attributes the >1,400 t/month to the **Sindo** facility in Homa Bay, Kenya ([The Star, 3 Jul 2026](https://www.the-star.co.ke/counties/nyanza/2026-07-03-victory-farms-bets-on-tech-and-talent-to-boost-fish-production)). An Oct 2026 KNA extract calls it group sales ([KNA](https://www.kenyanews.go.ke/?p=168926)); that [CONFLICT] is flagged in the plan |
| R1-02 | major | **Resolved** | `size_senior()` sizes on CFADS ×0.80 at 1.30x. `finance_and_returns()` injects cure equity below 1.10x (prepaying senior, plus a waiver fee) and applies a 50% sweep in lock-up. `run_fixed()` iterates to convergence. Min DSCR, cure equity and peak equity are reported for every scenario, both sides of every tornado row, every joint case and every VOI draw. Debt capacity is FID test D1 |
| R1-03 | major | **Resolved** | Refined = crude + `refine_spread` (model.py l.679). The parity table covers three duty readings, duty-free and misdeclared imports, local CPO refiners and a 2022 jerrican cross-check. The base of 240k sits between the local-refiner floor (~219k) and the import ceiling (246–269k). K11 is added, but see R1-10 for a units error. My search could not confirm the 2026 refined-oil duty either ("25% or USD 500/t" is confirmed only in 2023 reporting; Capital FM cites 35%); the plan correctly makes it a due-diligence item |
| R1-04 | major | **Resolved** | The WACC is computed from the modelled 2027–29 sources: 32.3% (87% equity). The headline verdict is reversed to "Fails". Gate (d) now tests incremental equity NPV at 35%. I also tested gate (d) at the established-business 27.5%, since Phase 2 is decided on an operating business: the incremental equity NPV is still −KES 505m, so the no-go holds |
| R1-05 | major | **Resolved** | The `voi_analysis()` Monte Carlo puts every Phase 0 policy below stopping. Phase 0 is restaged (S0 ≤ USD 50k, then 0a USD 0.3m, then 0b) with stop gates. The pilot is cut to 500–600 ha with a back-to-back buyer and budgeted seed working capital. Feed-mill-first (9.6%) and crusher-only (1.5%) are modelled; acquisition and JV are assessed qualitatively. The recommendation changes to stop |
| R1-06 | minor | **Resolved** | The ask is stated by stage, net of Phase 0, at stated FX years. The arithmetic checks: 1,525 / 142.4 = USD 10.7m; 1,646 / 154.0 = USD 10.7m |
| R1-07 | minor | **Resolved** | [CONFLICT] flagged and reconciled (FOB ~USD 1,100; landed KES 177k). The base crude price uses the lower parity, 175k |
| R1-08 | minor | **Resolved** | Minimum tax is modelled at a 25% probability as an expected value, with a tornado row and risk 11. A new fact affects the probability: see R2-03 |
| R1-09 | minor | **Resolved** | Capex VAT is apportioned by exempt turnover (model.py l.849–851): KES 93m irrecoverable. The 2% leakage now covers operating inputs only |
| R1-10 | minor | **Partially resolved** | `calibrate_gates()` calibrates the thresholds in the model, and G1(b) is tightened. However, **K11 is converted into KES/t at base crude (175k) while it was calibrated with crude at its bull value (187.5k)**, so the stated 212k/t is too loose. Carried forward below |
| R1-11 | minor | **Resolved** | Late-failure branch added (7% of the total), plus a failure-probability sweep. The bond comparison uses survival-weighted founder flows after shareholder tax: −KES 479m at 12.25% |
| R1-12 | minor | **Resolved** | The GM's 4% is modelled as dilution. The guarantee is modelled in the failure branches and appears in risk 12. Appendix B discloses that the financing file rests on a single search. AgDevCo Ventures is noted. The TCX-hedged 14% loan is flagged as optimistic |
| R1-13 | minor | **Resolved** | §9.1 now reads "2030 first full year; 2031 first steady-state year" |

## Open issues

### R1-10 (minor, carried forward): K11 refined-oil kill threshold is in the wrong units
- **Location.** Plan §12.2 K11, §9.6 break-even table ("refined 212k, KES 193/L"), §4.4 LOI condition, risk 4; `calibrate_gates()`.
- **Problem.** The kill value of the refining spread (37.3k) was found with every other driver at bull, **including crude at 187.5k**. The plan converts it to a refined price at base crude: 175k + 37.3k = 212k. At bull crude the threshold refined price is **224.8k/t (about KES 205/L ex-VAT)**.
- **Evidence.** My re-run, with others at bull:
  - spread 37,256 gives refined 224,756 and a survival-weighted IRR (p_fail 20%) of exactly 35.0%;
  - refined at 212k with bull crude (spread 24.5k) gives 33.4%.

  The K11 gate as written therefore admits a failing case. The same ambiguity applies to the `p_crude` kill (122k, at bull spread).
- **Required fix.** State K11 as the refined price at the crude price used in the calibration (about 225k/t, or KES 205/L ex-VAT). Alternatively, calibrate directly on the refined price with crude at base. Update §4.4, §9.6, §12.2 and risk 4 to match.

### R2-01 (minor): the executive-summary claim about kill thresholds is not true in the model
- **Location.** Plan §1 Recommendation ("If any one of feed market size, feed price, share, seed cost or capex turns out at its base value or worse, the plant fails the hurdle even with every other driver at its favourable (bull) value") and §9.6 ("the case still fails if SAM, feed price, share, seed cost or capex comes in at base or worse").
- **Problem.** Four of the five kill thresholds sit slightly on the *adverse* side of base:
  - SAM 23.7 kt against a 25 kt base;
  - feed price ×0.991;
  - seed cost ×1.014;
  - capex ×1.040.

  So at base, with the others at bull, the plant *passes*. Only share (15.3% against 15%) behaves as claimed.
- **Evidence.** My re-run, setting one driver at base with the others at bull, gives these survival-weighted IRRs at p_fail 20%:

  | Driver at base | IRR |
  |---|---|
  | SAM | 37.0% |
  | Feed price | 35.4% |
  | Seed cost | 35.6% |
  | Capex | 35.9% |
- **Required fix.** Reword it, for example: "the kill thresholds sit within 1–4% of the base values: a driver only slightly worse than base fails the hurdle even with every other driver at bull." The substantive message (no margin of safety) is unchanged.

### R2-02 (minor): the risk register's price-war probability is inconsistent with the base feed-price path
- **Location.** Plan §11 risk 2 ("About 50% that real prices fall 3% a year or more") against the base `feed_real_decline` = 1%/yr (Appendix A; model.py l.128).
- **Problem.** If the plan believes a 50% chance of a decline of 3% a year or more, then the median decline is at least 3%/yr and the probability-weighted path is well above 1%/yr. The base is therefore optimistic relative to the plan's own risk assessment. The error runs in the direction that *strengthens* the stop verdict, so it does not change the decision.
- **Evidence.** The tornado shows 3%/yr gives 5.5% equity IRR and a 0.54x min DSCR. My search found no published 2026 feed price cut (consistent with round1_evidence.md §1.3). WorldFish still cites commercial feed at about USD 1.00–1.24/kg ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back), undated).
- **Required fix.** Either lower the stated probability to match a 1% base, for example "about 20–25% that prices fall 3% a year or more", or move the base path to the probability-weighted decline.

### R2-03 (minor): the minimum-tax risk omits the Finance Act 2025 repeal
- **Location.** Plan §7.2, §7.4 and risk 11; round1_evidence.md §3.
- **Problem.** The plan records the court strike-down, the MTRS commitment and the absence of a minimum tax from Finance Bill 2026. It does not record that **the Finance Act 2025 repealed s.12D of the Income Tax Act** (the minimum-tax provision), bringing the statute into line with the Court of Appeal ruling. Reintroduction would now need fresh primary legislation that survives the constitutional objection, which arguably lowers the 25% probability. The effect is tiny: certain/never moves equity IRR by only 0.6 points.
- **Evidence.** EY, "Kenya enacts Finance Act 2025", 16 July 2025 ([EY](https://taxnews.ey.com/news/2025-1498-kenya-enacts-finance-act-2025)), as read through a search extract.
- **Required fix.** Add the repeal to the minimum-tax row and risk 11, and either justify the 25% probability or lower it.

### R2-04 (minor): the "3 PIK years" remedy is an off-model run
- **Location.** Plan §9.6 ("Deferring mezzanine cash interest one more year ... minimum DSCR 2.15x [supplementary run]"), §10.1 terms column, risk 6; model.py l.303 (`mezz_pik_years` low/base/high = 0 / 2 / 2).
- **Problem.** The base breach in 2030 is cured by a term that the parameter table cannot represent: the high bound of `mezz_pik_years` is 2. The §10.1 column headed "Terms (model)" lists "3 PIK years needed", which reads as though 3 is modelled.
- **Evidence.** I confirmed the claim: with `mezz_pik_years` = 3, equity IRR is 15.6% and min DSCR 2.15x.
- **Required fix.** Widen the parameter range to include 3, add a tornado or alternative-structure row, and relabel the §10.1 entry "negotiating target (not in base)".

### R2-05 (minor): VOI precision and the failure-branch construction are not disclosed
- **Location.** Plan §12.6, Appendix B; `voi_analysis()`, `_components()`, `half()`.
- **Problem.**
  1. With 150 draws, "P(pass) = 0.0%" has a 95% upper bound of about 2%, and the 2.0–3.3% figures under ρ = 0.5 rest on 3–5 draws. No Monte Carlo error is reported.
  2. In every VOI state and kill calibration, the early-failure branch is the *fixed global* bear case: `half()` reads `ASSUMPTIONS` base values, not the drawn state. Meanwhile senior debt is re-sized to the drawn state, so in favourable states the failure branch runs bear operations with KES 300–600m of senior debt.

  Neither point changes the conclusion. At P(pass) = 5% and a passing-state NPV of about +KES 140–300m, the gross value of information is about KES 7–15m, still well below Phase 0a's KES 41m. Both should still be disclosed.
- **Required fix.** Report binomial confidence intervals for P(pass) and the gross value of information, or raise the draws to 1,000 or more. State in §9.7 and §12.6 that the failure branch is state-independent bear operations, carrying the state's sized debt.

## Checks performed (no issue found)

**Model and arithmetic**
- The model reproduces exactly; all 19 internal checks pass, with one "CHECK" flag: the 2030 covenant cure, which is disclosed.
- 2031 mass balance:
  - oil: 9,450×31% + 4,050×12% = 3,416 t;
  - oil split 130 + 2,628 + 657;
  - refinery 2,497 + 131;
  - process losses 715 = 472 + 243.
- Revenue mix: feed 42% in 2031 and 57% in 2038. The plan's tables match `pnl_annual.csv` and `outputs.md`.
- WACC: 0.87×35% + 0.13×(mezzanine at about 13.9% post-tax) ≈ 32.3%.
- Survivor IRR needed: (1.35⁵ / 0.63)^(1/5) − 1 = 48.1%.
- Equity totals: 391 + 946 + 300 = 1,637 (Phase 1 equity); +9 cure = 1,646 (peak).
- The stop verdict is robust to the VF [CONFLICT]: the SAM high case (37 kt) still gives only 19.9%.

**Spot checks of sources and dates**
- The Kenyan election on 10 August 2027 is the constitutional second Tuesday of August.
- No 2026 Court of Appeal GMO judgment was found. The March 2025 conservatory order is still the latest reported ([Citizen Digital](https://citizen.digital/article/blow-to-govt-as-court-of-appeal-bars-importation-of-gmos-n358801); [Capital FM](https://capitalfm.africa/coa-halts-gmo-importation-pending-appeal/)), consistent with the plan.
- No 2026 Kisumu feed or 20 L oil quote was found, consistent with the plan's due-diligence list.

## Notes for the founder (not issues)
- The comparison that decides the case is simple: **15.5% conditional on survival, against 25–30% even for an established business.** The heavier machinery (survival tree, VOI, gate calibration) confirms that result and is not needed to reach it.
- If the founder still wants to explore the case, the plan's S0 desk check is correctly sized and focused: VF's Kenyan output, non-VF feed use, and Kisumu feed and 20 L oil quotes. Use the corrected K11 (about KES 225k/t) in its stop rule.
