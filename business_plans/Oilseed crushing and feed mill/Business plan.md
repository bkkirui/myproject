# Kisumu oilseed crushing and extruded aquafeed mill: business plan

**Prepared:** 19 October 2026. **For:** the investor-founder and prospective DFI or bank credit committees.
**Status:** draft v2.0, revised after independent adversarial review round 1 (`reviews/review_round_1.md`; responses in `reviews/response_round_1.md`). It is not an offering document. Every model figure was checked on 19 October 2026 against a fresh run of `model.py` and its outputs (`model/outputs.md`, the CSVs and the workbook).

**Conventions**
- Every factual claim carries an inline link to its source as cited in the specialist research files in `research/`. Round 1 evidence is in [research/round1_evidence.md](research/round1_evidence.md). Most sources were read only through search-result extracts, because direct page fetches failed. Each therefore needs checking against the primary document before capital is committed.
- **[ESTIMATE]** marks an analyst figure, with its reasoning given or referenced. **[DATED]** marks a source from before 2025. **[CONFLICT]** marks sources that disagree. **[UNVERIFIED]** marks a weak or secondary source.
- Financial figures come from the model (`model/model.py`; outputs in [model/outputs.md](model/outputs.md)). They are nominal KES unless stated, with a value date of 2027. FX starts at KES 129.8/USD and depreciates 4% a year, plus an extra 1.5 points in 2027. **USD conversions state the year whose FX rate is used.**
- **Round 1 changed the answer.** The revision log at the end of the document lists every change.
  - In v1.1 the base equity IRR was 28.9% conditional on survival and 22.3% survival-weighted.
  - In v2.0 it is **15.5% conditional and 8.9% survival-weighted**.
  - The bridge in section 9.8 shows which correction does what.

---

## 1. Executive summary

**What and where.** An integrated plant at peri-urban Kisumu, 60–130 km from the Lake Victoria cage-farming clusters in Siaya and Homa Bay ([technical_operations.md §6](research/technical_operations.md)).
- **Phase 1** (FID Q4 2027, operations from about April 2029): 50 t/day of multi-seed crushing (70% sunflower, 30% non-GM soy), a 15 t/day refinery that fortifies with vitamin A, and a 3 t/h twin-screw line making floating fish feed.
- **Phase 2** (an option tested on 2031 results): crushing rises to 100 t/day with dehulling and solvent extraction, plus a second 3 t/h extrusion line. **The Phase 2 gate fails in the v2.0 base case.**

