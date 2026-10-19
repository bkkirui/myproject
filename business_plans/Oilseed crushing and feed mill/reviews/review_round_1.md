# Independent adversarial review, round 1

**Plan reviewed:** `Business plan.md` (draft v1.1, 19 Oct 2026), `model/model.py` and its outputs, and the five research files.
**Reviewer stance:** a sceptical DFI investment-committee member, forensic model auditor and Kenyan agribusiness operator, with no stake in the plan.
**Date:** 19 October 2026.

## Verdict: REVISE

Five major issues are open.

## Summary

**What holds up.**
- `model.py` runs cleanly. Its outputs (`outputs.md` and all CSVs) reproduce byte for byte.
- The mass-balance, oil-routing and feed-mash checks close.
- Every headline figure in the plan that I spot-checked matches the model:
  - IRRs, NPVs, the 2031 P&L lines, funding uses and the Phase 1 equity of KES 1,279m.
  - The survival tree.
  - Case A from section 9.6: 42.6% conditional, 32.2% expected at a 30% failure probability, 35.8% at 20%. All reproduced.
- The plan's bottom line is sound: **do not commit to Phase 1 on current evidence**. Survival weighting is applied correctly against the 35–40% greenfield hurdle.

**What is wrong.** The errors mostly cut in the investor's favour, so the plan looks less risky than it is. Several of them also undermine the one thing the plan asks for now, which is USD 0.8m for Phase 0.

1. **The feed volume rests on an inflated market.** The model's merchant aquafeed market (SAM) is 45 kt in 2026 and includes Uganda and Tanzania. The research's own figures do not support that.
   - At the research's Kenya-only base of 30 kt, Phase 1 breaches its debt covenants and Phase 2 is a no-go.
   - Kill test K1 lets through a 20 kt market, where the minimum DSCR is 0.53x.
2. **The senior debt has no headroom.** It is sized to exactly 1.30x DSCR in 2030.
   - 9 of the 26 adverse one-at-a-time sensitivity settings breach the 1.10x default covenant.
   - The IRRs reported for those cases ignore what a default would do.
3. **The refined-oil price (KES 240/L ex-VAT) is unsupported, and the debt depends on it.** At the model's own low bound the plant defaults on the covenant.
4. **The headline claim that the project "clears WACC" is wrong.** The 23% WACC assumes 50% equity. The modelled structure is about two-thirds equity, which gives a WACC of about 27%, and project NPV at 27% is negative.
5. **The Phase 0 recommendation has no value-of-information case, and its pilot is unfunded and has no buyer.**
   - Even the state of the world that passes the gate is worth only about +KES 40m at 35%.
   - The proposed outgrower pilot buys 1,800–2,700 t of seed with no plant to crush it, and the budget does not include that seed.

## Prior-issue status

This is the first round, so there are no prior issues.

| ID | Status | Note |
|---|---|---|
| – | – | – |

## Open issues

### R1-01 (MAJOR): The merchant aquafeed SAM is inflated, and kill test K1 is set where Phase 1 would default

**Where:** Plan §2.3, §2.4, §12.2 (K1); `model.py` `sam_2026` = 45,000 t.

**Problem.** Feed is "the business": about 60% of revenue and 64% of gross margin. The volume driving it is 15% of a 45 kt SAM that grows 8% a year and includes the Ugandan and Tanzanian lake shores.

The research's own figures are smaller than that:
- `market_demand.md` row 21 gives Kenyan merchant demand of 20 / 30 / 40 kt.
- The same file (§1.5, §3.3) says exports to Uganda and Tanzania face De Heus (50–100 kt) and Tunga plants located inside those countries.
- Tanzania's entire commercial fish-feed use was 6.2 kt in 2023 ([UNCST], [DATED]).

The 45 kt base therefore credits about 15 kt of cross-border demand that the plan's own competitor analysis says is blocked.

