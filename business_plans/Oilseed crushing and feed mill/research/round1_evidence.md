# Round 1 evidence file: market rebase, oil parity, tax and financing points

Prepared 19 October 2026 in response to `reviews/review_round_1.md`. FX KES 129.8/USD; 1 t of oil = 1,099 L.
Conventions as in the other research files: **[ESTIMATE]** = analyst figure with reasoning; **[DATED]** = source older than 2025; **[CONFLICT]** = sources disagree; **[UNVERIFIED]** = weak source or search-result extract only. Direct page fetches were not attempted beyond search results, so every figure below was read through search extracts and needs checking against the primary page.

---

## 1. Contestable Kenyan merchant aquafeed market (R1-01)

### 1.1 Victory Farms' Kenya-only output, reconciled with KNBS

| Evidence | Figure | Source |
|---|---|---|
| Victory Group output, company-wide | ~25,000 t/yr; target 100,000 t by 2030 | [KNA](https://www.kenyanews.go.ke/168926-2/) (page date uncertain; extract dated Oct 2026) |
| Victory Farms monthly output (Nyanza article) | ">1,400 tonnes of fish per month", aiming for 2,000 t/month by end-2026 | [The Star, 3 Jul 2026](https://www.the-star.co.ke/counties/nyanza/2026-07-03-victory-farms-bets-on-tech-and-talent-to-boost-fish-production) |
| Kivu Choice (Rwanda arm) | ~800 t/month, "more than half of the country's farmed fresh fish"; 9,000 t/yr base, 30,000 t target | [New Times, 2026](https://www.newtimes.co.rw/article/36743/National/cepgel-governors-meet-in-gisenyi/amp); [New Times](https://www.newtimes.co.rw/article/34852/National/eac-tax-authorities-adopt-international-standards/amp) |
| Group 2026 target | 30,000 t | [Business Daily, 2026](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840) (via search extract) |
| KNBS cage output | 13,700 t (2021) to 28,100 t (2025) | KNBS via [Ecofin](https://www.ecofinagency.com/news-agriculture/1703-53851-kenya-s-fish-farming-boom-draws-new-bet-from-victory-farms) |

**Reconciliation [ESTIMATE].**
- If The Star's 1,400 t/month is the Kenyan operation (the article is a Nyanza county story), Kenya runs at about 16.8 kt/yr in mid-2026. Add Kivu Choice's ~9.6 kt/yr and the group is ~26 kt, which matches the "25,000 t" group figure. **[CONFLICT/UNVERIFIED]:** an October 2026 KNA extract describes the same 1,400 t/month as group sales "across Kenya and Rwanda". On that reading Kenya is only ~7 kt/yr. The first reading is internally consistent with the group total, so it is the base; the second is the high-merchant case.
- Victory Farms' Kenyan 2025 output was therefore roughly 13–16 kt, against 28.1 kt of KNBS cage output: **about 45–60% of Kenyan cage output is Victory Farms**, and about 90% of its feed is made in-house ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840)).
- This is consistent with KNBS counting Victory Farms. If KNBS undercounted Victory Farms, the non-VF residual would be larger; no evidence of that was found.

### 1.2 Build-up of the contestable merchant SAM, 2026 [ESTIMATE]

| Item | Low | Base | High | Basis |
|---|---|---|---|---|
| KNBS-basis cage output, 2026 (kt) | 30 | 32 | 34 | 28.1 kt in 2025, growing 7–20% ([market_demand.md row 18](market_demand.md)) |
| less Victory Farms Kenya (kt) | 18 | 16 | 14 | §1.1 |
| = non-VF cage output (kt) | 12 | 16 | 20 | |
| × FCR | 1.5 | 1.6 | 1.8 | [market_demand.md row 19](market_demand.md) |
| × share not tied to SamakGro/VF-linked supply | 75% | 85% | 90% | No data on SamakGro's sales to VF-linked or contracted farms; judgement |
| = contestable non-VF cage feed (kt) | 13.5 | 21.8 | 32.4 | |
| + pond and hatchery extruded feed (kt) | 1.5 | 3.0 | 5.0 | ~8 kt pond fish × 1.5 FCR, only part on commercial extruded feed ([market_demand.md §3.2](market_demand.md)) |
| **Contestable Kenyan merchant SAM, 2026 (kt)** | **15** | **25** | **37** | Model `sam_2026` = 15 / 25 / 37 kt |
| Uganda and Tanzania lake shores (kt) | 0 | **0** | 12 | Upside only (`sam_regional`): De Heus Njeru (50–100 kt) and Tunga Uganda sit inside those markets ([market_demand.md §1.5, §3.3](market_demand.md)); Tanzania's commercial fish-feed use was 6.2 kt in 2023 ([UNCST](https://nru.uncst.go.ug/bitstreams/4670621e-4062-4039-9bc1-f274e4da36df/download)) [DATED] |

The base (25 kt) sits in the lower half of the research's 20–40 kt Kenyan merchant range ([market_demand.md row 21](market_demand.md)), because that range was not net of SamakGro's VF-linked sales. v1.1 used 45 kt including Uganda and Tanzania.

### 1.3 Competitor response (feed prices)

- Tunga Nutrition (Skretting/Nutreco + Unga) raised extrusion capacity from 24 kt to 45 kt a year around February 2026 ([WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi)).
- SamakGro, Maxim Agri and Gatsby are building an 8 t/h geothermal-powered plant at Olkaria, aimed at making feed more affordable; no construction timeline or commissioning date has been disclosed ([Capital FM, 2026](https://capitalfm.africa/fish-feed-firms-to-invest-sh510mn-at-kengens-olkaria-park/); [Food Business MEA](https://www.foodbusinessmea.com/?p=2161573)).
- A search extract also mentions a DiscoverAqua feed facility at Athi River due to start in Q3 2026. The source page could not be identified, so this is **[UNVERIFIED]**.
- **No 2026 feed price cut was found.** Feed is still reported as 60–70% of production cost, and commercial feed at about USD 1.00–1.24/kg ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back), undated).
- **Modelling choice [ESTIMATE].** The base has a 1% a year real decline in feed prices from 2029. A competitor-response scenario has 3% a year plus a 10% entrant discount, and the tornado runs 0–3%.

---

## 2. Edible-oil parity (R1-03, R1-07)

### 2.1 The CPO conflict, reconciled

| | market_demand.md rows 4–5 | feedstock_supply.md §2.4 | **Round 1 reconciliation** |
|---|---|---|---|
| CPO FOB (USD/t) | 1,150 (RM 4,500–4,600 at RM 4.04–4.08 per USD) | 1,007.5 (Indonesian reference, Sep 2026) and 1,091 (Malaysian reference, Oct 2026) | **1,100.** The Malaysian Oct 2026 reference is USD 1,091 ([Bernama](https://www.bernama.com/en/news.php?id=2604287)). Indonesia's reference is an export-levy base, not a traded FOB price |
| Freight and insurance | 60 | included | 60 + 4 |
| Duty | 10% | 10% | 10% on CIF = 116 |
| IDF + RDL | 5.5% | omitted | 4.5% (2.5% + 2.0%, plan §7.2) = 52 |
| Port and clearing | 30 | omitted | 30 |
| **Landed Mombasa** | KES 185k/t | KES 150–166k/t | **USD 1,362 = KES 177k/t (KES 161/L)** |

**[CONFLICT] resolved.**
- The feedstock file's 150–166k left out the IDF/RDL levies and port costs, and used the Indonesian reference. The market file's FOB was slightly high.
- Refiners can switch between local crude and CPO, so local crude sells at about CPO parity ([feedstock_supply.md §2.4](feedstock_supply.md)).
- **The model's crude oil price (`p_crude`) is set at KES 175k/t, the lower parity.** v1.1 used 190k.
- High case: crude sunflower oil parity of KES 209k less 5% (about 200k). Low case: 155k, for CPO duty loss plus weaker palm prices.

### 2.2 Refined oil: import ceiling and local floor

**Duty on refined oils [CONFLICT].**
- An EY table lists RBD palm olein (HS 1511.90.30) at a 35% CET, with a proposed new rate of "25% or USD 500/MT, whichever is higher" ([EY, Jul 2023](https://globaltaxnews.ey.com/news/2023-1308)) [DATED].
- Search extracts from the [Standard](https://standardmedia.co.ke/sports/business/article/2001498266/www.digger.co.ke) and a 2026 MPOB news item quoting Kenyan manufacturers ([MPOB, Apr 2026](https://prestasisawit.mpob.gov.my/en/palmnews/news/35498)) say Kenya applies **25% or USD 500/t, whichever is higher**, on refined soya, RBD palm olein, other palm oil, refined sunflower and refined corn oil under an EAC stay.
- Capital FM (2024) says imported refined palm oil pays 35%, and that refined oil has been misdeclared as crude to pay 10% ([Capital FM](https://www.capitalfm.co.ke/business/?p=98825)) [DATED].
- An FNJ guide says EAC Gazette Notice No. 19 of 2025 lowered CET rates for Kenya on several refined-oil lines, without giving the rate ([FNJ](https://fnjassociates.co.ke/a-guide-to-customs-import-duty-in-kenya/)) [UNVERIFIED].
- **Verify against the current KRA tariff before FID.** At current prices, the USD 500/t specific floor binds (25% of a USD 1,317 CIF is only USD 329), so the specific rate matters a great deal.

**Landed and delivered parity, 20 L bulk, ex-VAT [ESTIMATE]** (USD/t unless stated):

| Case | CIF | Duty | IDF/RDL + port | Landed Mombasa | KES k/t | + Mombasa–Kisumu freight (KES 5.7k), 20 L packing (KES 8.8k), 3% trade margin | Delivered Kisumu, KES k/t (KES/L) |
|---|---|---|---|---|---|---|---|
| RBD olein, 25% or USD 500/t (binding: 500) | 1,317 (FOB 1,252.5 + 60 + 4) | 500 | 59 + 30 | 1,906 | 247 | +22 | **269 (245/L)** |
| RBD olein, 35% ad valorem | 1,317 | 461 | 89 | 1,867 | 242 | +22 | 264 (240/L) |
| RBD olein, 25% ad valorem (the reviewer's case) | 1,317 | 329 | 89 | 1,735 | 225 | +21 | 246 (224/L) |
| RBD olein misdeclared as crude (10%) | 1,317 | 132 | 89 | 1,538 | 200 | +21 | 221 (201/L) |
| RBD olein duty-free (KNTC-type waiver) | 1,317 | 0 | 89 | 1,406 | 182 | +20 | 202 (184/L) |
| Local refiner from CPO (cost-plus: CPO 177k + 8% loss + KES 4k chemicals/energy + packing + freight Thika–Kisumu KES 5k + 5% margin) | | | | | | | **~219 (199/L)** |
| Refined sunflower, imported (FOB about 1,370; freight 100) | 1,474 | 500 | 66 + 30 | 2,070 | 269 | +23 | 292 (266/L) |

**Cross-checks.**
- A 20 L jerrican cost KES 5,100 at the 2022 peak, when 1 L retail was KES 366–380 ([People Daily](https://peopledaily.digital/news/makers-warn-cooking-oil-prices-to-rise)) [DATED]. That is KES 255/L including VAT, KES 220/L ex-VAT, or **KES 242k/t**.
- Retail salad oil was KES 358.09/L in July 2026, close to the 2022 peak ([Business Daily](https://www.businessdailyafrica.com/bd/economy/cooking-oil-prices-climb-back-to-highs-of-2022-crisis-5548020)). The same 20 L-to-retail ratio would give about KES 240k/t today.
- KNTC Mama Pima loose palm olein sells at KES 185/L wholesale ([Kenya Times, Jul 2026](https://thekenyatimes.com/business/govt-unveils-mama-pima-cooking-oil-dispenser/)). If VAT-inclusive, that is KES 159/L ex-VAT, close to the duty-free import case. It is a policy-driven tail, not the market.
- **No 2026 quote for a 20 L jerrican was found in any search.** This is a Phase 0a deliverable.
- Sunflower premium: Kenyan CIF import unit values in Q2 2025 were KES 153.9k/t for sunflower oil and KES 136.6k/t for palm, 13% higher ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)). That is an import-cost premium. **No evidence of a consumer or institutional price premium for 20 L sunflower oil was found**, so the base assumes none.

**Modelling choice.**
- Refined price = crude price + a refining spread (`refine_spread`). The base spread is KES 65k/t, giving **KES 240k/t (KES 218/L ex-VAT)**, near the midpoint of the local-refiner floor (219k) and the import ceiling (246–269k) and matching the 2022 jerrican cross-check.
- Range: spread of 40k / 90k, which is KES 215k / 265k at base crude.
- v1.1 had an unlinked KES 264k/t, at the top of the band.

---

## 3. Minimum tax (R1-08)

| Item | Evidence |
|---|---|
| Design | Finance Act 2020: 1% of gross turnover, payable where it exceeds the CIT liability ([People Daily](https://peopledaily.digital/business/think-tank-floats-steps-for-minimum-tax-resumption/amp)) |
| Court history | Declared unconstitutional; Court of Appeal upheld ([Mondaq](https://mondaq.co.uk/capital-gains-tax/1269472/court-of-appeal-upholds-decision-declaring-minimum-tax-as-unconstitutional)) [DATED] |
| Policy intent | The Medium-Term Revenue Strategy 2024/25–2026/27 commits to reintroducing a redesigned minimum tax ([IPF, Jan 2025](https://ipfglobal.or.ke/wp-content/uploads/2025/01/IS-A-MINIMUM-TAX-STILL-A-VIABLE-OPTION-FOR-KENYA.pdf)) |
| Finance Bill 2026 | No minimum tax found in summaries ([KPMG, May 2026](https://kpmg.com/us/en/taxnewsflash/news/2026/05/kenya-tax-proposals-finance-bill-2026.html); [CDH, May 2026](https://www.cliffedekkerhofmeyr.com/en/news/publications/2026/Kenya/Tax-Exchange-Control/tax-and-exchange-control-alert-8-may-Analysis-of-the-Finance-Bill-2026)), based on search extracts only |

**Modelling choice [ESTIMATE].** 25% probability from 2028, applied as an expected value: tax = CIT + 25% × max(0, 1% × revenue − CIT). The tornado runs certain / never.

---

## 4. Financing evidence basis (R1-12)

- `financing_capital.md` rests on **one** web search. Most of its terms are [PK-UNVERIFIED] prior knowledge, including the rates, tenors, the founder guarantee and 125–150% collateral cover, the AGF guarantee terms and the TCX-hedged KES pricing (file header and §2).
- AgDevCo is still deploying after the 2025 aid cuts. AgDevCo Ventures reached a USD 49m first close in August 2026, with tickets of GBP 0.75–2.5m ([AgDevCo PR, Aug 2026](https://www.agdevco.com/site/assets/files/2918/press_release_agdevco_ventures_-further_funding_announcement_august_2026.pdf)), as cited by the reviewer. The USD 1.7m mezzanine sits inside that ticket range, but whether Ventures does mezzanine for a greenfield processor is unconfirmed.
- A KES DFI loan at 14% with a TCX hedge is optimistic: the TCX premium alone typically brings hedged KES pricing close to bank rates [PK-UNVERIFIED]. The Phase 2 loan matters only in the bull case, because Phase 2 is a no-go in the round 1 base.

---

## 5. Failure probability (R1-11)

No Kenya- or Africa-specific failure rate for greenfield agro-processors was found. The 30% early-failure probability is the screening report's illustrative figure. Round 1 adds a 10% late-failure probability, conditional on early survival, which brings the total to 37%. It runs sweeps over 0–60% instead of claiming precision.