**The thesis, and what round 1 did to it.**
- The headline story is a crusher selling into a KES 100–130bn edible-oil import gap ([People Daily, Feb 2025](https://peopledaily.digital/business/trade-cs-lee-kinyanjui-pushes-for-local-alternatives-to-slash-ksh100b-edible-oil-imports/amp); [The Standard, 2025](https://thestandard.ke/sports/business/2001515437/edible-oil-processors-rekindle-push-to-scrap-import-duty-tax); [CONFLICT]). The economics are different: the business depends on extruded fish feed and on the refining spread, while the crush margin is thin.
- The v1.1 feed volume rested on a 45 kt merchant market that included the Ugandan and Tanzanian lake shores. **The contestable Kenyan merchant market is about 25 kt in 2026 (range 15–37)**, net of Victory Farms' captive feed and SamakGro's sales to VF-linked farms (section 2.3). At a 15% share, feed sales in 2031 are **5.5 kt**, not 9.9 kt.
- The v1.1 refined-oil price (KES 264k/t) was an unsupported estimate. Landed-parity work puts 20 L bulk refined oil at **KES 240k/t (KES 218/L ex-VAT)**, linked to a crude price of **KES 175k/t**, which is reconciled CPO parity (section 2.1).
- Seed supply, not oil demand, still binds the crusher: Kenya's recorded sunflower output is 6–30 kt a year, against a Phase 1 need of about 13.5 kt ([feedstock_supply.md §1](research/feedstock_supply.md)).

**How much** (base case):

| Item | KES | USD (FX year) |
|---|---|---|
| Phase 1 capex, as spent | 1.40bn | 9.5m (2026 prices; range 6.6–13.8) |
| Phase 1 total uses, 2027–29 | 2.10bn | 14.7m (2028) |
| Phase 1 equity, net of Phase 0 (the incremental FID ask) | 1.53bn | 10.7m (2028) |
| Standby equity for overruns | 0.21bn | 1.5m (2028) |
| Peak net equity, including covenant cure | 1.65bn, reached in 2030 | 10.7m (2030) |
| Senior debt the plant can carry on the lender downside test | **0** | 0 |

**Returns against the hurdles** (base case, KES; [model/outputs.md §6, §9](model/outputs.md)):

| Measure | Base | Hurdle or benchmark | Verdict |
|---|---|---|---|
| Project IRR (KES / USD) | 15.3% / 10.9% | WACC of the modelled structure: **32.3%** (87% equity at 35%) | **Fails:** project NPV at 32.3% is −KES 976m (−635m even at the financing file's 23%) |
| Equity IRR, survival assumed (KES / USD) | 15.5% / 11.1% | Greenfield 35–40% expected; about 48–54% conditional on survival at a 37% total failure risk | **Fails** |
| Equity IRR, survival-weighted (30% early and 10% late failure) | **8.9%** (founder after GM dilution and shareholder tax: 7.6%) | Greenfield 35–40% | **Fails by 26–31 points** |
| Expected founder NPV at 35% / 40% | −KES 1,121m / −1,141m | 0 | Fails |
| Survival-weighted, after-tax founder NPV at the 12.25% tax-free infrastructure bond | **−KES 479m** | 0 | **Fails: the bond is better** |
| Minimum DSCR / covenant cure | 0.92x in 2030 / KES 9m | 1.10x default | Breach in the ramp year |
| Equity IRR without exit value | 4.7% | – | The exit carries the return |

**Key risks, in rank order:**
1. Feed market size, share and price, in a regional aquafeed market that is over-supplied: Tunga 45 kt, SamakGro 8 t/h, De Heus 50–100 kt. Victory Farms is about half of Kenyan cage output and makes about 90% of its own feed.
2. Delivered seed cost: equity IRR runs from 26.0% to −8.8% across the research range.
3. The refined-oil price and its spread over crude.
4. Capex overrun.
5. Policy: the CPO duty was struck down in November 2025, the GMO import ruling is pending, duty waivers recur, and the minimum tax could return.
6. Execution by a founder without sector operating experience.
7. Social licence for cage farming on Lake Victoria (a Senate inquiry opened in October 2026).
8. The election on 10 August 2027.

**Recommendation.**
- **Do not build, and do not fund Phase 0 as designed.** The v1.1 plan asked for USD 0.8m now. The value-of-information analysis (section 12.6) shows that even its cheap first stage (Phase 0a, USD 0.3m) has negative expected value against stopping:
  - With independent priors, none of 150 simulated states of the world passes the proceed test.
  - With priors in which favourable outcomes cluster (correlation 0.5), only 2–3% pass. The gross value of perfect information is then at most KES 12m (about USD 0.09m at 2027 FX), against KES 41m for Phase 0a.
- **The kill thresholds now sit at or just beyond the base values** (section 12.2). If any one of feed market size, feed price, share, seed cost or capex turns out at its base value or worse, the plant fails the hurdle even with every other driver at its favourable (bull) value.
- **The restructure alternatives do not rescue it.** Feed-mill-first returns 9.6% (conditional equity IRR) and crusher-only 1.5% (section 9.5).
- **Options for the founder:**
  - **Preferred:** redeploy the capital to the higher-ranked opportunities in the screening report, or to tax-free infrastructure bonds, which beat this plan's survival-weighted after-tax return.
  - **If the founder holds a strong prior that the market is much larger than the evidence suggests:** spend at most **USD 50k** on a desk-and-telephone check, with a hard stop at the end (section 12.5). It would test the three facts that alone could reopen the case:
    1. Victory Farms' Kenyan output and the non-VF merchant feed market, from county fisheries offices and distributors.
    2. 20 L oil and feed distributor quotes in Kisumu.
    3. Two budget capex quotes.
  - **The only structure worth re-examining** is buying an under-used existing feed mill, which is unmodelled and needs its own evidence (section 12.7).
- **What would have to be true to build.** Roughly all of the following together (Case B plus regional demand, or the bull case; section 9.6):
  - a contestable Kenyan market of at least 32 kt;
  - a 20% share;
  - feed prices 10% above base;
  - seed 10% cheaper;
  - capex 15% lower;
  - refined oil at KES 250k/t;
  - Ugandan and Tanzanian access;
  - a failure probability cut to 20%.

  The modelled probability of that combination is under 5% even on generous priors.

**If the case is ever reopened, the gates stand as recalibrated in section 12:**
- **G0 (FID):** the calibrated kill thresholds, a debt-capacity test (senior debt of at least KES 300m sized on the lender downside case, with no cure needed in the base), and a survival-weighted founder IRR of at least 35% at a defensible failure probability.
- **G1 (Phase 2):** contracted seed, at least 9 kt of 2031 feed sales at a gross margin of at least 30%, and a positive incremental equity NPV at 35%.

---

## 2. Market opportunity

### 2.1 Edible oil

**Size and import dependence.**
- Palm oil is more than 90% of Kenyan oil and fat consumption. USDA puts palm imports at 875 kt in 2024, heading for 1.05 Mt in 2025/26, of which 90–100 kt is re-exported ([OFI Magazine](https://www.ofimagazine.com/news/kenyan-palm-oil-consumption-to-reach-record-high); [Milling MEA/USDA, Jul 2025](https://millingmea.com/kenyas-palm-oil-imports-to-hit-1-05-million-tonnes-in-2025-2026-usda/)).
- AFA's quarterly data show 183,139 t of edible oils worth KES 25.6bn imported in the quarter to June 2025, including only 3,909 t of sunflower and 1,671 t of soy oil ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)).
- **[CONFLICT] Volume.** AFA and the Ministry say about 600 kt is consumed ([The Star, Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)), while USDA palm imports alone are about 1 Mt. The research base for food-grade oils and fats is **about 780 kt in 2026** [ESTIMATE, [market_demand.md §1.1](research/market_demand.md)].
- **[CONFLICT] The import bill.** Figures of KES 100bn ([People Daily](https://peopledaily.digital/business/trade-cs-lee-kinyanjui-pushes-for-local-alternatives-to-slash-ksh100b-edible-oil-imports/amp)), KES 130bn for CPO ([The Standard](https://thestandard.ke/sports/business/2001515437/edible-oil-processors-rekindle-push-to-scrap-import-duty-tax)) and KES 145bn ([The Star](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)) are all cited. The research base is KES 120–135bn in 2026 [ESTIMATE].
- **Local oil from local seed is under 5% of consumption** [ESTIMATE, [market_demand.md §1.1](research/market_demand.md)]. Bidco needs more than 10 kt a year of local seed but gets about 5 kt ([KNA](https://www.kenyanews.go.ke/?p=23808), date uncertain).
- **Policy push.** In March 2026 the government relaunched a sunflower and soy drive aimed at halving imports between 2026 and 2030 ([KNA, Aug 2026](https://www.kenyanews.go.ke/sunflower-soybean-initiative-to-curb-edible-oil-import-bill/)). The 50%-local target is not credible [ESTIMATE, [feedstock_supply.md §5](research/feedstock_supply.md)].

**Prices (Sep–Oct 2026).**
- Retail salad oil averaged KES 358.09/L in July 2026, close to the September 2022 peak of KES 379.84 ([Business Daily](https://www.businessdailyafrica.com/bd/economy/cooking-oil-prices-climb-back-to-highs-of-2022-crisis-5548020)).
- KNTC's state-linked "Mama Pima" loose oil sells at KES 185/L wholesale and KES 210/L retail ([Kenya Times, Jul 2026](https://thekenyatimes.com/business/govt-unveils-mama-pima-cooking-oil-dispenser/)). That is about the price of duty-free imported olein, a policy-driven tail.
- RBD olein USD 1,252.5/t FOB, 8 September 2026 ([Fastmarkets](https://www.fastmarkets.com/insights/correction-to-price-for-refined-bleached-deodorized-palm-olein-on-september-8-2026/)). Malaysian CPO reference USD 1,091/t for October ([Bernama](https://www.bernama.com/en/news.php?id=2604287)). Crude sunflower oil USD 1,265–1,275/t FOB Black Sea ([Commodity-Board](https://commodity-board.com/russia-takes-the-wheel-in-sunflower-oil-what-it-means-for-prices), [UNVERIFIED aggregator]).

**[CONFLICT] resolved: CPO parity** ([round1_evidence.md §2.1](research/round1_evidence.md)).
- The two research files disagreed. The feedstock file put CPO landed at KES 150–166/kg and called it the ceiling on local crude value ([feedstock_supply.md §2.4](research/feedstock_supply.md)). The market file put it at KES 185k/t and set local crude at 190k ([market_demand.md rows 5, 8](research/market_demand.md)).
- The feedstock file used the Indonesian reference price and omitted the IDF/RDL levies and port costs. The market file's FOB was slightly high.
- **Reconciled:** FOB about USD 1,100, giving **KES 177k/t landed**. Refiners can switch to CPO, so **local crude is now modelled at the lower parity, KES 175k/t** (v1.1: 190k).

**Refined 20 L bulk oil: landed parity** ([round1_evidence.md §2.2](research/round1_evidence.md); ex-VAT, delivered Kisumu, [ESTIMATE]):

| Benchmark | KES k/t | KES/L |
|---|---|---|
| Imported RBD olein at "25% or USD 500/t, whichever is higher" (the specific duty binds) | 269 | 245 |
| Imported RBD olein at a 35% ad valorem CET | 264 | 240 |
| Imported RBD olein at a 25% ad valorem CET (the reviewer's case) | 246 | 224 |
| Local refiner working from CPO, cost-plus | ~219 | ~199 |
| 2022 jerrican (KES 5,100 per 20 L) at retail prices similar to today ([People Daily](https://peopledaily.digital/news/makers-warn-cooking-oil-prices-to-rise), [DATED]) | ~242 | ~220 |
| RBD olein imported duty-free (KNTC-type) or misdeclared as crude | 202–221 | 184–201 |
| **Model base: crude 175k + refining spread 65k** | **240** | **218** |

- **[CONFLICT] on the refined-oil duty.**
  - EY lists a 35% CET on RBD olein ([EY, 2023](https://globaltaxnews.ey.com/news/2023-1308), [DATED]).
  - Kenya has applied "25% or USD 500/t, whichever is higher" under an EAC stay. Kenyan manufacturers described that stay as continuing in 2026 ([MPOB, Apr 2026](https://prestasisawit.mpob.gov.my/en/palmnews/news/35498), [UNVERIFIED extract]).
  - An EAC Gazette notice of 2025 lowered some refined-oil rates for Kenya without a rate being found ([FNJ](https://fnjassociates.co.ke/a-guide-to-customs-import-duty-in-kenya/)).
  - The current KRA tariff line is a Phase 0a and due-diligence item.
- **No sunflower premium is assumed.** CIF unit values show sunflower 13% above palm at import ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)). No consumer or institutional premium for 20 L sunflower oil was evidenced.
- **The refined price is now linked to crude** through the refining spread (range 40–90k, so refined 215–265k at base crude). Crude, refined oil and the parity-linked seed price therefore move together. v1.1 had independent inputs, so lowering crude alone raised returns.
- **No 2026 quote for a 20 L jerrican was found.** Wholesale and institutional quotes in Kisumu are a Phase 0a item, and the refined price is now a kill test (K11).
- **Refining margin.** The COMESA Competition Commission alleged that refiners sold at KES 333/L against a "fair" KES 274/L ([Khusoko, Dec 2024](https://khusoko.com/2024/12/11/oil-firms-overcharged-kenyans-by-ksh-67-7-billion/), [DATED]). That margin is in the branded 1 L retail layer, which this plan does not enter.

### 2.2 Protein meal and compound feed

- **Formal compound feed** is about 2.5 Mt a year: poultry 60%, dairy 29% ([KNA](https://www.kenyanews.go.ke/?p=169703), date unconfirmed). Millers ran at 50–60% of capacity in July 2026 ([The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)). AKEFEMA warned of shortages of soybean meal, sunflower cake and canola in February 2026 ([The Star](https://www.the-star.co.ke/counties/central/2026-02-24-raw-material-crunch-threatens-to-push-animal-feed-cost-higher)).
- **Protein is the scarce input, not pelleting capacity** [ESTIMATE, [market_demand.md §3.1](research/market_demand.md)].
- **GMO status.** A Court of Appeal conservatory order (7 March 2025) bars GM imports pending appeal ([Citizen Digital](https://citizen.digital/article/blow-to-govt-as-court-of-appeal-bars-importation-of-gmos-n358801)). Judgment was expected on 24 April 2026 ([KNA](https://www.kenyanews.go.ke/?p=159340)). No reported outcome was found, so check Kenya Law before any commitment.
- **Protein prices modelled (2026 KES/t).** These are the weakest-sourced prices in the plan:

| Input | Modelled price | Basis |
|---|---|---|
| Sunflower cake | 40k | One [UNVERIFIED] Nairobi listing ([Jiji](https://jiji.co.ke/viwandani-makadara/feeds-supplements-seeds/sunflower-seed-cake-dTh5NuF0GdsvaWJ01XlkOR3T.html)) |
| Non-GM soybean meal | 95k | Indexbox KES 90–120k/t, [UNVERIFIED] ([Indexbox](https://www.indexbox.io/store/kenya-soya-beans-market-analysis-forecast-size-trends-and-insights/)) |
| Own soy expeller cake | 85k | [ESTIMATE] |

### 2.3 Aquaculture and the contestable aquafeed market

**Growth.**
- Cage tilapia output rose from 13,700 t in 2021 to **28,100 t in 2025** (KNBS via [Ecofin](https://www.ecofinagency.com/news-agriculture/1703-53851-kenya-s-fish-farming-boom-draws-new-bet-from-victory-farms)), a 19.7% compound annual growth rate.
- KMFRI puts riparian cage capacity at about 275,000 t a year ([WAS 2025](https://www.was.org/Meeting/Program/PaperDetail/166835)).

**Victory Farms reconciled with KNBS** ([round1_evidence.md §1.1](research/round1_evidence.md)).
- The Victory group produces about 25 kt a year company-wide and targets 100 kt by 2030 ([KNA](https://www.kenyanews.go.ke/168926-2/)).
- Victory Farms runs at more than 1,400 t a month ([The Star, Jul 2026](https://www.the-star.co.ke/counties/nyanza/2026-07-03-victory-farms-bets-on-tech-and-talent-to-boost-fish-production)). Its Rwandan arm, Kivu Choice, runs at about 800 t a month ([New Times, 2026](https://www.newtimes.co.rw/article/36743/National/cepgel-governors-meet-in-gisenyi/amp)).
- Reading The Star's figure as Kenya-only reconciles the group total. On that reading, Victory Farms' Kenyan output was about 13–16 kt in 2025, or **about 45–60% of KNBS cage output**. It makes about 90% of its feed in-house ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840)).
- [CONFLICT/UNVERIFIED]: a KNA extract describes the 1,400 t a month as group sales. If so, Victory Farms' Kenyan share is smaller and the merchant market larger. This is the high case.

**Contestable Kenyan merchant SAM, 2026** ([round1_evidence.md §1.2](research/round1_evidence.md), [ESTIMATE]):

| | Low | Base | High |
|---|---|---|---|
| Non-VF cage output (kt) | 12 | 16 | 20 |
| × FCR | 1.5 | 1.6 | 1.8 |
| × share not tied to SamakGro or VF-linked supply | 75% | 85% | 90% |
| + pond and hatchery extruded feed (kt) | 1.5 | 3 | 5 |
| **Contestable merchant SAM (kt)** | **15** | **25** | **37** |

- **Uganda and Tanzania are upside only (0 kt in the base, +12 kt in a scenario).** De Heus Njeru (50–100 kt) and Tunga Uganda sit inside those markets ([market_demand.md §1.5, §3.3](research/market_demand.md)). Tanzania's entire commercial fish-feed use was 6.2 kt in 2023 ([UNCST](https://nru.uncst.go.ug/bitstreams/4670621e-4062-4039-9bc1-f274e4da36df/download), [DATED]).
- The SAM grows 8% a year (4–14%). Most of the 19.7% cage growth is Victory Farms, which is captive.

**Competitor response.**
- Tunga Nutrition doubled its extrusion capacity to 45 kt a year around February 2026 ([WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi)).
- SamakGro's 8 t/h geothermal plant aims to make feed more affordable, with no commissioning date disclosed ([Capital FM, 2026](https://capitalfm.africa/fish-feed-firms-to-invest-sh510mn-at-kengens-olkaria-park/)).
- No 2026 price cut was found ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back)).
- **The base now has feed prices falling 1% a year in real terms from 2029.** A competitor-response scenario has 3% a year plus a 10% entrant discount [ESTIMATE].

**Feed prices.**
- SamakGro's retail list: 4 mm finisher KES 116–130/kg; 3 mm grower KES 144/kg ([SamakGro store](https://take.app/samakgro/p/clzr0xsj9004nirjw3brif1fa), undated).
- **Modelled (2026 KES):** grow-out KES 125/kg and starter KES 200/kg [ESTIMATE], less a 5% dealer margin. Net of the 1% a year real decline, grow-out realises about KES 118/kg in 2031 (2026 KES).

### 2.4 Market sizing (TAM / SAM / SOM)

| Level | Edible oil | Aquafeed | Source |
|---|---|---|---|
| TAM | About 780 kt; about KES 156bn at wholesale | Kenyan aquafeed 50–80 kt (all buyers) | [market_demand.md §5](research/market_demand.md) [ESTIMATE] |
| SAM | Soft oils a Kenyan crusher can displace: 60–100 kt | **Contestable Kenyan merchant extruded feed: 25 kt in 2026 (15–37), about 37 kt by 2031**; Uganda/Tanzania upside only | §2.3 [ESTIMATE] |
| **Plant (model)** | **2.5 kt refined plus 0.7 kt crude oil in 2031** (under 0.5% of consumption) | **5.5 kt of feed in 2031 and 9.4 kt in 2038** (15% of the contestable SAM) | [model/outputs.md §4](model/outputs.md) |

**What the plant can and cannot do.**
- It matters to neither national total. The "KES 100bn gap" is real but is not the investment case.
- In feed, 15% of the contestable Kenyan market is 5.5 kt in 2031. That leaves the 3 t/h extruder (11.5 kt a year effective) at under 50% use in 2031. Reaching v1.1's 9.9 kt would need a 27% share of a market where Tunga, SamakGro, the Victory Farms Doho mill and Aller Aqua imports already compete.

### 2.5 Customer segments

| Segment | Product | Volume, 2031 (model) | Buying behaviour |
|---|---|---|---|
| Mid-size and smallholder cage farms in Siaya, Homa Bay, Busia and Migori; pond farmers | Extruded grow-out feed (3–6 mm) | 4.7 kt | Price- and FCR-sensitive; credit-constrained; buy through depots and dealers, e.g. AquaRech-type depots ([Aller Aqua](https://www.aller-aqua.com/about/news/aller-aqua-partners-with-aquarech-to-ensure-high-quality-quality-feeds-reach-all/)) |
| Hatcheries and fingerling producers | Starter and fry feed (0.3–2 mm, 35–45% CP) | 0.8 kt | Value quality and pellet size; currently import-dependent |
| Institutions, wholesalers, hotels and schools in western Kenya | Refined fortified oil, 20 L | 2.5 kt | Price-matched to 20 L palm olein delivered in Kisumu (KES 240k/t base); no premium assumed |
| Refiners (Bidco, Menengai, Kapa, Pwani) | Crude oil | 0.7 kt | Oligopsony; local crude at about CPO parity |
| Dairy and layer feed millers in the Rift and Central belt | Sunflower and surplus soy cake | 6.5 kt | Commodity buyers; prices swing with regional export bans and duty waivers |

---

## 3. Competitive landscape and positioning

### 3.1 Named competitors

**Aquafeed.** Regional capacity is several times the contestable Kenyan merchant demand of about 25 kt ([market_demand.md §3.3](research/market_demand.md)).

| Competitor | Facts | Threat |
|---|---|---|
| **Tunga Nutrition** (Skretting/Nutreco and Unga JV; brands Skretting and Fugo), Nairobi | Extrusion capacity raised from 24 kt to **45 kt a year**, about February 2026 ([WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi)) | High: multinational formulation and brand |
| **SamakGro** (Victory Farms, Maxim Agri, Gatsby Africa), Naivasha | Sells to third parties. A new USD 3.95m, 8 t/h geothermal plant was announced in July 2026 ([The Fish Site](https://thefishsite.com/es/articles/african-aquaculture-leaders-join-forces-to-build-feed-mill-maxim-agri-victory-farms-gatsby-africa); [ThinkGeoEnergy](https://www.thinkgeoenergy.com/fish-feed-producer-invests-in-geothermal-powered-green-energy-park-in-kenya/?amp=1)) | High: low-cost power; owner of the largest cage farm |
| **Victory Farms Doho mill**, Homa Bay | KES 1.3bn extruded feed mill ([The Standard](https://www.standardmedia.co.ke/business/nyanza/article/2001549421/new-bid-to-improve-fish-production-in-homa-bay)); capacity undisclosed | High if it sells surplus feed in the plant's home market |
| **De Heus Uganda**, Njeru | 50 kt rising to "up to 100 kt"; USD 25m; opened about 2025 ([De Heus](https://www.deheus.com/csr-stories/how-a-de-heus-plant-can-support-fish-farming-in-uganda-and-help-feed-the-nation); [Ecofin](https://www.ecofinagency.com/news-industry/0509-48437-de-heus-invests-25-million-in-ugandan-fish-feed-industry); [CONFLICT on capacity]) | Medium-high: blocks feed exports to Uganda |
| **Aller Aqua** imports via AquaRech | Depots in Kakamega, Kisii, Migori, Bondo, Homa Bay, Siaya, Busia and elsewhere ([Aller Aqua](https://www.aller-aqua.com/about/news/aller-aqua-partners-with-aquarech-to-ensure-high-quality-quality-feeds-reach-all/)) | Medium |
| Unga Farm Care (Fugo), Sigma Feeds, Jewlet; a reported DiscoverAqua plant at Athi River (Q3 2026, [UNVERIFIED]) | Fugo launched in Homa Bay ([Aquafeed.com](https://aquafeed.com/newsroom/news/kenya-unga-farm-care-launches-fish-feed-to-improve-tilapia-business-in-homa-bay)); Sigma has made fish feed since 2010 ([Milling MEA](https://millingmea.com/sigma-feeds/)) | Low-medium |
| Kisumu Fisheries Centre of Excellence (public) | USD 19.3m, includes a feed mill ([Food Business MEA](https://www.foodbusinessmea.com/?p=2133722), date unclear) | Unknown: competitor or toll partner |

**Edible oil and crushing.**
- Bidco, Pwani, Kapa, Menengai and Edible Oil Products dominate refining, mostly of imported CPO ([market_demand.md §1.3](research/market_demand.md)).
- Agventure / Pure Mountain crushes just under 10 kt a year of canola ([CPM, Mar 2026](https://www.cpm-magazine.co.uk/wp-content/uploads/sites/9/2026/03/066-68-Kenya-March-26.pdf)).
- Regional seed competitors include Mukwano in Uganda (more than 100,000 contracted farmers; [Uganda Invest](https://ugandainvest.go.ug/?p=579)) and Mainland Group in Dodoma ([Milling MEA](https://millingmea.com/chinese-agribusiness-giant-mainland-group-to-launch-new-sunflower-oil-plant-in-tanzania/)).

### 3.2 Why this plant could win, and how strong each advantage is

| Source of advantage | Mechanism | Strength |
|---|---|---|
| Secure non-GM protein | Own soy cake covers the feed line's soy need (1.8 kt in 2031, mass-balance CSV). This de-links the plant from GMO, waiver and export-ban shocks ([feedstock_supply.md §2.3](research/feedstock_supply.md)) | **Moderate.** Own cake is transferred at market prices, so the base IRR contains no integration cost saving |
| Proximity | 60–130 km to the cage clusters, against about 345 km from Nairobi. Saves about KES 2,200/t (about 2% of price) [ESTIMATE, [feedstock_supply.md §0](research/feedstock_supply.md)] | **Weak to moderate.** Victory Farms' Doho mill is closer still |
| Twin-screw fry and fingerling feeds | Small pellets and high-fibre recipes ([technical_operations.md §3.1](research/technical_operations.md)) | Moderate, but replicable |
| Farmer bundle | Cake buy-back or a feed discount for seed outgrowers ([feedstock_supply.md §4.2](research/feedstock_supply.md)) | Moderate; builds seed loyalty, not feed share |
| EAC-origin oil | Oil from EAC seed should trade duty-free within the EAC ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/bidco-pushes-for-review-of-25pc-duty-rule-for-eac-exports-2120464), [DATED]) | Upside only; unverified |
| Outgrower network | Agventure took more than 10 years to reach about 10 kt | The most durable moat, if achieved; also the hardest task |

**Judgement.** The plant would enter as a regional challenger against better-capitalised multinationals and a vertically integrated market leader, with **no strong moat in feed**. Competitors are assumed to respond on price: the base has a 1% a year real decline, and a 3% a year decline gives an equity IRR of 5.2% (section 9.5).

---

## 4. Products and business model

### 4.1 Product mix and pricing (model base)

| Product | 2031 volume | 2031 revenue (KES m) | 2038 revenue (KES m) | Price basis, 2026 KES ex-VAT |
|---|---|---|---|---|
| Extruded grow-out feed (28–32% CP) | 4.7 kt | 752 | 1,816 | KES 125/kg list, less 1% a year real decline from 2029; 5% dealer margin; 5% entrant discount in operating years 1–2 |
| Starter and fingerling feed (35–45% CP) | 0.8 kt | 214 | 516 | KES 200/kg [ESTIMATE], same decline |
| Refined fortified oil (20 L) | 2.5 kt | 786 | 1,155 | Crude + KES 65k spread = KES 240k/t; 5% distribution cost |
| Crude oil to refiners | 0.7 kt | 148 | 217 | KES 175k/t (CPO parity) |
| Sunflower cake | 5.0 kt | 241 | 312 | KES 40k/t |
| Surplus soy cake | 1.5 kt | 152 | 30 | KES 85k/t |
| Soapstock and acid oil | 0.1 kt | 9 | 13 | 30% of crude value |
| **Total** | | **2,301** | **4,059** | Tradables escalate with the USD-drift × FX index; oil carries 60% of a KES 15k/t CPO-duty haircut |

Source: `model/pnl_annual.csv`.
- **Revenue mix:** feed is 42% of revenue in 2031 (v1.1: 60%) and 57% in 2038.
- **Gross margin mix:** feed is about 53% of combined crush and feed gross margin in 2031, with the refining margin excluded [calculation from the model].

### 4.2 Price linkages: how risk is shared

- **Oil.** Crude is the oil price index. Refined oil equals crude plus a refining spread, and seed absorbs 50% of changes in oil-plus-cake value, through the floating, parity-linked contract in [feedstock_supply.md §4.2](research/feedstock_supply.md). With fixed-price seed, the oil-price swing runs 6.4% to 17.2% equity IRR (tornado).
- **Feed.** Feed prices absorb 70% of changes in competitors' ingredient costs and fall 1% a year in real terms [ESTIMATE]. Tunga and SamakGro set the market price.

### 4.3 Channel strategy

- **Feed.** Half direct to mid-size cage farms and half through dealers at about 10% margin (blended to 5%). Sales force and extension cost 3% of feed revenue; credit terms are 21 days. Victory Farms is **not** a target customer.
- **Refined oil.** Bulk 20 L containers to institutions, wholesalers and hotels in western Kenya, priced against palm olein. Branded 1 L retail is not entered. Public-sector sales are capped at 10% of revenue: pending bills stood at KES 466bn in March 2026 ([Capital FM](https://capitalfm.co.ke/news/2026/06/kenya-pending-bills-sh465-87-billion-cob-march-2026)).
- **Crude oil and cake.** Monthly parity-linked pre-sales to refiners and Rift and Central feed millers ([financing_capital.md §7](research/financing_capital.md)).

### 4.4 Offtake agreements: required before FID

No offtake agreement exists. If the case is reopened, FID would require:
- signed LOIs for at least 50% of crude oil or cake, and at least 8–10 kt a year of seed ([financing_capital.md §6](research/financing_capital.md));
- **LOIs from at least five non-Victory cage farms for at least 3 kt a year of grow-out feed**, at a net realisation of at least KES 124/kg list-equivalent (the calibrated K2 threshold);
- **a 20 L institutional or wholesale price of at least KES 212k/t** (KES 193/L ex-VAT; K11).

---

## 5. Feedstock strategy

### 5.1 The binding constraint

**Kenyan supply is small and poorly measured** [CONFLICT]:

| Crop | Estimates | Source |
|---|---|---|
| Sunflower | 3.6 kt (Economic Survey), 6 kt (FAOSTAT), about 9.5 kt for Nakuru alone | [KIPPRA](https://kippra.or.ke/leveraging-on-the-sunflower-value-chain-for-job-creation-in-kenya/); [Selina Wamucii](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds); [KNA](https://www.kenyanews.go.ke/?p=179463) |
| Soy | 2 kt or 17 kt | [Nation](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966) |

- The research's working range for national sunflower output is **10–30 kt a year** [ESTIMATE, [feedstock_supply.md §1.2](research/feedstock_supply.md)].
- A crusher above about 20 kt a year is not supportable before year 5 ([feedstock_supply.md §9](research/feedstock_supply.md)). Seed is drawn from three countries (section 5.2).

**The model's supply path** is the potential available seed: 8, 11, 14, 17 and 20 kt in 2029–33, rising to 32 kt in 2038. Actual crush is capped at 90% of nameplate:

| | 2029 | 2030 | 2031 | 2032 | 2033 | 2034 | 2035 | 2036–38 |
|---|---|---|---|---|---|---|---|---|
| Seed crushed, base (Phase 1 only; kt) | 6.0 | 11.0 | 13.5 | 13.5 | 13.5 | 13.5 | 13.5 | 13.5 |
| Seed crushed if Phase 2 were built (kt) | 6.0 | 11.0 | 13.5 | 13.5 | 20.0 | 23.0 | 26.0 | 27.0 |

The research puts the probability that year-1 throughput falls below 60% of plan at about 40% [ESTIMATE, [feedstock_supply.md §10](research/feedstock_supply.md)].

### 5.2 Sourcing mix and delivered cost

The mix is shown for a reference 20 kt plant ([feedstock_supply.md §8–9](research/feedstock_supply.md); all [ESTIMATE]).

| Source | Year 1 share | Year 5 share | Delivered base, KES/t | Notes |
|---|---|---|---|---|
| Kenyan contracted outgrowers (West/Nyanza, Rift) | 10% | 45% | 62,300 | Hybrid seed; floating price; weigh-and-pay |
| Kenyan spot via aggregators and co-ops | 20% | 15% | 55,500 | |
| Uganda sunflower and soy (licensed aggregators in Lira, Soroti, Tororo) | 35% | 25% | 47,000 | EAC duty-free; about 450 km; competes with Mukwano |
| Tanzania sunflower (swing) | 30% | 5% | 50,000 | Capped at 25% or less; worst quality; 10% export levy proposed |
| Canola and specialty soy | 5% | 10% | about 70,000 | Opportunistic |
| **Blended sunflower** | **52,300** | **57,600** | | Model path, 2026 KES |
| Soybean (Kenya/Uganda) | | | 75,000 | Homa Bay farmgate about KES 70/kg ([The Standard, Jul 2026](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)) |

**Price anchors.**
- Kenyan farmgate sunflower is about KES 47/kg ([Selina Wamucii, Jun 2026](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds), [UNVERIFIED]).
- Tanzanian farmgate is TZS 497 ([Selina TZ](https://www.selinawamucii.com/insights/prices/tanzania/sunflower-seeds/)).
- Ugandan export unit value is USD 0.17/kg ([Selina UG](https://www.selinawamucii.com/insights/prices/uganda/sunflower-seeds/)).
- Black Sea seed landed in Kisumu would cost about KES 105–115/kg, about twice local. **That is not a viable fallback** ([commodity-board](https://commodity-board.com/sunflower-seeds-under-pressure-while-oil-finds-support-in-tight-black-sea-flows); [ESTIMATE]).

**Flow direction.** Kenyan seed currently flows *into* Tanzania at Loitokitok, because Tanzanian buyers pay more ([Nation, mid-2026](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502)). Tanzania's 2026/27 budget proposes a 10% export levy on sunflower seed ([Milling MEA, Jun 2026](https://millingmea.com/tanzania-targets-edible-oil-self-sufficiency-with-tax-relief-and-import-controls/)); the model weights it at a 70% probability.

### 5.3 Outgrower model

The design follows the evidence in [feedstock_supply.md §4](research/feedstock_supply.md):
1. **A floating price**, set as a floor plus a share of oil and cake parity and announced before planting.
2. **Cake buy-back or a feed discount** for growers.
3. **Lead-farmer and co-op aggregation**, with weigh-and-pay by mobile money.
4. **Seed-only input credit.** Credit is recovered at delivery, using a tripartite bank model on the Bidco and Equity Bank precedent ([Business Daily](https://www.businessdailyafrica.com/bd/news/counties/bidco-set-to-buy-sh120m-sunflower-seeds-from-farmers-in-meru-2301152), [DATED]).
5. **Geographic diversification** across bimodal and unimodal zones.
6. **Ride on county, AFA and LBDA seed distribution** rather than duplicating it ([Milling MEA, LBDA Kisumu](https://millingmea.com/lbda-expands-sunflower-farming-drive-to-boost-farmer-incomes-in-kisumu/)).

**Scale required [ESTIMATE].** At 0.9 t/ha delivered and 30% side-selling, the 2031 outgrower share (30% of 9.45 kt of sunflower) needs about 4,500 ha, or 4,500–9,000 smallholders. With Phase 2 (50% of 18.9 kt by 2036) it would need about 15,000 ha, or 15,000–30,000 smallholders.

**Partner.** Farm Africa's soy aggregation centres in Homa Bay serve about 6,000 farmers ([The Standard, Jul 2026](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)). They are a ready partner.

**Evidence gap.** No quantified side-selling rate exists for East African oilseeds. The model uses 15/30/50% for low/base/high [ESTIMATE]. If the case is ever reopened, the right-sized Phase 0b pilot (section 12.5) would measure it against a named buyer.

### 5.4 Seasonality and working capital

- About 70% of seed is bought June to October. Lean-season prices are 50–90% higher ([feedstock_supply.md §7](research/feedstock_supply.md); Homa Bay middleman spread in [Nation 2026](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966)).
- The model's safety stock (1.5 months) was **calibrated by the modeller** so that peak stock is about 41% of annual crush (8.2 kt per 20 kt). That sits inside the research's 7–12 kt range.
- Year-end working capital is KES 593m in 2031. Peak intra-year revolver draws are KES 353m in Phase 1 and KES 523m (nominal) by 2038 ([model/outputs.md §3](model/outputs.md)).
- The steady-state seasonal peak checks against the research: KES 754m per 20 kt (2026 KES), within its KES 650–950m range ([model/outputs.md §12](model/outputs.md)).

### 5.5 Quality and aflatoxin control

- **Standard.** Finished tilapia feed must meet total aflatoxin of 10 ppb or less and AFB1 of 5 ppb or less under KS 2289-1:2016 ([WTO TBT notification](https://members.wto.org/crnattachments/2016/TBT/KEN/16_4795_00_e.pdf), [DATED but current]).
- **Why it matters.** Small Tanzanian expeller cake measured 1.4–598 ng/g ([PLOS One](https://pmc.ncbi.nlm.nih.gov/articles/PMC5395219)). KEBS found only 1 of 17 sampled feed brands fully compliant ([Milling MEA](https://millingmea.com/kenya-bureau-of-standards-warns-of-non-compliant-animal-feeds-amid-increasing-production-costs/), date unclear).
- **Controls [ESTIMATE, industry norms]:**
  - Intake moisture of 9% or less (sunflower) and 12% or less (soy).
  - Lateral-flow aflatoxin test on every lot, with monthly HPLC confirmation at an accredited laboratory.
  - NIR seed analysis and an oil-content price grid. Seven points of oil yield is worth about KES 12k per tonne of seed ([feedstock_supply.md §3](research/feedstock_supply.md)).
  - Dehulling in Phase 2.
  - Toxin binder in premix.
  - Non-compliant lots diverted to dairy or poultry cake sales.
  - **No groundnut.**
  - Strip tests on soy for GM content, with identity-preservation records ([regulatory_tax_risk.md §4.3](research/regulatory_tax_risk.md)).

---

## 6. Site, technology and operations

### 6.1 Site

**Choice.** Peri-urban Kisumu: the Kisumu–Busia road, Kibos/Mamboleo, or near the port. Seed buying and pre-cleaning depots at Busia and Bungoma, and a feed depot at Homa Bay or Bondo.
- Kisumu scored 3.95 on the weighted site matrix, ahead of Bungoma/Eldoret (3.80), Nakuru/Naivasha SEZ (3.55) and Busia (3.50) [ESTIMATE, [technical_operations.md §6](research/technical_operations.md)].
- The plant should sit **inland, 10–30 km from the shoreline**. A shoreline site would add riparian review and exposure to the Senate inquiry ([regulatory_tax_risk.md §3.2](research/regulatory_tax_risk.md)).

**Land.** Hold land in a wholly Kenyan-owned PropCo that leases to the OpCo for 33–49 years. Under Article 65, non-citizens hold land only on leases of up to 99 years ([Rödl](https://roedl.com/insights/foreign-ownership-land-kenya)), and a DFI or foreign co-investor would make the OpCo non-citizen ([regulatory_tax_risk.md §5](research/regulatory_tax_risk.md)).

### 6.2 Configuration and capacities

| Unit | Phase 1 (2029) | Phase 2 (from 2033) | Technology |
|---|---|---|---|
| Crushing | 50 t/day (15 kt/yr nameplate; 90% maximum use) | 100 t/day (30 kt/yr) | P1: hot full-press expellers plus a soy extruder-expeller. P2: dehulling, prepress and hexane solvent extraction |
| Refinery | 15 t/day crude in | +20 t/day | Semi-continuous chemical refining with winterisation and vitamin A dosing; 20 L filling |
| Extrusion | 3 t/h twin-screw (about 11.5 kt/yr effective) | +3 t/h (about 23 kt/yr total) | Famsun/Muyang-class; fine grinding, preconditioner, belt dryer, coater |
| Seed storage | 5 kt silos plus leased overflow | +7.5 kt | Galvanised silos with aeration |
| Utilities | 3–4 t/h biomass boiler, 1.6 MVA transformer, about 1 MVA standby genset, ETP, borehole | Hull-fired boiler extension | Standby power is a process requirement: an extruder trip blocks the die |

**Design choices.**
- The **refinery** is 15 t/day rather than the 20 t/day in the technical file, because 30% of the seed is soy, which yields only 12% oil.
- **Phase 2 is smaller** than the technical file's 150 t/day and +6 t/h. Neither the seed path nor feed demand can fill the larger plant. Forced through at that specification, equity IRR falls to 6.3%, with KES 889m of covenant cures ([model/outputs.md §7](model/outputs.md)).
- **The 3 t/h extruder is oversized for the v2.0 market:** it runs at 48% of effective capacity in 2031 and 82% in 2038. A 2 t/h line would save part of the USD 1.9m extrusion package. It is not modelled, because the verdict does not turn on it.
- **No solvent extraction in Phase 1.** At 50 t/day the solvent gain of about USD 0.95m a year does not justify about USD 3m of plant plus hexane-safety risk for a first-time operator ([technical_operations.md §1.2](research/technical_operations.md)). The minimum efficient scale is above 75–200 t/day ([Missouri EM0602](https://extension.missouri.edu/media/wysiwyg/Extensiondata/Pub/pdf/energymgmt/em0602.pdf), [DATED]; [AMPC](https://www.ampc.montana.edu/documents/briefings/briefing86.pdf), [DATED]).

### 6.3 Mass balance, 2031 (Phase 1 steady state; model)

```
Seed crushed 13,500 t  = sunflower 9,450 t (full press, 31% oil) + soy 4,050 t (extruder-expeller, 12% oil)
 ├─ crude oil 3,416 t  (sun 2,930 + soy 486)
 │    ├─ to feed (mash + coating) ............ 130 t
 │    ├─ to refinery 2,628 t -> RBD 2,497 t + soapstock 131 t
 │    └─ sold crude to refiners .............. 657 t
 ├─ sunflower cake 6,048 t -> feed 1,003 t; sold to dairy/poultry millers 5,045 t
 ├─ soy cake 3,321 t       -> feed 1,823 t; sold 1,498 t
 └─ process losses (impurities, moisture, foots) 715 t
Feed: mash 5,651 t (own cake/oil + purchased maize, pollard, omena, cottonseed cake, premix)
      -> 5,510 t finished (grow-out 4,683 t; starter 826 t); 2.5% shrink
```

- Source: `model/mass_balance_annual.csv`. All closure checks pass ([model/outputs.md §12](model/outputs.md)).
- With the smaller feed volume, 1.5 kt of soy cake is surplus and sold. That weakens the "secure non-GM protein" rationale for crushing soy.
- Refinery use peaks at 62%.

### 6.4 Feed formulation

The base grow-out formula is 29.7% CP: sunflower cake 20%, soy cake 30%, omena/fishmeal 7%, cottonseed cake 5%, maize 18%, pollard 13%, plus oil, bran and premix ([technical_operations.md §3.3](research/technical_operations.md)).
- **Raw-material cost:** about KES 71.5/kg blended in 2031 (2026 KES; [model/outputs.md §12](model/outputs.md)), against a cash cost of KES 88–93/kg.
- **Fibre is the binding constraint.** Ugandan trials found 15% sunflower cake best ([LRRD](https://lrrd.org/lrrd24/5/aany24084.htm), [DATED]).
- **Omena supply and aflatoxin risk** argue for a 0–3% fishmeal variant using soy, BSF or blood meal [ESTIMATE].
- **Nutritionist sign-off and KMFRI feeding trials would be a Phase 0b deliverable.**

### 6.5 Utilities and energy

- **Grid power:** KES 20/kWh all-in, plus a KES 1,100/kVA monthly demand charge. Sources: the EPRA 2023 schedule ([EPRA](https://www.epra.go.ke/wp-content/uploads/2023/01/ABRIDGED-KPLC-TARIFF-2023.pdf), [DATED]) plus KES 3.87/kWh of pass-throughs in June 2026 ([People Daily](https://peopledaily.digital/business/explainer-how-epras-new-electricity-bill-will-affect-households-and-businesses/amp)).
- **Tariff risk.** Kenya Power has warned of a rise of more than 30% from county wayleave charges ([Serrari](https://serrarigroup.com/kenya-power-warns-of-30-increase-in-electricity-prices-amid-mounting-wayleave-charges-and-debt-crisis/)).
- **Energy cost 2031:** KES 65m in 2026 KES, below the technical file's KES 76–84m because the feed line runs at half capacity.
- **Water:** about 30–50 m³/day [ESTIMATE].
- **Boiler fuel:** biomass at about KES 8/kg [ESTIMATE; no 2026 price found]. It must come from certified sustainable briquettes or residues, not uncontrolled firewood (section 14).

### 6.6 Quality standards

| Area | Requirement |
|---|---|
| Fish feed | KEBS S-mark under KS 2289-1. Internal release limit of 10 ppb aflatoxin [ESTIMATE] |
| Edible oil | Mandatory vitamin A fortification under KS EAS 769, as a condition of licence renewal ([ATNi, Jul 2025](https://accesstonutrition.org/app/uploads/2025/07/20250701_ATNi_EAMA_Kenya_Micronutrients_v2.pdf)). Filtration matters: KEBS failed imported oil on insoluble impurities ([Food Business MEA](https://www.foodbusinessmea.com/kebs-declares-government-imported-cooking-oil-unfit-for-consumption-unveiling-web-of-controversy/), [DATED]) |
| Customer-driven | HACCP; FSSC 22000 if moving to supermarket listings; ASC Feed Standard if supplying ASC farms [ESTIMATE] |
| QC laboratory (USD 0.15m) | NIR, Kjeldahl/Dumas, Soxhlet, FFA/PV, aflatoxin reader, floatability and pellet-durability tests |

### 6.7 Staffing

| Group | Phase 1 (about 70 FTE; KES 61m/yr including on-costs) |
|---|---|
| Management (6) | GM, plant manager, finance, procurement/outgrower, sales, QA |
| Laboratory | 4 |
| Operators | 41 |
| Maintenance (including a certified boiler operator) | 6 |
| Stores and logistics | 8 |
| Field extension officers | 6–10 |

Source: [technical_operations.md §4.3](research/technical_operations.md).
- **Phase 2 adds about 45 FTE** (KES 32m/yr) [ESTIMATE].
- **Wages.** The statutory machine-operator minimum is KES 24,359 a month in the five cities ([Kenyans.co.ke](https://www.kenyans.co.ke/news/124803-fke-announces-implementation-new-minimum-wages-workers)). The model pays KES 35–40k.

---

## 7. Regulatory, licensing and tax

### 7.1 Licensing roadmap and timeline

The source is [regulatory_tax_risk.md §3](research/regulatory_tax_risk.md); the timings are [ESTIMATE] unless cited.

| Month (from Phase 0 start, Q4 2026) | Step | Regulator |
|---|---|---|
| 0–2 | HoldCo, OpCo and PropCo; KRA PIN; **eTIMS, including reverse invoicing for smallholder seed**; investment certificate; AFA dealer registration (to buy trial seed); tax opinion | BRS, KRA, KenInvest, AFA |
| 1–6 | Land lease and change of user (2–9 months; the long pole); **NEMA EIA full study** (3–6 months including public participation, [Kenya Times](https://thekenyatimes.com/climate/environment-climate/eia-license-kenya/)); WRA permits; power connection application (3–9 months) | County LCB, NEMA, WRA, KPLC |
| 5–12 | County building approval; NCA registration; KEPHIS import permits for seed | County, NCA, KEPHIS |
| Build and commissioning (2028 to early 2029) | DOSH workplace and boiler certificates; effluent discharge licence (LN 177/2024, [Kenya Law](https://new.kenyalaw.org/akn/ke/act/ln/2024/177/eng@2024-12-06)); air licence; AFA processor licence; **KEBS marks on trial batches (2–4 months per SKU)**; feed-manufacturer registration | DOSH, NEMA, AFA, KEBS, DVS |
| Ongoing | EAC duty-remission quota applications each April; renewals; monitor the Livestock Bill 2026 ([Animal Business MEA, 15 Oct 2026](https://www.animalbusinessmea.com/2026/10/15/kenya-introduces-livestock-bill-to-regulate-animal-feeds/)) and the Food and Feed Safety Act 2026 ([The Star](https://www.the-star.co.ke/counties/2026-08-11-new-food-safety-law-seeks-to-protect-consumers-livestock)) | |

- From site selection to licensed operation takes about **15–21 months**, of which 6–9 months of regulatory steps are on the critical path.
- One-off licensing costs are KES 8–30m [ESTIMATE].
- Phase 2's solvent plant needs a fresh full EIA and hazardous-area classification.

### 7.2 Tax regime as modelled

| Item | Treatment | Source |
|---|---|---|
| CIT | 30% | [Chambers 2026](https://practiceguides.chambers.com/practice-guides/corporate-tax-2026/kenya) |
| Investment deduction | 100% in year 1 (outside Nairobi and Mombasa) [CONFLICT on the KES 250m / 1bn / 2bn threshold]. If it is denied, the 50% + 25% reducing-balance regime costs **0.1 points** of equity IRR | [PwC](https://taxsummaries.pwc.com/kenya/corporate/deductions); [regulatory_tax_risk.md row 3](research/regulatory_tax_risk.md) |
| Tax losses | 5-year expiry (Finance Act 2025). None expire in the base case | [The Standard](https://thestandard.ke/sports/amp/opinion/2001528930/how-businesses-can-navigate-new-tax-loss-restrictions) |
| Foreign interest (mezzanine) | Deductible up to 30% of EBITDA, with 3-year carry-forward; 15% WHT grossed up | [Grant Thornton](https://www.grantthornton.co.ke/insights/interest-restriction-rule/) |
| VAT | Oil 16%. Feed inputs zero-rated (proposals to exempt them were dropped in 2025 and 2026). Finished feed exempt or zero-rated [CONFLICT]. Base treats feed as exempt: 2% of feed revenue as irrecoverable VAT on **operating** inputs, and capex VAT apportioned by the exempt turnover share (35% in 2029–31), so **KES 93m of capex VAT is an up-front cost, not a refund** (v1.1 recovered 100%) | [Feed Business MEA, May 2026](https://www.feedbusinessmea.com/2026/05/26/finance-bill-2026-how-proposed-tax-shifts-will-impact-feed-industry-value-chain/); [regulatory_tax_risk.md row 19](research/regulatory_tax_risk.md) |
| Minimum tax | 1% of turnover where it exceeds CIT, at a **25% probability from 2028** (expected value). Struck down 2021–22; the MTRS commits to a redesign; not in Finance Bill 2026 | [IPF, Jan 2025](https://ipfglobal.or.ke/wp-content/uploads/2025/01/IS-A-MINIMUM-TAX-STILL-A-VIABLE-OPTION-FOR-KENYA.pdf); [KPMG, May 2026](https://kpmg.com/us/en/taxnewsflash/news/2026/05/kenya-tax-proposals-finance-bill-2026.html) |
| IDF and RDL on imported equipment | 2.5% and 2.0% | [Dawan/PwC, Jan 2026](https://www.dawan.africa/news/pwc-urges-importers-to-seek-refunds-after-high-court-strikes-down-10percent-palm-oil-duty) |
| Feed regulator levy | 0.5% of feed revenue (expected value) | [regulatory_tax_risk.md §4.4](research/regulatory_tax_risk.md) [ESTIMATE] |
| Dividends and exit | 5% dividend WHT for a resident individual; 15% CGT [UNVERIFIED] | [PwC WHT](https://taxsummaries.pwc.com/kenya/corporate/withholding-taxes) |

**Effective tax rate.**
- The 100% investment deduction defers corporate tax: **no material CIT is paid until 2035**, which is why a minimum tax would bite in the ramp years. Cumulative tax from 2027 to 2038 (KES 698m, including the expected minimum tax) is about 26% of cumulative pre-tax profit [calculation from `model/pnl_annual.csv`].
- Shareholder taxes (dividend WHT and CGT) cut equity IRR from 15.5% to 14.6%.
- Distributed profit bears a statutory 33.5% for a resident individual ([regulatory_tax_risk.md row 28](research/regulatory_tax_risk.md)). A Kenyan HoldCo holding at least 12.5% receives dividends tax-free and defers the second layer ([regulatory_tax_risk.md §2.5](research/regulatory_tax_risk.md)).

### 7.3 Incentives and structuring

- **SEZ route (not in base).** 10% CIT for 10 years ([CDH, Feb 2025](https://www.cliffedekkerhofmeyr.com/en/news/publications/2025/Practice/Tax-Exchange-Control/tax-and-exchange-control-alert-6-february-Not-so-special-after-all-An-analysis-of-the-impact-of-the-Business-Laws-Amendment-Act-2024-on-taxation-of-Special-Economic-Zones)) and an AFA levy exemption on EAC oil crops ([The Star, Apr 2025](https://www.the-star.co.ke/news/2025-04-18-no-import-levy-on-nuts-oil-crops-from-epzs)).
  - It is worth only **+1.1 points** of equity IRR in the model, and it ignores the risk that domestic sales are treated as imports.
  - No SEZ near Kisumu is confirmed.
  - **Do not pursue without advance rulings from SEZA and KRA.**
- **EAC duty remission** on premix and fishmeal from year 1: about KES 27m a year at a 20 kt feed scale [ESTIMATE, [regulatory_tax_risk.md §1.2](research/regulatory_tax_risk.md)]. Not modelled; it is upside.
- **Must-fix compliance.** eTIMS reverse invoicing for informal seed purchases. Without it, seed costs risk being disallowed: up to 30% × the informally bought seed cost ([biasharaguide](https://biasharaguide.co.ke/articles/significant-economic-presence-tax-kenya/); [regulatory_tax_risk.md §2.1](research/regulatory_tax_risk.md)). **Not modelled.**

### 7.4 Policy exposure (probability-weighted in the base case)

| Policy item | Probability used | Effect | Sources |
|---|---|---|---|
| CPO duty removed or unenforceable | 60% × −KES 15k/t on oil | Struck down by the High Court on 27 Nov 2025, yet listed among Kenya's 2026/27 increases [CONFLICT/legal void] | [AllAfrica](https://allafrica.com/stories/202511270355.html); [Wansom, 2 Oct 2026](https://www.wansom.ai/briefly/news/kenya-s-customs-squeeze-export-declarations-car-valuation-disputes-and-eac-tariff-moves-2026-10-02) |
| GM feed imports allowed | 40% × −25% on protein meals | | [regulatory_tax_risk.md §7](research/regulatory_tax_risk.md) |
| Duty waivers on feed ingredients | One year in three × −7.5% on cake | | as above |
| Tanzanian seed levy | 70% × 10% | | as above |
| Minimum tax reintroduced | 25% × 1% of turnover above CIT | MTRS commitment; not in Finance Bill 2026 | [round1_evidence.md §3](research/round1_evidence.md) |

Because the base case already weights these shocks by probability, each moves equity IRR only **0.1–2.3 points** when switched fully on or off. But each also moves the minimum DSCR by 0.3–0.9× (tornado, [model/outputs.md §8](model/outputs.md)).

---

## 8. Management, organisation and governance

### 8.1 Why management is the first risk to fix

- The investor-founder is a senior academic economist with no operating history in oilseed crushing, refining or feed milling.
- The best available evidence says this matters. Prior experience in the same industry predicts startup success, and the mean founder age among the fastest-growing 1-in-1,000 startups is 45 ([Azoulay, Jones, Kim and Miranda](https://ideas.repec.org/p/cen/cpaper/2018-03.html); cited in the [screening report](../../reports/Profitable%20business%20opportunities%202026.md)). Age is not the founder's constraint; sector experience is.
- Kenyan firm-survival data are stark but dated and about micro-firms: 46% of closed MSMEs closed in their first year ([KIPPRA/KNBS 2016](https://kippra.or.ke/14355-2/), [DATED]).
- **The plan therefore treats a sector-experienced general manager as a condition of FID, not a hire to be made after it.**

### 8.2 Key hires (in sequence)

| Role | When | Profile | Cost (model) |
|---|---|---|---|
| **General Manager / CEO** | Phase 0a, by month 6 | 10+ years running a crushing or feed plant in East or Southern Africa, from Bidco, Mukwano, Unga, Tunga, De Heus, ETG or similar; P&L ownership | KES 600k/month base [ESTIMATE, [technical_operations.md §4.3](research/technical_operations.md)], plus equity incentive: 3–5% vesting over 4 years, **modelled at 4%** (founder-group equity IRR 15.0% against 15.5%) |
| Procurement and outgrower manager | Phase 0, month 3 (runs the pilot) | Contract-farming experience (One Acre Fund, Farm Africa, Mukwano, Agventure) | KES 200k/month |
| Aquafeed nutritionist / technical director | Phase 0 (part-time consultant), full-time at commissioning | Extruded tilapia feed formulation; least-cost software | [ESTIMATE] within G&A |
| Plant and engineering manager | FID | Commissioning of expellers, refinery and extrusion; boiler and DOSH compliance | KES 350k/month |
| QA manager | FID | Aflatoxin control; KEBS and FSSC | KES 200k/month |
| Feed sales manager | 6 months before COD | Lake-region dealer network; cage-farm relationships | KES 200k/month |
| Finance manager | FID | Project-finance reporting, covenant compliance, eTIMS/VAT | KES 250k/month |

### 8.3 Board and governance

- **Board of five to seven.** The founder as non-executive chair; one independent with crushing or refining experience; one with aquaculture or feed experience; one finance/audit independent; seats for the co-investor and, if required, the mezzanine lender (observer). The GM attends.
- **Committees:** audit and risk (covenants, FX, commodity exposure), and E&S (DFI action plan, Lake Victoria engagement).
- **Policies:** a delegated-authority matrix; a commodity position limit of 3–4 months of unhedged stock ([financing_capital.md §7](research/financing_capital.md)); a related-party policy covering PropCo leases; an anti-bribery policy (Kenya scored 30/100 on the CPI in 2025, [TI](https://files.transparencycdn.org/images/CPI-2025-Report-EN.pdf)).
- **Legal structure.** HoldCo (Kenyan, founder plus co-investors) over OpCo (crusher and feed mill in **one** entity, so that feed profits absorb crusher losses under the 5-year loss cap), plus a wholly Kenyan-owned PropCo for land.

### 8.4 Partners

| Type | Candidates | Purpose |
|---|---|---|
| Technical | Extrusion OEM (Famsun or Muyang-class) with commissioning and 2-year service; oil-equipment OEM; KMFRI (Kegati/Sangoro) for feeding trials | Commissioning and formulation |
| Supply | Farm Africa, LBDA and county agriculture departments; licensed Ugandan aggregators; a WRS collateral manager; a named crusher for back-to-back resale of pilot seed | Seed and stock finance |
| Strategic co-investor (preferred) | A mid-size cage-farm group (feed offtake), a Rift feed miller (cake offtake) or a family office | Reduces failure probability and commercial risk ([financing_capital.md §6](research/financing_capital.md)) |

### 8.5 The founder's role

The founder's comparative advantages are patient equity in an equity-scarce market (Kenyan startups raised about USD 86m in Q3 2026, more than 92% of it as debt; [Business Today](https://businesstoday.co.ke/african-ventures-raise-us-674million-in-q3/)) and the ability to design and analyse evidence. Proposed responsibilities:
- Chair; capital allocation; DFI and lender relations.
- **Design and analysis of the Phase 0 experiments**, if the case is reopened: for example, randomising outgrower contract terms (floating against fixed price, with and without a cake buy-back) across farmer groups in the right-sized pilot [plan recommendation]. The model's CSVs, including `voi_draws.csv`, are Stata-ready.
- **Personal exposure.** Lenders are expected to ask for a founder personal guarantee and 125–150% collateral cover ([financing_capital.md §2](research/financing_capital.md), [PK-UNVERIFIED]). See section 10.1 and risk 12.
- Not day-to-day operations.

---

## 9. Financial projections

All figures are from `model/model.py` v2.0, nominal KES m unless stated. **Read IRRs as ±10 points:** most inputs are estimates and there are no binding quotes.

### 9.1 Annual summary (base case; Phase 2 gate fails, so Phase 1 only)

| KES m | 2029 | 2030 | 2031 | 2032 | 2033 | 2034 | 2035 | 2036 | 2037 | 2038 |
|---|---|---|---|---|---|---|---|---|---|---|
| Seed crushed (kt) | 6.0 | 11.0 | 13.5 | 13.5 | 13.5 | 13.5 | 13.5 | 13.5 | 13.5 | 13.5 |
| Aquafeed sold (kt) | 1.4 | 3.6 | 5.5 | 6.0 | 6.4 | 6.9 | 7.5 | 8.1 | 8.7 | 9.4 |
| Refined oil sold (kt) | 0.7 | 1.7 | 2.5 | 2.5 | 2.5 | 2.5 | 2.5 | 2.5 | 2.4 | 2.4 |
| Revenue | 755 | 1,604 | 2,301 | 2,489 | 2,694 | 2,919 | 3,166 | 3,436 | 3,733 | 4,059 |
| EBITDA | −18 | 186 | 408 | 428 | 462 | 506 | 554 | 607 | 664 | 727 |
| EBITDA margin | −2.4% | 11.6% | 17.7% | 17.2% | 17.1% | 17.3% | 17.5% | 17.7% | 17.8% | 17.9% |
| Net income | −172 | 6 | 214 | 235 | 270 | 327 | 248 | 298 | 335 | 374 |
| CFADS | −184 | 44 | 268 | 336 | 364 | 401 | 312 | 336 | 369 | 403 |
| DSCR (mezzanine only; no senior debt) | – | **0.92** | 2.43 | 3.21 | 3.71 | 4.42 | 3.78 | – | – | – |
| Equity injected (incl. cure) | 300 | 9 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| Distributions | 0 | 0 | 173 | 225 | 259 | 303 | 222 | 328 | 361 | 394 |
| EBITDA (USD m) | −0.12 | 1.21 | 2.55 | 2.57 | 2.66 | 2.81 | 2.96 | 3.11 | 3.28 | 3.45 |
| KES/USD | 148.1 | 154.0 | 160.2 | 166.6 | 173.3 | 180.2 | 187.4 | 194.9 | 202.7 | 210.8 |

- Pre-operating years: EBITDA is −112 in 2027 and −51 in 2028. Equity injected is 391 in 2027 and 946 in 2028.
- 2030 is the first full operating year and 2031 the first steady-state year. Commercial operation starts in April 2029.
- **Cost structure, 2031:** seed KES 1,086m (47% of revenue); purchased feed ingredients 275; energy 89; labour 87; dealer margin 48; irrecoverable feed VAT 19 (`model/pnl_annual.csv`).
- **Benchmark:** Phase 1 EBITDA in 2031 is KES 299m in 2026 KES, below the financing file's rough KES 400m (v1.1: 565m).

### 9.2 Unit economics (2026 KES)

| | 2031 (Phase 1) | 2035 (Phase 2, if built) | Research benchmark |
|---|---|---|---|
| Crush gross margin, per t of seed | 16,627 | 20,499 | About 12k ([feedstock_supply.md §8](research/feedstock_supply.md)) to about 31k ([market_demand.md §6](research/market_demand.md)) |
| Feed gross margin, per t of feed | 46,065 (36%) | 41,069 (33%) | Cash cost KES 88–93/kg against a KES 110–150 price ([technical_operations.md §3.3](research/technical_operations.md)) |
| EBITDA per t of seed | 22,166 | 21,878 | – |

The feed gross margin is still at the top of the research range. Distributor quotes and toll-produced test sales would be the first check.

### 9.3 Funding need (Phase 1, 2027–29)

| Uses | KES m | Sources | KES m |
|---|---|---|---|
| Capex incl. land, contingency, IDF/RDL | 1,402 | Founder and co-investor equity (incl. KES 112m Phase 0) | 1,637 |
| Phase 0 and pre-operating | 199 | Senior term loan (sized on the lender downside test) | **0** |
| Interest and fees | 14 | Mezzanine (USD 1.70m) | 242 |
| Working-capital build | 327 | Grants | 42 |
| Net VAT on capex (timing plus most of the KES 93m irrecoverable feed share) | 96 | Seasonal revolver at end-2029 | 161 |
| Tax and minimum cash | 63 | 2029 operating EBITDA | 17 |
| **Total** | **2,100** | **Total** | **2,099** |

Source: workbook sheet "Cash flow & funding".
- Peak net equity is **KES 1,646m in 2030**, including KES 9m of covenant cure: USD 10.7m at 2030 FX.
- Peak project funding need is KES 2,007m.
- Equity payback is 2037.

### 9.4 Returns

| Metric | Plan (gate auto = Phase 1 only) | Full plan (Phase 2 forced) |
|---|---|---|
| Project IRR, KES / USD | 15.3% / 10.9% | 11.9% / 7.6% |
| Project IRR, KES, no terminal value | 5.1% | −3.9% |
| **WACC of the modelled Phase 1 structure** (equity 87% at 35%, mezzanine 13% post-tax) | **32.3%** | 32.3% |
| Project NPV at 32.3% / at the financing file's 23% (memo) | −976 / −635 | −1,513 / −1,252 |
| Equity IRR, KES / USD | **15.5% / 11.1%** | 10.9% / 6.7% |
| Equity IRR, KES, no terminal value | 4.7% | −8.6% |
| Equity IRR after dividend WHT and CGT | 14.6% | 10.1% |
| Equity IRR, founder group after the GM's 4% equity | 15.0% | 10.4% |
| Equity NPV at 35% / 40% | −879 / −936 | −1,292 / −1,294 |
| Minimum DSCR / cure equity | 0.92x (2030) / 9 | 0.89x / 143 |

**WACC (R1-04).**
- v1.1 compared the project IRR with a 23% WACC that assumed 50% equity. The structure actually modelled is 87% equity, because no senior debt passes the downside test, which gives a WACC of 32.3%.
- The project IRR of 15.3% is below the WACC on either basis. It is also near the 15.5% cost of senior debt, so **leverage cannot rescue the equity return**. If lenders fund 2030 interest from the budget and test from 2031 with a 24-month grace, the plant could carry KES 177m of senior debt, and equity IRR is unchanged at 15.4% ([model/outputs.md §6](model/outputs.md)).

**Phase 2 on its own terms.**
- Gate (d) now tests Phase 2 at the cost of the capital that would fund it. Existing shareholders' equity is at the 35% hurdle; the funding-mix WACC is 21.1% for the project view.
- In the base, Phase 2's incremental project IRR is 5.7% and its incremental equity IRR 0.6%. The incremental equity NPV at 35% is −KES 413m. Gate (b1) also fails (5.5 kt of feed against 8 kt).
- **Phase 2 is live only in the bull case,** where its incremental equity IRR is 50% (section 12.3).

**The exit carries the return.**
- The 2038 terminal value is 5.0× EBITDA of KES 727m: EV KES 3.6bn, or USD 17.2m at 2038 FX.
- At 4× / 7× the equity IRR is 14.0% / 18.1%; without exit value it is 4.7%.

### 9.5 Scenarios and restructure alternatives

Senior debt is held at base sizing (zero) in every case. Each case reports its minimum DSCR and cure equity ([model/outputs.md §7](model/outputs.md)).

| | Bear | Base | Bull | Competitor response | UG/TZ upside | v1.1 market (bridge) | Feed-mill-first | Crusher-only |
|---|---|---|---|---|---|---|---|---|
| Phase 2 | No-go | No-go | Go | No-go | No-go | No-go | n/a | n/a |
| Equity IRR, KES | n/a (losses) | 15.5% | 43.5% | 5.2% | 19.9% | 27.9% | 9.6% | 1.5% |
| Project IRR, KES | n/a | 15.3% | 39.2% | 7.1% | 19.1% | 26.0% | 10.8% | 4.8% |
| Equity NPV at 35% | −2,232 | −879 | 591 | −1,080 | −712 | −361 | −625 | −819 |
| EBITDA 2031 | −150 | 408 | 1,095 | 357 | 544 | 738 | 138 | 195 |
| Feed sold 2031 (t) | 3,078 | 5,510 | 10,447 | 5,510 | 8,155 | 9,918 | 5,510 | 0 |
| Minimum DSCR | −6.43 | 0.92 | 3.69 | 0.04 | 2.19 | 4.20 | −0.73 | −0.36 |
| Cure equity | 2,630* | 9 | 0 | 51 | 0 | 0 | 131 | 98 |
| Peak net equity | 6,127* | 1,646 | 1,199 | 1,697 | 1,635 | 1,522 | 1,029 | 1,185 |

\*In the bear case the model keeps injecting equity and cures to fund losses. A real owner would stop; the survival view models that stop as failure plus liquidation.

**Scenario definitions.**
- **Bear:** each market and cost driver half-way to its adverse bound, including SAM 20 kt, refined spread 52.5k and a 2% feed decline; seed supply ×0.85; CPO, GMO and Tanzanian levy shocks certain; exit at 4.5×.
- **Bull:** each driver half-way to its favourable bound, including SAM 31 kt, feed ×1.10, share 20%, seed ×0.895 and capex ×0.85; no policy shocks; exit at 6.0×.
- **Competitor response:** 3% a year real feed decline from 2029 plus a 10% entrant discount.
- **UG/TZ upside:** +12 kt of lake-shore demand in the SAM.
- **v1.1 market:** restores SAM 45 kt, crude 190k and refined 264k, with no decline, no minimum tax and full capex-VAT recovery, under v2.0 financing rules.
- **Feed-mill-first / crusher-only:** the [ESTIMATE] capex and fixed-cost scaling in `CONFIG_CAPEX` and `CONFIG_FIXED`.

**The restructure alternatives are worse than the integrated plant.**
- A feed mill that buys protein at market prices keeps the feed margin. But it loses the crush and refining spread, and still carries most of the fixed cost: 9.6%.
- A crusher without the feed line sells cake into a commodity market: 1.5%.
- **Integration is not the problem; market size and prices are.**

### 9.6 Sensitivities, break-evens and joint cases

**Tornado** (one driver at a time; base equity IRR 15.5%, minimum DSCR 0.92x; senior debt at zero). Full table with cure and peak equity: [model/outputs.md §8](model/outputs.md).

| Driver (low / high setting) | Equity IRR low | Equity IRR high | Min DSCR low | Min DSCR high | Cure equity, KES m (low / high) |
|---|---|---|---|---|---|
| Delivered seed cost (×0.79 / ×1.26) | 26.0% | −8.8% | 4.68 | −4.01 | 0 / 741 |
| Feed prices (×0.88 / ×1.20) | 7.5% | 24.0% | −0.28 | 2.93 | 67 / 0 |
| Feed market share (8% / 25%) | 6.8% | 20.8% | −0.32 | 2.69 | 68 / 0 |
| Feed real price decline (3% / 0% a year) | 5.5% | 19.0% | 0.54 | 1.11 | 27 / 0 |
| Contestable SAM 2026 (15 / 37 kt) | 8.3% | 19.9% | −0.14 | 2.19 | 60 / 0 |
| Capex (×0.70 / ×1.45) | 20.9% | 9.4% | 1.24 | 0.44 | 0 / 32 |
| Oil index with fixed-price seed (crude 155k / 200k) | 6.4% | 17.2% | −1.49 | 1.42 | 130 / 0 |
| Sunflower oil yield (27% / 34%) | 10.6% | 18.3% | −0.38 | 1.80 | 72 / 0 |
| Refining spread (refined 215k / 265k) | 11.4% | 18.9% | −0.05 | 1.89 | 55 / 0 |
| Oil index with 50% seed pass-through (crude 155k / 200k) | 13.7% | 17.5% | 0.42 | 1.55 | 33 / 0 |
| Exit multiple (4× / 7×) | 14.0% | 18.1% | 0.92 | 0.92 | 9 / 9 |
| Minimum tax (certain / never) | 15.1% | 15.7% | 0.67 | 1.00 | 21 / 5 |
| Feed VAT-exempt / zero-rated (capex VAT) | 15.5% | 16.1% | 0.92 | 0.92 | 9 / 9 |

**The base case and every adverse tornado setting breach the 1.10x default covenant in 2030.** This is not because debt is high: the base carries only USD 1.7m of mezzanine. It is because the 2030 ramp year barely covers mezzanine interest. Deferring mezzanine cash interest one more year (three PIK years instead of two) removes the base breach (minimum DSCR 2.15x) [supplementary run]. That would be a term to negotiate, but it changes neither the IRR nor the verdict.

**Break-evens** ([model/outputs.md §11](model/outputs.md); senior debt held at base where stated):

| Driver | Base | Min DSCR = 1.10x (others at base) | 35% conditional equity IRR (others at base) | **Kill threshold**: 35% survival-weighted at p_fail 20%, every other driver at bull |
|---|---|---|---|---|
| Contestable SAM 2026 | 25.0 kt | 26.7 kt | not reachable (≤60 kt) | **23.7 kt** |
| Feed price (× list) | 1.00 (KES 125/kg) | 1.018 | not reachable (≤1.5) | **0.991 (KES 124/kg)** |
| Feed share | 15% | 16.0% | not reachable (≤40%) | **15.3%** |
| Seed cost (× path) | 1.00 (KES 57.6k/t) | 0.990 | **0.567** (KES 33k/t) | **1.014 (KES 58.4k/t)** |
| Capex (× base) | 1.00 (USD 9.5m) | 0.830 | not reachable (≥0.4) | **1.040 (USD 9.9m)** |
| Refining spread | 65k (refined 240k) | 69.6k | not reachable | **37.3k (refined 212k, KES 193/L)** |
| Oil index (crude) | 175k | 182k | not reachable | 122k |

- **No single driver within its research range reaches a 35% conditional equity IRR**, except seed at KES 33k/t, far below the 45k research low.
- The kill column is the decisive one. With every other driver at its favourable value, the case still fails if SAM, feed price, share, seed cost or capex comes in at base or worse.

**Joint cases** (senior debt re-sized for each; founder flows; [model/outputs.md §11](model/outputs.md)):

| Case | Conditional equity IRR | Survival-weighted IRR (p_fail 30% / 20%) | Founder NPV at 35% (30% / 20%), KES m | Senior sized | Phase 2 |
|---|---|---|---|---|---|
| Base | 15.5% | 8.4% / 10.4% | −1,121 / −1,049 | 0 | No-go |
| v1.1 Case A: feed +10%, seed −10%, capex −15% | 28.1% | 17.6% / 20.6% | −726 / −600 | 226 | No-go |
| Case A + SAM 32 kt | 31.8% | 20.4% / 23.7% | −622 / −481 | 324 | No-go |
| Case B: SAM 32 kt, share 20%, feed +10%, seed −10%, capex −15%, refined 250k | 36.7% | 23.5% / 27.3% | −475 / −315 | 511 | No-go |
| Case B + Uganda/Tanzania 12 kt | 40.6% | 29.0% / 32.4% | −319 / −138 | 616 | Go |
| Bull (every driver half-way favourable) | 46.6% | 33.6% / **37.4%** | −78 / **+139** | 610 | Go |

**Only the bull case at a 20% failure probability clears the 35% expected hurdle.** v1.1's Case A, which cleared at 20% failure risk on the old market assumptions, now gives 20.6%.

### 9.7 Survival-weighted returns against the hurdles

| Branch | Probability | Equity IRR | Equity NPV at 35% | Founder NPV at 35% (incl. guarantee and GM) |
|---|---|---|---|---|
| Early failure: bear operations to 2030, liquidation in 2031 at 35% of capex and 70% of WC | 30% | −50.5% | −1,623 | −1,623 |
| Late failure: base Phase 1 operations to 2034, liquidation in 2035 (price war, Phase 2 start-up or exit failure) | 7% (10% of survivors) | 0.8% | −1,008 | −1,008 |
| Survive, Phase 1 only (the base gate is a no-go, so P(Phase 2) = 0) | 63% | 15.5% | −879 | −894 |
| **Expected** | | **8.9%** (founder 8.4%; after shareholder tax 7.6%) | **−1,111** (−1,134 at 40%) | **−1,121** (−1,141 at 40%) |

Source: [model/outputs.md §9](model/outputs.md). The 30% early-failure probability is the screening report's illustration. The 10% late-failure probability, the 35% recovery and the guarantee terms are judgement. No Kenyan base rate exists ([round1_evidence.md §5](research/round1_evidence.md)).

**Against the hurdles:**
- **Greenfield, 35–40% expected:** fails at every failure probability. Even with zero early-failure risk the expected IRR is 14.7%. The sweep: 10% → 12.9%; 20% → 11.0%; 30% → 8.9%; 45% → 5.4%; 60% → 1.2%.
- **Established business, 25–30%:** fails even conditional on survival (15.5%).
- **Tax-free infrastructure bond, 11.75–12.74%** ([Serrari](https://serrarigroup.com/cbk-opens-ksh150bn-tax-free-infrastructure-bond-sale/)):
  - v1.1 compared the bond with survival-conditional, pre-tax flows (+KES 3.43bn then; +KES 397m now).
  - On the correct basis (survival-weighted founder flows after dividend WHT and CGT, with GM dilution and the guarantee), **the NPV at 12.25% is −KES 479m. The bond wins.**
- **Bank lending, about 14.4%** ([Capital FM](https://capitalfm.africa/private-sector-credit-growth-accelerates-to-10-6pc-in-september/)): the project IRR (15.3%) barely exceeds the cost of debt, so leverage adds nothing.

### 9.8 Bridge from v1.1 to v2.0 (equity IRR, KES)

| Step | Conditional | Survival-weighted | Min DSCR | Senior sized (KES m) | EBITDA 2031 |
|---|---|---|---|---|---|
| v1.1 as published | 28.9% | 22.3% | 1.30 | 416 | 770 |
| + v2.0 financing rules: downside sizing, cures, gate (d) at 35%, four-branch tree | 28.3% | 19.2% | 1.62 | 248 | 738 |
| + SAM rebased to the contestable Kenyan market (45 → 25 kt) | 21.8% | 14.4% | 1.62 | 29 | 492 |
| + oil parity (crude 190 → 175k; refined 264 → 240k, linked) | 19.8% | 12.7% | 1.20 | 0 | 434 |
| + feed prices −1% a year real from 2029 | 16.3% | 9.5% | 1.00 | 0 | 408 |
| + minimum tax (25% probability) and capex VAT apportioned | **15.5%** | **8.9%** | 0.92 | 0 | 408 |

[supplementary runs of `model.py`, applying the changes in sequence and re-sizing debt at each step]

---

## 10. Financing plan and capital structure

### 10.1 Phase 1 sources, if the case were reopened

| Instrument | KES m | USD m (2028 FX 142.4) | Terms (model) | Likely providers and evidence |
|---|---|---|---|---|
| Founder and co-investor equity (net, including Phase 0) | 1,637 | 11.5 | Ordinary equity; the GM's 4% vests over 4 years | Founder; preferably a strategic co-investor |
| of which the incremental FID ask, net of Phase 0 | 1,525 | 10.7 | | |
| Standby equity for overruns | 210 (undrawn) | 1.5 | 15% of capex | Founder |
| Senior KES term loan | **0 on the downside test** (177 if 2030 interest is funded from the budget) | 0 (1.2) | 15.5%; 7 years; 18–24 months' grace; lock-up at 1.30×; default at 1.10× with equity cure; first charge; **founder personal guarantee and 125–150% collateral cover expected** [PK-UNVERIFIED] | KCB, Equity, Stanbic, NCBA, Co-op, ideally with IFC or BII risk-sharing ([BusinessTech Africa](https://www.businesstechafrica.co.za/article/african-smes-are-finding-another-way-to-borrow-money)) |
| Mezzanine (USD) | 242 | 1.70 | 13% plus 15% WHT gross-up; 8 years; 3-year grace; **3 PIK years needed** to avoid the 2030 breach | AgDevCo: USD 9.5m to Agventure ([AgDevCo PR](https://www.agdevco.com/site/assets/files/2133/agventure_press_release_nov_2024.pdf), [DATED]); AgDevCo Ventures reached a USD 49m first close in Aug 2026 with GBP 0.75–2.5m tickets ([AgDevCo PR, Aug 2026](https://www.agdevco.com/site/assets/files/2918/press_release_agdevco_ventures_-further_funding_announcement_august_2026.pdf)), which fits the ticket, though mezzanine appetite for a greenfield processor is unconfirmed |
| Grants | 42 | 0.30 | Outgrower and ESIA co-funding | AECF, foundations [UNVERIFIED] |
| Seasonal stock-finance revolver | 161 at end-2029 (intra-year peak 353) | 1.1 | 14.5%; 65% of seed stock under collateral management or WRS | Lead bank plus a collateral manager |

**Debt sizing is now an explicit FID test (D1, section 12.2).**
- Senior debt is sized on a lender downside case, with CFADS cut by 20% before the 1.30× test. In the base no senior debt passes.
- Below 1.10× the sponsor must inject cure equity. The model applies the cure to prepay senior and charges a 1% waiver fee. Below 1.30× distributions stop and 50% of excess cash prepays senior. All cure equity is counted in peak equity and in the IRRs.

**Evidence basis of the financing terms.** `financing_capital.md` rests on a single web search. Most of its terms are [PK-UNVERIFIED] prior knowledge: rates, tenors, guarantees, collateral cover, AGF terms and TCX pricing ([round1_evidence.md §4](research/round1_evidence.md)). A TCX-hedged KES DFI loan at 14% is probably optimistic, but it matters only in the bull case, where Phase 2 is live.

**Founder's personal downside.**
- A personal guarantee converts limited-liability equity loss into personal exposure, up to the full senior balance (KES 0–616m across the cases above).
- On the model's 20–35% liquidation recoveries, plant resale covers senior debt in every modelled failure branch, so no call arises. The exposure bites only if a single-use plant in Kisumu sells for well under a fifth of its cost, which is plausible in a distressed sale.

### 10.2 Phase 2 sources

Phase 2 is a no-go in the base. In the bull case it would be funded by 55% KES DFI debt (KES 1.6bn at 14%, 9 years) and equity.
- The model tests it at existing shareholders' 35% hurdle.
- **Recommended variation (not modelled):** fund the Phase 2 equity with a 25–40% minority from an outside fund at a step-up valuation.

### 10.3 Phasing of the capital commitment (as recommended in v2.0)

| Stage | Commitment | FX used | Decision gate |
|---|---|---|---|
| Now | **Nothing**, or at most USD 50k (about KES 7m) for a desk check | 2026 spot | Founder's choice (section 12.5) |
| Phase 0a (only if the desk check reopens the case) | USD 0.3m = KES 41m | 2027: 136.9 | Stop gate S1 (section 12.5) |
| Phase 0b | USD 0.5m + USD 0.05m expected pilot seed loss = KES 75m | 2027: 136.9 | Stop gate S2 |
| FID | KES 1,525m of equity net of Phase 0 (USD 10.7m), plus KES 210m standby (USD 1.5m) | 2028: 142.4 | G0 (section 12.2) |
| Phase 2 | Bull case only | – | G1 |

---

## 11. Risk register and mitigants

The register is ranked by expected impact on equity value. Probabilities are [ESTIMATE] unless cited. IRR and DSCR effects are from the v2.0 tornado and scenarios.

| # | Risk | Probability (2027–31) | Impact | Mitigants | Early-warning indicator |
|---|---|---|---|---|---|
| 1 | **Feed market size and share.** The contestable Kenyan market is about 25 kt; Victory Farms is about half of cage output and captive; regional capacity is several times demand | High | SAM 15 kt: equity IRR 8.3%, min DSCR −0.14. Share 8%: 6.8% | Census before any commitment; anchor LOIs; starter niche; toll or protein-supply deal | Census result; non-VF cage licences |
| 2 | **Feed price war** (Tunga 45 kt, SamakGro 8 t/h) | About 50% that real prices fall 3% a year or more | 3% a year decline: 5.2–5.5%, min DSCR 0.04–0.54 | Low-cost formulation; service; non-GM positioning | Competitor list prices; dealer quotes |
| 3 | **Seed cost and volume** | About 40% that year-1 throughput is below 60% of plan ([feedstock_supply.md §10](research/feedstock_supply.md)) | Seed ×1.26: −8.8%, cure KES 741m. Supply ×0.70: 14.2%, min DSCR −0.09 | Floating parity-linked contracts; three-country sourcing; cake buy-back | Pilot delivery rate; side-selling |
| 4 | **Refined-oil price and duty** (20 L parity unquoted; duty on refined imports [CONFLICT]; misdeclared or duty-free imports) | 30% that the realised price is below KES 225k/t | Refined 215k: 11.4%, min DSCR −0.05 | Quotes before commitment (K11); institutional contracts | KRA tariff; Mama Pima expansion |
| 5 | **Capex overrun and delay** | About 30% for a more than 20% overrun | ×1.45: 9.4%, min DSCR 0.44 | Three written quotes per package; fixed-price civil works; contingency; standby equity | Quotes above USD 9.9m (K6) |
| 6 | **Covenant breach and cure** (ramp-year CFADS barely covers mezzanine interest) | Base case breaches in 2030 | Cure KES 9m in the base; KES 27–741m in adverse settings | Three PIK years on mezzanine; lender downside sizing; cure reserve in the standby equity | Quarterly CFADS from 2029 |
| 7 | **Policy reversal on oil.** CPO duty lost (60%); duty-free oil imports (25%) | 60% / 25% ([regulatory_tax_risk.md §7](research/regulatory_tax_risk.md)) | Certain CPO removal: 15.0% | Probability-weighted in base; seed price linked to parity | EAC gazette each June |
| 8 | **Management and execution** | High without mitigation | Drives the 30% failure probability | Experienced GM before FID; independent directors | GM not hired |
| 9 | **GMO ruling allowing GM imports** | 40% by end-2028 | Certain: 14.1% | Never accept GM material | Court of Appeal judgment |
| 10 | **Lake Victoria social licence** (Senate petition 5 Aug 2026; hearings 2 Oct 2026) | 40% zoning; 10% moratorium | SAM growth 4%: 10.4% | Diversify buyers; support zoning; FCR advisory | Senate report; KeFS data |
| 11 | **Minimum tax reintroduced** (1% of turnover where it exceeds CIT). Struck down 2021–22 ([Mondaq](https://mondaq.co.uk/capital-gains-tax/1269472/court-of-appeal-upholds-decision-declaring-minimum-tax-as-unconstitutional), [DATED]); the MTRS 2024/25–2026/27 commits to reintroduction ([IPF](https://ipfglobal.or.ke/wp-content/uploads/2025/01/IS-A-MINIMUM-TAX-STILL-A-VIABLE-OPTION-FOR-KENYA.pdf)); not in Finance Bill 2026 ([KPMG](https://kpmg.com/us/en/taxnewsflash/news/2026/05/kenya-tax-proposals-finance-bill-2026.html)) | **25% from 2028** (base expected value) | Certain: equity IRR 15.1%, min DSCR 0.67. Bites in the ramp years, when CIT is nil because of the investment deduction | Tax opinion; lobby via KAM | Finance Bills each June |
| 12 | **Personal guarantee and collateral** (125–150% cover expected [PK-UNVERIFIED]) | Near-certain if senior debt is raised | Founder exposure up to the senior balance if resale value collapses | Negotiate limited or springing guarantees; IFC/AGF risk-sharing | Term sheets |
| 13 | **Election, 10 Aug 2027** | 30% for 2+ weeks of disruption; 50% for KES depreciation above 6% in 2027 | Capex delay; FX on imported plant | FID only after the result is settled | KES forwards |
| 14 | **FX** | Base 4% a year; tail 20–25% | USD IRR 11.1% against KES 15.5% | Mezzanine at 37% or less of term debt; USD trade lines | CBK reserves |
| 15 | **Aflatoxin and quality incident** | 15–25% in 5 years | Loss of brand and KEBS mark | Lot testing; no groundnut | Rejection rates |
| 16 | **VAT: feed exempt or zero-rated; refunds; eTIMS** [CONFLICT] | 60% for refund delays above 6 months | Exempt feed makes KES 93m of capex VAT irrecoverable (modelled) | KRA private ruling; eTIMS reverse invoicing | KRA ruling |
| 17 | **Exit risk:** no Kenyan agro-processing multiple observed | – | 4×: 14.0%; no exit value: 4.7% | Build a strategic buyer universe | Approaches |
| 18 | Power cost; hexane safety (Phase 2); government arrears; price controls | 10–30% | −0.5 to −1.1 points each | As in v1.1 | – |

---

## 12. Implementation plan and decision gates

### 12.1 Decision now

The v1.1 timeline (Phase 0 in Q4 2026–Q3 2027, FID Q4 2027, COD April 2029) is **suspended**. The model's verdict on current evidence is to stop, because no stage of Phase 0 has positive expected value against stopping (section 12.6). The timeline below applies only if the founder chooses the desk check and it reopens the case.

| Period | Milestone (conditional) |
|---|---|
| Q4 2026 (4–6 weeks) | Desk check, up to USD 50k (§12.5). Stop gate S0 |
| Q1–Q2 2027 | Phase 0a, USD 0.3m: census, quotes, capex, GM search. Stop gate S1 |
| Q2–Q4 2027 | Phase 0b, USD 0.55m: right-sized pilot, toll trials, EIA, financing. Stop gate S2 / G0 after the 10 August 2027 election |
| 2028 | Construction (15 months) |
| About April 2029 | COD |
| Early 2032 | G1 on 2031 audited results |

### 12.2 Gate G0 (FID): calibrated kill and proceed criteria

**Kill: abandon if any one of these holds.** Thresholds marked † come from the re-run model: each is the value at which the survival-weighted founder IRR equals 35% at a 20% failure probability with every other driver at its bull value. Worse than that, no plausible combination of the other drivers passes ([model/outputs.md §11](model/outputs.md)).

| # | Test (in the model's own units) | Kill threshold | Base | Model reference |
|---|---|---|---|---|
| K1† | Contestable Kenyan merchant extruded-feed demand, 2026-equivalent (census, net of Victory Farms captive and SamakGro VF-linked sales; `sam_2026`) | **Below 24 kt** | 25 kt | Below 26.7 kt the base also breaches 1.10× |
| K2† | Achievable grow-out list price before dealer margin (quotes, trial sales) | **Below KES 124/kg** | 125 | – |
| K2b† | Share implied by feed LOIs and the census | **Below 15%** | 15% | – |
| K3† | Delivered blended sunflower seed cost (signed terms plus pilot) | **Above KES 58k/t** | 57.6k | – |
| K4 | Seed contracted or under credible import agreement for 2029 | Below 8 kt | – | [financing_capital.md §6](research/financing_capital.md) |
| K5 | Pilot outcome | Side-selling above 50%, or delivered yield below 0.6 t/ha | – | Research adverse bounds |
| K6† | Firm Phase 1 capex quotes | **Above USD 9.9m** | 9.5m | – |
| K7 | Lab-tested oil content of target-county seed | Full-press yield below 28% | 31% | At 27%: 10.6% |
| K8 / **D1** | **Debt capacity**: senior sized by the lender's own term sheet on the 20%-haircut downside | **Below KES 300m, or any cure needed in the base** | 0 | Every joint case that clears the hurdle carries KES 600m or more |
| K9 | Management | No sector-experienced GM signed | – | Section 8 |
| K10 | Policy | Broad moratorium on new cage licences in Siaya and Homa Bay | – | [regulatory_tax_risk.md §7](research/regulatory_tax_risk.md) |
| K11† | 20 L refined oil: institutional and wholesale quotes in Kisumu, ex-VAT | **Below KES 212k/t (KES 193/L)** | 240k | – |

**Proceed: FID only if all kill tests pass AND the model, re-run with the Phase 0 values, gives a survival-weighted founder IRR of at least 35% at a failure probability the board can defend** (20% or less, given the risk reducers below).
- On current inputs that requires roughly the bull case: SAM of 31 kt or more, feed price ×1.10, share 20%, seed ×0.90, capex ×0.85, refining spread 77.5k, no policy shocks, exit at 6×.
- Risk reducers needed to defend 20%: feed LOIs of at least 3 kt a year from five or more non-Victory farms; LOIs for at least 50% of crude oil or cake; at least 10 kt of seed contracted; an experienced GM in post.

**v1.1's thresholds were too loose.** For example, K1 at 20 kt admitted a minimum DSCR of 0.53×. Every threshold is now calibrated to the re-run model.

### 12.3 Gate G1 (Phase 2, on 2031 audited results)

Phase 2 is live only in the bull case. There, Phase 2's incremental equity IRR is 50%, with 2031 feed of 10.4 kt at a 38% gross margin and a 2031 DSCR of 3.08×. Phase 2's incremental equity NPV turns negative at seed ×1.22 or supply ×0.68, with others at bull. It is not sensitive to the feed price until ×0.73. Gates:
- (a) At least 24 kt of seed **contracted** for 2035. Seed is the binding Phase 2 driver.
- (b) 2031 feed sales of at least 9 kt at a gross margin of at least 30%. This is calibrated to the bull path less a margin. v1.1's 20% was too loose: at 20%, 2031 EBITDA would be far below the covenant level.
- (c) At least 70% of crude refined under the own brand.
- (d) **Positive incremental equity NPV at 35%**, the cost of the existing shareholders' equity that funds it. v1.1 tested 16.5%.
- (e) A 2031 DSCR of at least 1.5× with no cure in 2029–31.
- (f) Outside Phase 2 equity priced at or above the Phase 1 equity invested.

### 12.4 Operating tripwires (2029–31)

A board review of turnaround, sale or wind-down is triggered by any of:
- 2030 EBITDA below KES 150m (model 186);
- 2030 feed sales below 3 kt (model 3.6);
- seed crushed in 2030 below 7 kt (model 11.0);
- any covenant cure.

The survival tree's failure branches show the cost of acting late.

### 12.5 Staged Phase 0 with stop gates (replaces the v1.1 USD 0.8m programme)

| Stage | Content | Cost [ESTIMATE] | Stop gate |
|---|---|---|---|
| **S0: desk check** (optional, founder's choice) | Telephone census via county fisheries officers and three or four distributors of non-VF cage farms' feed use; Victory Farms' Kenya output from KeFS licensing data; three distributor quotes for grow-out feed and three for 20 L oil in Kisumu; the KRA tariff line for refined oils; two budget capex quotes | **≤ USD 50k** | Stop unless the census implies SAM ≥ 32 kt **and** quotes imply feed ≥ KES 137/kg and refined ≥ KES 250k/t |
| **0a** | Full market census (sample of cage farms in Siaya, Homa Bay, Busia and Migori); dealer margins and credit terms; three written CIF quotes per equipment package; lab tests on 20–30 seed lots; GM retained search | USD 0.3m (KES 41m) | Stop if any K1, K2, K2b, K6, K7 or K11 fails, or the re-run model is below 35% at p_fail 20% with seed at base |
| **0b** | **Right-sized pilot:** 500–600 ha (about 500 t of seed) under randomised contract terms, with a signed **back-to-back resale contract** with a named crusher (Bidco, Menengai, or a toll-crush with a Rift crusher) before planting. Seed working capital of about KES 26–30m is revolving, with an expected loss of USD 0.05m budgeted. Plus toll-extruded feed trials (200–500 t), EIA, legal and tax rulings, and financing term sheets | USD 0.5m + 0.05m = KES 75m | G0 |

- **Why the v1.1 pilot was wrong.** 2,000–3,000 ha would buy 1,800–2,700 t of seed (KES 95–140m) with no plant to crush it and no buyer. That was more than the plant's own year-1 outgrower base, and none of the seed was in the budget.
- The right-sized pilot measures the side-selling rate against a credible buyer, which is the commercially relevant measure.

### 12.6 Value of information: why the recommendation is to stop

[model/outputs.md §10](model/outputs.md); 150 draws per prior; founder NPV at 35%, KES m, value date 2027; Phase 0 costs charged as the option price:

| Prior | Failure probability | Stop | Invest now (no info) | Phase 0a only | Staged 0a → 0b | Perfect information | P(pass) | Gross value of perfect information |
|---|---|---|---|---|---|---|---|---|
| Independent (ρ = 0) | 30% | 0 | −1,059 | −41 | −41 | −116 | 0.0% | 0 |
| Independent (ρ = 0) | 20% | 0 | −995 | −41 | −41 | −116 | 0.0% | 0 |
| Correlated (ρ = 0.5) | 30% | 0 | −1,049 | −38 | −36 | −110 | 2.0% | 6 |
| Correlated (ρ = 0.5) | 20% | 0 | −984 | −32 | −32 | −105 | 3.3% | 12 |

- **Priors** [ESTIMATE]:
  - triangular(low, base, high) on SAM, feed price, share, feed decline, capex, oil index and refining spread, which Phase 0a reveals;
  - the same on seed cost and supply, which Phase 0b reveals.
  - ρ = 0.5 lets favourable outcomes cluster, which is generous to the project.
- **Reading.**
  - Even perfect, free information is worth at most KES 12m (about USD 90k at 2027 FX), and only under the generous prior.
  - Phase 0a alone costs KES 41m, so every Phase 0 policy is worse than stopping.
  - The VOI treats Phase 0 as revealing true values. Real tests are noisy, so these are upper bounds.
- **The optional S0 desk check (≤ USD 50k)** is justified only for a founder whose own prior puts materially more weight on a large-market, high-price world than these priors do. A plausible reason would be that Victory Farms' Kenyan share is much smaller than §2.3 estimates.

### 12.7 Restructure alternatives

| Alternative | Evidence | Result |
|---|---|---|
| **Feed-mill-first** (3 t/h line buying protein; no crusher) | Modelled (`config` = 1) | Equity IRR 9.6%; min DSCR −0.73; peak equity KES 1,029m. **Reject** |
| **Crusher + refinery only** (sell cake, e.g. a protein-supply deal with Tunga, SamakGro or De Heus) | Modelled (`config` = 2) | Equity IRR 1.5%. **Reject** |
| **Acquire an under-used existing feed mill** (millers run at 50–60% use, [The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)) | Not modelled; no price or target identified | The only structure that attacks the capex and fixed-cost problem. It still faces the same 25 kt market. Worth a separate desk screen only if S0 shows a larger market |
| **JV with a strategic** (cage-farm group or feed multinational bringing offtake) | Not modelled | Shifts market risk to a partner but caps upside; requires a counterparty. No approach has been made |
| **Redeploy capital** (screening report's higher-ranked opportunities; tax-free infrastructure bonds at 11.75–12.74%) | Screening report | The bond alone beats this plan's survival-weighted after-tax return (−KES 479m NPV at 12.25%) |

---

## 13. Exit options and valuation

**Valuation basis.**
- The base exit is 5.0× 2038 EBITDA [ESTIMATE, [financing_capital.md §8](research/financing_capital.md)]: EV of KES 3.6bn (USD 17.2m at 2038 FX) and equity of about KES 3.4bn.
- Anchors: KPC's IPO at about 8.1× EV/EBITDA, a regulated-infrastructure upper bound ([african-markets](https://www.african-markets.com/en/stock-markets/nse/kenya-pipeline-company-ipo-subscribed-at-105-7-listing-on-the-nairobi-securities-exchange-scheduled-for-march-10)); US lower-middle-market private equity at 5.5–6.4× ([Capitalpad](https://capitalpad.com/lower-middle-market-ebitda-multiples/)).
- No Kenyan or East African agro-processing transaction multiple was found.

**Exit routes** [judgement]: a trade sale to a feed strategic (Nutreco/Skretting via Tunga, De Heus, Victory Farms/SamakGro); a trade sale to an edible-oil refiner; a regional agri-trader; a PE secondary. An NSE listing is unrealistic at a USD 17m EV.

| Exit assumption | Equity IRR |
|---|---|
| 4× | 14.0% |
| 5× (base) | 15.5% |
| 7× | 18.1% |
| No exit value | 4.7% |

**Interim liquidity.** Distributions begin in 2031 and total KES 2.3bn over 2031–38. Equity payback is 2037.

---

## 14. ESG and development impact

### 14.1 Material E&S issues and the action plan

| Issue | Risk | Management (IFC Performance Standards-aligned, as DFI lenders will require) |
|---|---|---|
| Lake Victoria cage expansion | The plant's feed demand depends on cage growth that faces pollution and tourism objections and fish kills ([KNA, 1 Oct 2026](https://www.kenyanews.go.ke/pollution-blamed-for-mass-fish-deaths-in-l-victoria/); [People Daily](https://peopledaily.digital/news/lake-victoria-fish-cage-crisis-senate-launches-probe-over-pollution-blocked-beaches-and-tourism-losses)) | Sell only to licensed farms in designated zones; promote low-phosphorus, high-digestibility feeds and FCR advisory; support KMFRI zoning and carrying-capacity work; publish feed-to-fish conversion data |
| Effluent and air | Refinery effluent (oil and grease, BOD, soapstock); boiler emissions | ETP (DAF plus biological; KES 40–80m budget [ESTIMATE]); effluent discharge licence; 6-monthly returns |
| Boiler fuel sourcing | Fuelwood can drive deforestation | Briquettes and agri-residues with chain-of-custody; sunflower hulls from Phase 2 (about 48% of steam need) |
| Food and feed safety | Aflatoxin (a carcinogen) in feed passes up the food chain; vitamin A fortification | Lot testing; release limits; fortification compliance |
| Hexane (Phase 2) | Fire and explosion | Hazardous-area design; experienced operator; DOSH; emergency plan |
| Smallholder contracts | Debt traps, side-selling disputes, price risk to farmers | Seed-only credit; transparent floating price with a floor; grievance mechanism; no exclusivity penalties |
| Labour | About 70 jobs (115 with Phase 2) plus field staff | Statutory wages and above; OSH; contractor standards |
| Land | Change of user; community claims | Industrial-zoned plot; title due diligence; no involuntary resettlement |

### 14.2 Development impact (indicative; [ESTIMATE] unless stated)

- **Smallholder income.** About 4,500–9,000 contracted farmers by 2031 (section 5.3), paid by mobile money at harvest. Seed gross revenue at the KES 52k/t contract price is about KES 0.15bn in 2031 (2026 KES). Phase 2's larger outgrower base is not in the v2.0 base case.
- **Import substitution.** About 3.2 kt of oil a year in Phase 1, worth about USD 4–5m a year at landed parity, plus about 9 kt of non-GM cake and meal. Both are small against national totals (under 0.5% of oil consumption).
- **Fish-feed access.** Locally made, tested floating feed for small and mid-size cage farmers, who face feed at more than 60% of production cost ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back)). FCR improvements lower both cost and lake nutrient loading.
- **Jobs.** About 70 direct jobs in Phase 1 (about 115 if Phase 2 were built), plus 6–10 extension staff and indirect jobs in aggregation and haulage.
- **Nutrition.** Vitamin A-fortified oil for the institutional segment.
- **Measurement.** A randomised outgrower pilot would give credible impact evidence, valuable to DFIs and grant funders. That is not enough to justify the commercial investment.

---

## Appendix A. Key assumptions and sources

All inputs, with low, base and high values, are on the Assumptions sheet of `model/financial_model.xlsx`. The selection below lists 2026 KES unless stated.

| Parameter | Low | Base | High | Source / status |
|---|---|---|---|---|
| KES/USD 2026; depreciation per year | 129.4; 2% | 129.8; 4% (+1.5 points in 2027) | 130.0; 7% | [Kenya Times, 15 Oct 2026](https://thekenyatimes.com/business/kenyan-shilling-holds-firm-as-forex-reserves-drop-by-221million/); depreciation [ESTIMATE] |
| Phase 1 crush / refinery / extrusion | – | 50 t/d / 15 t/d / 3 t/h | – | [technical_operations.md §5](research/technical_operations.md); refinery resized [ESTIMATE] |
| Phase 2 crush / added extrusion / added refinery | 75 / 0 / 10 | 100 t/d / +3 t/h / +20 t/d | 150 / +6 / +40 | Resized from the 150 t/d spec [ESTIMATE] |
| Soy share of seed | 15% | 30% | 40% | [technical_operations.md §5.2](research/technical_operations.md) [ESTIMATE] |
| Sunflower oil yield, full press | 27% | 31% | 34% | [technical_operations.md row 3](research/technical_operations.md); COSTECH [DATED] |
| Phase 2 solvent uplift | +5 pts | +7 pts | +9 pts | [technical_operations.md row 6](research/technical_operations.md) |
| Soy oil yield (extruder-expeller) | 10% | 12% | 14% | [ESTIMATE] |
| Seed supply path, 2029–38 | ×0.70 | 8 → 32 kt potential | ×1.25 | [feedstock_supply.md §9](research/feedstock_supply.md), extended [ESTIMATE] |
| Delivered sunflower, blended | ×0.79 | 52.3k → 57.6k KES/t | ×1.26 | [feedstock_supply.md §8–9](research/feedstock_supply.md) [ESTIMATE] |
| Delivered soybean | 60k | 75k | 100k | [feedstock_supply.md row](research/feedstock_supply.md) [ESTIMATE] |
| Seed price pass-through of oil+cake value | 0 | 50% | 80% | [ESTIMATE]; contract design per [feedstock_supply.md §4.2](research/feedstock_supply.md) |
| Crude oil to refiners = oil price index | 155k | **175k** (v1.1: 190k) | 200k KES/t | Reconciled CPO landed parity [CONFLICT resolved, [round1_evidence.md §2.1](research/round1_evidence.md)] |
| Refining spread (refined = crude + spread) | 40k | **65k → refined 240k** (v1.1: independent 264k) | 90k KES/t | Landed-parity band 219–269k; 2022 jerrican cross-check ~242k [ESTIMATE, [round1_evidence.md §2.2](research/round1_evidence.md)] |
| CPO duty protection × probability lost | 12k | 15k × 60% | 18k | [regulatory_tax_risk.md §7](research/regulatory_tax_risk.md) |
| Sunflower cake | 32k | 40k | 50k KES/t | Jiji listing [UNVERIFIED]; [DATED] series |
| Non-GM soybean meal (bought) / own soy cake | 80k / 65k | 95k / 85k | 120k / 100k | Indexbox [UNVERIFIED]; [ESTIMATE] |
| Grow-out feed / starter feed (`feed_px_mult` ×0.88 / ×1.00 / ×1.20) | 110 / 176 | 125 / 200 | 150 / 240 KES/kg | SamakGro list (undated); WorldFish; starter [ESTIMATE] |
| Real feed price decline from 2029 | 0% | **1%/yr** (v1.1: 0) | 3%/yr | Competitor response [ESTIMATE, [round1_evidence.md §1.3](research/round1_evidence.md)] |
| Feed dealer margin; new-entrant discount | 0%; 0% | 5%; 5% (years 1–2) | 10%; 10% | [ESTIMATE] |
| Contestable Kenyan merchant aquafeed SAM 2026; growth | 15 kt; 4% | **25 kt** (v1.1: 45 kt incl. UG/TZ); 8% | 37 kt; 14% | Build-up in [round1_evidence.md §1.2](research/round1_evidence.md) [ESTIMATE] |
| Uganda/Tanzania demand added to SAM | 0 | **0** | 12 kt | Upside only [ESTIMATE] |
| Maximum feed share of SAM | 8% | 15% | 25% | [ESTIMATE] |
| Refined share of crude for sale | 50% | 80% | 95% | [ESTIMATE] |
| Starter share of feed tonnes | 5% | 15% | 25% | [ESTIMATE] |
| Grid electricity | 16 | 20 | 25 KES/kWh | EPRA 2023 [DATED] plus 2026 pass-throughs |
| Labour, Phase 1 | 50 | 61 | 80 KES m/yr | [technical_operations.md §4.3](research/technical_operations.md) |
| Maintenance | 2.5% | 3.5% | 5% of equipment | [technical_operations.md row 33](research/technical_operations.md) |
| Phase 1 / Phase 2 capex | ×0.70 | USD 9.49m / 15.25m | ×1.45 | [technical_operations.md §4.1](research/technical_operations.md) [ESTIMATE, ±40%] |
| Phase 0 development, total (0a + 0b; expensed in 2027 in the FID case) | 0.6 | 0.8 | 1.0 USD m | [financing_capital.md §6](research/financing_capital.md) |
| Senior rate / tenor / grace | 14% / 5y / 12m | 15.5% / 7y / 18m | 17.5% / 8y / 24m | [financing_capital.md rows 5–6](research/financing_capital.md) [ESTIMATE] |
| Mezzanine (USD) | 11% | 13% plus WHT gross-up | 16% | [financing_capital.md row 9](research/financing_capital.md) [ESTIMATE] |
| DSCR sizing and lock-up | 1.20 | 1.30 | 1.40 | [financing_capital.md row 14](research/financing_capital.md) |
| Lender downside haircut on CFADS for sizing; first test year | 0%; 2030 | **20%; 2030** | 30%; 2031 | [ESTIMATE] R1-02 |
| Default covenant; waiver fee; cash sweep in lock-up | 1.05×; 0%; 0% | 1.10×; 1%; 50% | 1.20×; 2%; 100% | [PK-UNVERIFIED] |
| Founder guarantee of senior shortfall; GM equity | 0; 0% | 100%; 4% | 100%; 5% | [financing_capital.md §2](research/financing_capital.md) [PK-UNVERIFIED]; plan §8.2 |
| Phase 2 DFI loan: share / rate / tenor | 45% / 13% | 55% / 14% / 9y | 60% / 16% | [financing_capital.md §6](research/financing_capital.md) |
| CIT; investment deduction | 10% (SEZ); 50% | 30%; 100% | 30%; 100% | [regulatory_tax_risk.md rows 1–3](research/regulatory_tax_risk.md) |
| Irrecoverable feed VAT (operating inputs only); feed levy | 1%; 0 | 2%; 0.5% | 3.5%; 1% | [ESTIMATE] |
| Finished feed VAT-exempt (capex VAT apportioned) | 0 | **1** | 1 | [regulatory_tax_risk.md row 19](research/regulatory_tax_risk.md) [CONFLICT] |
| Minimum tax: rate; probability from 2028 | 0; 0 | **1%; 25%** | 1%; 100% | [round1_evidence.md §3](research/round1_evidence.md) [ESTIMATE] |
| Exit multiple | 4.0× | 5.0× | 7.0× | [financing_capital.md row 27](research/financing_capital.md) [ESTIMATE] |
| WACC | – | **Computed from the modelled structure: 32.3%** | – | Equity at 35%; the financing file's 23% / 16.5% (which assumed 50% equity) kept as memo items only |
| Early-failure probability; late-failure probability (of survivors); liquidation recovery; P(Phase 2 go, if the gate passes) | 15%; 5%; 20%; 30% | 30%; **10%**; 35%; 50% | 45%; 15%; 50%; 70% | Judgement, anchored on the [screening report](../../reports/Profitable%20business%20opportunities%202026.md) |
| Phase 0a; Phase 0b; expected pilot seed loss | 0.2; 0.4; 0.02 | 0.3; 0.5; 0.05 | 0.4; 0.7; 0.10 USD m | [ESTIMATE] R1-05 |
| Seed safety stock; bad debts | 0.5 mo; 0.25% | 1.5 mo; 0.5% | 2.5 mo; 1% | **Modeller's judgements, not in the research** |

---

## Appendix B. Evidence-quality notes

| Input | Grade* | Comment |
|---|---|---|
| Edible-oil import volumes and bill | B | Official AFA and USDA series exist, but conflict by ±25%; bill estimates range KES 100–160bn [CONFLICT]. This does not drive returns |
| Cage output growth | B | KNBS via secondary press; the Victory Farms share is unresolved [CONFLICT]. **This drives the feed SAM** |
| Merchant aquafeed market size and share | **C** | Derived in round 1 as non-VF cage output × FCR net of VF-linked supply, plus ponds. Victory Farms' Kenya-only output is inferred from two press reports [CONFLICT]. No survey. **The decisive unknown** |
| Feed prices | C | Undated retail list and a WorldFish farm-level range; no ex-mill or distributor quote. **The 37% margin sits on this** |
| Seed volumes and delivered cost | **C** | National statistics conflict by up to 10×; delivered cost is a build-up estimate; no side-selling data |
| Oil prices (crude and refined, local) | C | Import parity is reasonably sourced (B), but the duty on refined imports is [CONFLICT] (25%, 35%, or 25% with a USD 500/t floor). No 2026 20 L quote and no public local-crude price |
| Cake and meal prices | C | Mostly [DATED] or marketplace listings |
| Capex | C | Bottom-up estimate (±40%); listings, not quotes; comparators are full-scope (Mainland USD 28m, De Heus USD 25m) |
| Process yields | C | International or older literature; Kenyan seed oil content unmeasured |
| Tax and duty regime | B | Statutes cited through practitioner summaries; several [CONFLICT]s (deduction threshold, feed VAT, IDF/RDL, CPO duty status) |
| Policy probabilities | C | Judgemental, informed by event history |
| Debt terms | **C/D** | `financing_capital.md` rests on **one** web search. Most terms (rates, tenors, guarantees, 125–150% collateral cover, AGF and TCX terms) are [PK-UNVERIFIED] prior knowledge. No disclosed term sheet for any Kenyan agri DFI deal |
| Minimum tax status | B | Court history [DATED]; MTRS commitment (IPF, 2025); Finance Bill 2026 summaries (search extracts) |
| Exit multiple | C | No Kenyan comparables; US LMM benchmarks with a country discount |
| Failure probability | C | The screening report's illustrative 30%; Kenyan survival data are dated and micro-firm-based |

*A = audited or regulator data at a close comparable; B = sourced market data with some conflict; C = estimate, listing or inference.

**General caveats.**
- Most web sources were read through search-result extracts only.
- KNA page dates are often crawl dates, not publication dates.
- Every comparable is a survivor (Victory Farms, Agventure); failures are not reported, so the evidence base is biased upward ([screening report](../../reports/Profitable%20business%20opportunities%202026.md)).
- **Not modelled:** the SEZ route; VAT refund delays; eTIMS disallowance of informal seed purchases; EAC duty remission (upside); dilution or accretion from outside Phase 2 equity; acquisition or JV alternatives; a right-sized 2 t/h extruder; a monthly cash model (the model is annual with a seasonal profile).
- **The VOI priors are judgement.** Under independent priors no simulated state passes. The conclusion is robust to a 0.5 correlation among favourable outcomes, but not to a founder prior that is much more optimistic than the research ranges.
- **The model treats the Phase 2 gate with perfect foresight** of each scenario's prices. In practice the decision is made under uncertainty.

---

## Appendix C. Items to verify in due diligence

**Market and commercial**
1. Victory Farms' **Kenya-only** output (The Star's "1,400 t/month" read as Kenya or group [CONFLICT]) and its share of KNBS cage output; SamakGro's sales to VF-linked farms; whether Doho sells surplus feed in Nyanza. **This single fact decides whether the contestable market is nearer 15 kt or 37 kt.**
2. Ex-mill and distributor prices for grow-out and starter feed from Tunga/Fugo, SamakGro, Aller Aqua/AquaRech and De Heus; dealer margins; credit terms.
3. Utilisation and pricing behaviour of Tunga (45 kt), SamakGro's new 8 t/h plant and De Heus Njeru.
4. Prices refiners pay for local crude sunflower oil; crude quality specification.
4a. **20 L wholesale and institutional prices** for palm olein and sunflower oil in Kisumu (schools, hotels, wholesalers), and the **current KRA duty on refined oils** (HS 1511.90.30, 1512.19): 25%, 35%, or 25% with a USD 500/t floor.
5. A 2026 price sheet for cake and meal from AKEFEMA members or Rift millers.
6. Tilapia farmgate prices (farmers' ability to pay for feed).

**Feedstock**
7. AFA Nuts and Oil Crops Directorate data and county reports on sunflower and soy area and yield in 2025–26.
8. Measured oil content of hybrid seed from target counties; aflatoxin incidence by origin.
9. Tanzania's 10% export levy: enacted or proposed? Any Ugandan restrictions.
10. WRS eligibility of sunflower and soy; availability of collateral managers in western Kenya.

**Technical**
11. Three written quotes per package with defined scope, CIF Mombasa; references for Famsun/Muyang twin-screw lines in East Africa.
12. Kenya Power connection lead time and cost at the chosen site; grid reliability.
13. KS 2289-1 contents (aflatoxin, fibre, moisture); the KEBS edible-oil standard number; whether KEBS certification is mandatory for fish feed.
14. 2026 biomass and briquette prices and sustainable supply.

**Regulatory and tax**
15. The current CPO duty rate and the status of any appeal against the 27 November 2025 judgment (COFEK).
16. The Court of Appeal GMO judgment date and any Supreme Court route.
17. The investment-deduction threshold (KES 250m / 1bn / 2bn) for a KES 1.4bn plant outside Nairobi and Mombasa.
18. A KRA private ruling: VAT status of finished feed (exempt or zero-rated); recovery of input VAT.
19. Whether the AFA 4% import levy applies to raw seed imported by a non-SEZ crusher.
20. IDF/RDL rates and any manufacturer concessions; CGT rate; **minimum tax**: any Finance Bill 2027 proposal under the MTRS.
21. The Livestock Bill 2026 text (feed levies, registration); the Food and Feed Safety Act 2026 obligations.
22. The outcome of the Senate cage inquiry; the aquaculture levy appeal.
23. eTIMS reverse-invoicing mechanics for smallholder seed purchases.
24. SEZ domestic-sale customs treatment (only if the SEZ route is considered).

**Financing and legal**
25. Indicative terms from AgDevCo (including AgDevCo Ventures' appetite for mezzanine and a KES option), two banks (with IFC, BII or AGF risk-sharing) and a collateral manager. Required guarantee and collateral cover; whether mezzanine would allow 3 PIK years.
26. Land title, change of user, the Land Control Board, and the PropCo lease structure under Article 65.
27. Kenyan or regional agro-processing M&A multiples; strategic interest from feed multinationals.

**Model**
28. Independent review of `model/model.py`: tax computation (including minimum tax), the downside debt-sizing loop, the cure/sweep iteration, the four-branch survival tree, the VOI Monte Carlo and the gate calibration. Gate (a) still uses the assumed supply path.

---

## Revision log

### Round 1 (v1.1 → v2.0, 19 October 2026)

This round responds to `reviews/review_round_1.md`; the per-issue responses are in `reviews/response_round_1.md`. New evidence is in [research/round1_evidence.md](research/round1_evidence.md). The model was re-run after every change.

**Net effect on the headline.**
- Conditional equity IRR: 28.9% → 15.5%.
- Survival-weighted IRR: 22.3% → 8.9%.
- Project IRR: 26.1% → 15.3%, against a WACC of 32.3% (previously compared with 23%).
- Recommendation: "fund a USD 0.8m Phase 0 option" → "stop; at most a USD 50k desk check".
- Section 9.8 bridges the two versions.

| Issue | Change |
|---|---|
| R1-01 (major) SAM and K1 | `sam_2026` rebased from 45 kt (Kenya plus Uganda and Tanzania) to the contestable Kenyan merchant market, 25 kt (15–37), net of Victory Farms' captive feed and SamakGro's VF-linked sales. Victory Farms' Kenyan output reconciled with KNBS (about 45–60% of cage output). Uganda and Tanzania moved to an upside scenario (`sam_regional`). Added a 1%/yr real feed price decline in the base (`feed_real_decline`) and a competitor-response scenario at 3%/yr plus a 10% entrant discount. K1 reset to 24 kt in model units, calibrated to the hurdle; the covenant break-even is 26.7 kt (§2.3, §12.2) |
| R1-02 (major) Covenants | Senior debt sized on a lender downside case (CFADS ×0.80 at 1.30×); the base now carries no senior debt. Modelled consequences of a breach: cure equity below 1.10× (prepays senior), a waiver fee, and a 50% cash sweep in lock-up. Every scenario and tornado row reports minimum DSCR, cure equity and peak equity. New FID test D1 on debt capacity. Alternative lender structures reported (§9.4, §9.5, §9.6, §10.1, §12.2) |
| R1-03 (major) Refined price | Landed-parity table for RBD olein (three duty cases, plus duty-free and misdeclared imports), refined sunflower and local CPO refiners, with a 2022 jerrican cross-check. Refined price is now crude plus a refining spread (base 240k against the unlinked 264k), so oil prices and seed move together. Refined price added as kill test K11 (212k/t). 20 L quotes and the refined-oil duty line made due-diligence items. The duty [CONFLICT] (25%, 35%, or 25% with a USD 500/t floor) is flagged (§2.1) |
| R1-04 (major) WACC and gate (d) | WACC computed from the modelled structure (32.3%); the financing file's 23% is now a memo. The "Clears WACC" verdict is reversed. Gate (d) now tests Phase 2's incremental equity NPV at 35%; the funding-mix WACC (21.1%) is reported for the project view. Phase 2 is a no-go in the base (§1, §9.4) |
| R1-05 (major) Phase 0 | Value-of-information Monte Carlo (150 draws × 2 priors): stop, invest, Phase 0a, staged, perfect information. Every Phase 0 policy is worse than stopping. Phase 0 restaged: an optional desk check (≤ USD 50k), then 0a (USD 0.3m), then 0b (USD 0.55m), with stop gates. The pilot is cut to 500–600 ha with a named back-to-back buyer and budgeted seed working capital. Restructure alternatives modelled (feed-mill-first 9.6%; crusher-only 1.5%) or assessed (acquisition, JV, redeploy) (§12.5–12.7) |
| R1-06 Ask and FX | The ask is shown by stage, net of Phase 0, each at a stated FX year. Peak equity is converted at the FX of its own year (§1, §10.3) |
| R1-07 Oil parity conflict | [CONFLICT] flagged and reconciled (CPO FOB about USD 1,100; landed KES 177k). Base crude set at the lower, CPO parity of KES 175k (§2.1) |
| R1-08 Minimum tax | Added to the model (25% probability from 2028, expected value), the tornado (certain: equity IRR 15.1%, minimum DSCR 0.67) and the risk register (risk 11) |
| R1-09 Capex VAT | Capex VAT apportioned by the exempt (feed) turnover share; KES 93m is now irrecoverable. The 2% leakage now covers operating inputs only (§7.2) |
| R1-10 Gate calibration | Every kill threshold marked † is calibrated in the model (`calibrate_gates()`). G1(b) raised to at least 9 kt at a 30% or higher margin. Tripwires updated (§12.2–12.4) |
| R1-11 Survival tree | Late-failure branch added (base operations to 2034, liquidation in 2035; 10% of survivors). Bond comparison redone on survival-weighted, after-shareholder-tax founder flows: −KES 479m at 12.25% (§9.7) |
| R1-12 Financing realism | GM's 4% equity modelled (founder IRR). Founder personal guarantee modelled in the failure branches and added to the risk register (risk 12) with collateral cover. Evidence basis of the financing file disclosed (Appendix B). AgDevCo Ventures noted. TCX-hedged KES pricing flagged as optimistic (§10.1) |
| R1-13 Wording | 2030 is the first full operating year and 2031 the first steady-state year (§9.1) |

**Model code changes (`model.py`):**
- new inputs: `sam_regional`, `feed_real_decline`, `feed_px_mult`, `refine_spread`, `p_feed_exempt`, `min_tax_rate`, `p_min_tax`, `sizing_haircut`, `dscr_first_year`, `default_dscr`, `waiver_fee`, `sweep_share`, `pg_cover`, `gm_equity`, `p_late_fail`, `late_fail_year`, `phase0a_usd`, `phase0b_usd`, `pilot_seed_loss_usd`, `config`;
- `p_refined` removed (now derived from crude plus the spread);
- senior debt schedule with prepayments;
- waterfall with cure and sweep, iterated to convergence;
- `wacc_model`;
- four-branch survival tree;
- new functions `voi_analysis()`, `calibrate_gates()`, `g1_calibration()` and `joint_cases()`;
- new scenarios and tornado rows;
- new workbook sheets "Phase 0 VOI" and "Gates & break-evens", and `voi_draws.csv`.

### v1.1 (19 October 2026, before review)

- **Gate-year cash.** The waterfall retained gate-year cash for Phase 2, instead of distributing it and re-injecting equity. Equity IRR fell from 29.4% to 28.9%.
- **Exit EV.** Exit EV was floored at zero.