**Evidence that even 20–40 kt may be high.**
- Victory Farms (VF) is about 25 kt a year company-wide, including Rwanda, and aims for 100 kt by 2030 ([KNA](https://www.kenyanews.go.ke/168926-2/), date uncertain). It raised money to scale "in Kenya and Rwanda" ([Business Daily, 2026](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840)).
- A search-result extract reports VF sales of about 1,400 t a month, or about 17 kt a year [UNVERIFIED: the page could not be identified].
- KNBS cage output was 28.1 kt in 2025.
- So VF is probably 60% or more of Kenyan cage output, with about 90% of its feed made in-house.
- Of what remains, part is served by SamakGro, which is VF-linked.

**Model runs** (senior debt held at the base KES 416m, gate on auto):

| SAM 2026 | Feed sold, 2031 | Equity IRR | Survival-weighted IRR | Minimum DSCR | Phase 2 |
|---|---|---|---|---|---|
| 45 kt (base) | 9.9 kt | 28.9% | 22.3% | 1.30 | go |
| 35 kt | 7.7 kt | 27.6% | 19.8% | 0.99 | no-go |
| 30 kt (research Kenya base) | 6.6 kt | 26.1% | 18.3% | 0.84 | no-go |
| 25 kt | 5.5 kt | 23.5% | 16.2% | 0.68 | no-go |
| 20 kt (K1 threshold) | 4.4 kt | 20.4% | 13.8% | 0.53 | no-go |

- K1 kills only below 20 kt of Kenyan merchant demand. A market just above that threshold passes K1 yet implies about 4.4 kt of feed in 2031. That is near the 2030 tripwire (4 kt), well below gate G1(b) (8 kt), and puts the plant in covenant default.
- The base case has no **competitor-response** path. Feed prices escalate with USD drift times FX, so they are flat in real terms, through the years when Tunga (45 kt, 2026) and SamakGro's 8 t/h geothermal plant are commissioning. SamakGro explicitly aims to make feed "more affordable" ([Capital FM, 2026](https://capitalfm.africa/fish-feed-firms-to-invest-sh510mn-at-kengens-olkaria-park/); commissioning date undisclosed).

**Required fix.**
1. Rebase the SAM to the contestable Kenyan merchant market: net of VF's captive feed and of SamakGro's sales to VF-linked farms. Treat Uganda and Tanzania as an upside case unless there is evidence of access.
2. Reconcile VF's Kenya-only output with KNBS.
3. Reset K1 to the SAM level at which the base clears both the covenant (DSCR of at least 1.30x) and the proceed test. Express K1 in the same units as the model's SAM.
4. Add a competitor-response scenario: a real feed-price decline of 1–3% a year from 2029, or a matched price cut by Tunga or SamakGro.

### R1-02 (MAJOR): Debt-covenant fragility is hidden, and sensitivity IRRs ignore default

**Where:** Plan §9.5, §9.6, §10.1, §11 risk 12; `model.py` `size_senior()` and `tornado()`.

**Problem.**
- Senior debt is sized so that the 2030 DSCR equals the 1.30x lock-up *exactly*. The plan admits that a 15% shortfall in CFADS breaches the 1.10x default covenant.
- The sensitivity table (tornado) and the scenarios report only IRRs and NPVs, holding the base debt fixed. The waterfall simply injects equity whenever there is a shortfall, so a covenant breach costs nothing in the model.

I re-ran every tornado setting and recorded the minimum DSCR from 2030:
- **9 of 26 adverse settings breach 1.10x.**
  - Seed cost ×1.26: −0.05x (negative CFADS).
  - Oil prices with fixed-price seed: 0.47x.
  - Feed price at its low bound: 0.61x.
  - Feed share 8%: 0.65x.
  - Seed supply ×0.70: 0.87x.
  - Sunflower oil yield 27%: 0.90x.
  - Feed dealer margin 10%: 1.01x.
  - Fixed opex ×1.25: 1.04x.
  - Oil prices at their low bound: 1.05x.
- Several more fall between 1.10x and 1.30x, which triggers lock-up.
- The 10% entrant-discount case gives 1.04x.

So the IRRs in the "low" column of §9.6 (for example 21.1% for feed price, 20.3% for share, 13.5% for seed cost) assume that lenders neither accelerate, sweep cash nor demand an equity cure. They also do not count any cure equity in the peak equity ask.

**Required fix.**
1. Report the minimum DSCR, and the equity cure needed, for every scenario and sensitivity.
2. Model default consequences: a cure injection with a dilution or penalty, a cash sweep, or a switch to the failure branch.
3. Size senior debt on a lender's downside case, for example 1.30x after a 15–20% CFADS haircut, or use repayments sculpted to CFADS. Then restate the equity requirement and the returns.
4. Add the debt-sizing result as an explicit FID condition. K8 currently tests only the quantum and the rate.

### R1-03 (MAJOR): The refined-oil price of KES 264k/t (KES 240/L ex-VAT) is unsupported, and the plant defaults at the model's own low bound

**Where:** Plan §2.1, §2.5, §4.1; `market_demand.md` row 9; `model.py` `p_refined`.

**Problem.** Refined oil is 28% of 2031 revenue and 35% of 2038 revenue, and it carries a refining spread of about KES 74k/t over the KES 190k/t crude transfer price. Yet:
- The price is a pure [ESTIMATE] with no quote.
- §2.5 claims "price parity to palm olein, with a modest health premium", but no refined palm-olein parity is computed anywhere.

**My parity estimate [ESTIMATE].**
- RBD olein FOB USD 1,252.5 ([Fastmarkets, 8 Sep 2026](https://www.fastmarkets.com/insights/correction-to-price-for-refined-bleached-deodorized-palm-olein-on-september-8-2026/)), plus freight of about USD 60, 25% CET, 4.5% IDF/RDL and USD 30 port costs: about USD 1,730/t, which is **about KES 225k/t, or KES 204/L ex-VAT**.
- At a 35% CET it would be about KES 220/L.
- KNTC Mama Pima loose oil sells at KES 185/L wholesale ([Kenya Times, Jul 2026](https://thekenyatimes.com/business/govt-unveils-mama-pima-cooking-oil-dispenser/)).
- A 20 L jerrican sold for about KES 5,100 at the 2022 price peak, when 1 L retail was KES 366–380 ([People Daily](https://peopledaily.digital/news/makers-warn-cooking-oil-prices-to-rise), [DATED 2022]). That is about KES 255/L including VAT, or about KES 220/L ex-VAT. Retail is now KES 358/L ([Business Daily, 2026](https://www.businessdailyafrica.com/bd/economy/cooking-oil-prices-climb-back-to-highs-of-2022-crisis-5548020)), close to that peak.

On this evidence, KES 240/L ex-VAT (KES 278/L including VAT, about KES 5,570 per jerrican) is 10–20% *above* parity for institutional bulk buyers, who are the most price-sensitive segment. It is not "parity plus a modest premium".

**Model runs.**

| Refined price | Equity IRR | Survival-weighted IRR | Minimum DSCR | Phase 2 |
|---|---|---|---|---|
| 231k (the model's own low bound) | 24.3% | 18.8% | 0.96 (default) | – |
| 215k | 24.6% | 16.9% | 0.79 | no-go |

**A related model-logic flaw.**
- Crude and refined prices are independent inputs, but the seed pass-through is indexed to crude.
- So lowering crude alone *raises* returns: crude at KES 150k gives an equity IRR of 31.0% and a minimum DSCR of 1.44x, because seed gets cheaper while the refined price is unchanged.
- KES 150k is the feedstock file's CPO-parity ceiling for local crude (`feedstock_supply.md` §2.4).

**Required fix.**
1. Build explicit landed-parity cases for RBD palm olein and refined sunflower oil, with the current CET band verified.
2. Obtain 20 L wholesale and institutional quotes in Kisumu and western Kenya.
3. Set the base refined price at parity plus an evidenced premium.
4. Link the refined price to crude (or both to an import-parity index) so that the spread cannot drift.
5. Add the refined price to the kill tests.

### R1-04 (MAJOR): "Project IRR clears WACC" is wrong for the capital structure actually modelled

**Where:** Plan §1 returns table, §9.4, §9.7; `financing_capital.md` §5; `model.py` `wacc_p1` and `wacc_ss`, gate (d).

**Problem.**
- The 23% Phase 1 WACC is derived from a structure of **50% equity at 35%**, 36% senior and 14% mezzanine (`financing_capital.md` §5).
- But the plan itself says the plant can carry only KES 416m of senior debt. Long-term Phase 1 funding is about **two-thirds equity** (KES 1,321m of 1,979m, §10.1).
- With the same layer costs, the WACC is 0.67 × 35% + 0.21 × 10.9% + 0.12 × 12.3%, which is **about 27%**.

| Discount rate | Project NPV, full plan | Project NPV, Phase 1 only |
|---|---|---|
| 23% (as in the plan) | +KES 423m | +KES 387m |
| 25% | +KES 135m | – |
| 27% (consistent with the modelled structure) | **−KES 102m** | about +KES 3m |

The project IRR of 26.1% is below a WACC consistent with the plan's own structure. The headline "Clears" verdict is therefore an internal contradiction.

The same issue affects Phase 2:
- Gate (d) tests Phase 2 at a 16.5% "steady-state" WACC that assumes 45% DFI debt and equity at 25% blended founder-plus-fund cost.
- In the base case, however, Phase 2 equity (KES 714m) comes from existing shareholders whose hurdle is 35–40%.
- Phase 2's incremental project IRR is 23.8%, and it dilutes equity IRR. Yet the model's gate says GO, and that GO feeds the 35% "go" branch of the survival tree.

**Required fix.**
1. Recompute the Phase 1 WACC from the modelled capital structure, and restate the headline table and §9.7.
2. Test gate (d) at the cost of the capital that would actually fund Phase 2: founder equity at 35%, or a priced outside-equity case.
3. Alternatively, model Phase 2 explicitly as an outside-equity raise at a stated valuation and show the founder's dilution or accretion.

### R1-05 (MAJOR): The Phase 0 recommendation (USD 0.8m "now") has no value-of-information case, and the outgrower pilot is unfunded and has no buyer

**Where:** Plan §1 (The ask, Recommendation), §10.4, §12.1, §12.5; `financing_capital.md` §6.

**Problem 1: the option value is not shown, and on the plan's own numbers it looks negative at the hurdle.**
- The only state that passes the proceed test is Case A (feed +10%, seed −10%, capex −15%) **plus** a failure probability of 20% or less.
- Even that state has an expected equity NPV at 35% of only **+KES 40m** (−KES 182m at 40%). This figure already includes the KES 112m Phase 0 cost.
- So Phase 0 has positive expected NPV at 35% only if the probability of reaching that state is roughly 70% or more.
- The plan's base values are central estimates, so the chance that three of them move favourably together *and* the failure risk falls is far lower than that.

The plan never states a probability of passing the gate, and never compares Phase 0 with cheaper ways of testing the decisive unknowns. Those are a feed-market survey, distributor price quotes and capex quotes, all desk or field work costing well under USD 0.3m. It also does not compare the restructure options (feed-mill-first, acquiring an existing mill, a JV), which the plan concedes may be the likely outcome.

**Problem 2: the pilot design does not work as written.**
- §12.5 item 3 and `financing_capital.md` §6 budget USD 250–400k for a **2,000–3,000 ha** outgrower pilot with weigh-and-pay in the 2027 long rains.
- At 0.9 t/ha that pilot produces about **1,800–2,700 t of seed**. At the KES 52k/t contract price, that is about **KES 95–140m of purchases**, about equal to the entire Phase 0 budget. It is not in the budget.
- There is no crusher until 2029, so the pilot has no buyer. The only processing mentioned is toll-pressing 20–50 t.
- A side-selling rate measured when the "buyer" is a pre-revenue startup that must resell the seed is not representative of the operating plant.
- The pilot is also larger than the plant's own year-1 outgrower base: about 1,300 ha in `feedstock_supply.md` §9.
- Contracts must be signed in Q1 2027, only weeks after incorporation and the recruitment of the outgrower manager.

**Required fix.**
1. Add an explicit value-of-information analysis: prior probabilities for the key inputs, the probability of passing G0, and the expected NPV at 35–40% of Phase 0 against stopping now.
2. Stage Phase 0 so the cheapest decisive tests come first, with a stop gate after them:
   - Stage 0a (about USD 0.2–0.3m): feed-market census, VF share, distributor and wholesale price quotes for feed and 20 L oil, three capex quotes.
   - Stage 0b: a pilot only if 0a passes.
3. Re-size the pilot to a level with a named offtaker (for example a back-to-back resale or toll-crush contract with Bidco or a Rift crusher), and budget seed working capital and price risk.
4. Evaluate the restructure alternatives within Phase 0 as first-class options.

### R1-06 (minor): The ask double-presents Phase 0, and the USD conversions mix FX years

**Where:** §1 The ask, §10.4.

- "USD 0.8m now" plus "USD 9.0m of Phase 1 equity" reads as USD 9.8m.
- But the KES 1,279m of Phase 1 equity (USD 8.98m) already includes the 2027 Phase 0 spend of KES 112m: equity injected in 2027 was KES 391m.
- Peak net equity of KES 1,994m is shown as "about USD 13.5m". At the 2032 FX rate, when the peak occurs, it is USD 12.0m.

**Required fix.** State the incremental Phase 1 ask net of Phase 0, and convert each figure at a stated FX date.

### R1-07 (minor): The research files conflict on oil parity, and the plan does not flag it

**Where:** §2.1; `feedstock_supply.md` §2.4 and §8; `market_demand.md` rows 5 and 8.

- The feedstock file puts CPO landed at **KES 150–166/kg** and calls it the ceiling on local crude value. It gets a base crush margin of about KES 12k/t, and says loss of the CPO duty "wipes out most of the margin".
- The market file puts CPO landed at **KES 185k/t** and local crude at **KES 190k/t**. The plan and model use these figures without a [CONFLICT] flag.
- The plan cites the crush-margin range (12–31k) but not the parity conflict that drives it.

**Required fix.** Flag the conflict, reconcile the CPO FOB and freight inputs, and show the base case at the lower parity. See also R1-03 on linking the oil prices.

### R1-08 (minor): The risk that minimum tax is reintroduced is missing

**Where:** §7.2, §11.

- The model pays no corporate tax until 2035.
- Kenya's 1% turnover minimum tax was struck down in 2021–22 ([Mondaq, Court of Appeal](https://mondaq.co.uk/capital-gains-tax/1269472/court-of-appeal-upholds-decision-declaring-minimum-tax-as-unconstitutional), [DATED]). Treasury's MTRS 2024/25–2026/27 commits to reintroducing a redesigned version ([IPF, Jan 2025](https://ipfglobal.or.ke/wp-content/uploads/2025/01/IS-A-MINIMUM-TAX-STILL-A-VIABLE-OPTION-FOR-KENYA.pdf)).
- At 1% of revenue over 2029–34, the exposure is about KES 200m nominal, falling in the cash-thin, covenant-tight years.

**Required fix.** Add the risk to the register with a probability and run it as a sensitivity.

### R1-09 (minor): VAT on capex is treated inconsistently

**Where:** `model.py` `vat_recov`; `regulatory_tax_risk.md` row 19.

- The model recovers 100% of capex VAT the following year.
- The research's 2%-of-feed-revenue irrecoverable-VAT estimate explicitly includes "capex depreciation", that is, the share of capex VAT attributable to exempt feed.
- If finished feed is exempt, the feed-attributable share of capex VAT (roughly KES 60–90m in Phase 1, more in Phase 2) is a cash cost up front, not a refund.

**Required fix.** Apportion capex VAT by expected taxable and exempt turnover, and keep the 2% for operating inputs only.

### R1-10 (minor): Gate thresholds are loose relative to the base case and the covenants

**Where:** §12.2 and §12.3.

- G1(b) accepts a 2031 feed gross margin of 20%, against a base of 37%. At 20%, 2031 EBITDA would be roughly KES 465m [ESTIMATE: 17 points × KES 1.8bn feed revenue], and the DSCR would be near or below default.
- K2 (KES 115/kg), K3 (KES 65k/t) and K6 (USD 12m) each admit cases with equity IRR of about 20–23% and covenant breach (see R1-02).

**Required fix.** Calibrate each kill and gate threshold to the covenant and hurdle results of the re-run model, not to the research's adverse bounds alone.

### R1-11 (minor): The survival tree models failure only in 2030

**Where:** §9.7; `survival_tree()`.

- Failure can occur only in 2030 and is liquidated in 2031. There is no later failure or impairment path, for example:
  - a Phase 2 hexane-plant start-up failure;
  - an exit-market failure;
  - an exit multiple taken at a cyclical peak.
- The 30% failure probability is the screening report's illustrative figure and is not derived for this business.
- The headline table also discounts the *survival-conditional* equity flows at the bond rate (+KES 3.43bn). The survival-weighted equivalent is +KES 1.52bn, and it is pre-shareholder-tax, whereas the bond is tax-free.

**Required fix.** Add a late-failure branch. Show the bond comparison on survival-weighted, after-shareholder-tax flows.

### R1-12 (minor): Financing realism details are omitted

**Where:** §8.2, §10.

- The GM's 3–5% equity incentive is not modelled as dilution.
- The financing research expects a founder personal guarantee and 125–150% collateral cover (`financing_capital.md` §2.3 and the term table). The plan omits both, and the failure branch assumes equity loss is capped at zero recovery.
- The financing file states that it rests on a single web search. Most of its terms are [PK-UNVERIFIED], which Appendix B does not disclose.
- A Phase 2 DFI loan in KES at 14% with a TCX hedge looks optimistic.
- On availability after the 2025 aid cuts, AgDevCo is still deploying FCDO-backed capital: AgDevCo Ventures reached a USD 49m first close in August 2026 ([AgDevCo PR, Aug 2026](https://www.agdevco.com/site/assets/files/2918/press_release_agdevco_ventures_-further_funding_announcement_august_2026.pdf)). That is supportive, but Ventures tickets are GBP 0.75–2.5m and need confirming against the USD 1.7m mezzanine.

**Required fix.** Add the guarantee and collateral to the risk register and to the founder's downside case. Model the GM's dilution. Disclose the evidence basis of the financing file.

### R1-13 (minor): Wording on the "first full year"

**Where:** §1.

2031 is described as the first full year. Commercial operation starts in April 2029, so 2030 is the first full year and 2031 is the first steady-state year.

**Required fix.** Correct the wording.

## Notes on items checked and found acceptable

- **Survival weighting against the hurdles** is done correctly: the IRR of probability-weighted cash flows is compared with the 35–40% expected hurdle, and the survivor IRR is checked against the 45–50% conditional figure.
- **Tax computation** is sound: the investment deduction, 5-year loss expiry, interest cap on foreign debt, WHT gross-up and CGT and dividend WHT. CGT at 15% and the 5% resident dividend WHT are consistent with current law as I understand it.
- **Mass balance and capacities** are internally consistent: extrusion runs at 86% of capacity in 2031 and the refinery peaks at 63% utilisation.
- **The GMO Court of Appeal judgment** was scheduled for 24 April 2026 ([KNA](https://www.kenyanews.go.ke/?p=159340)). I found no reported outcome, which is consistent with the plan's statement that it is pending. It needs checking on Kenya Law before FID.
