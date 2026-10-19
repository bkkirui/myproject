# Kisumu oilseed crushing and extruded aquafeed mill: business plan

**Prepared:** 19 October 2026. **For:** the investor-founder and prospective DFI or bank credit committees.
**Status:** draft v1, written for independent adversarial review. It is not an offering document.

**Conventions**
- Every factual claim carries an inline link to the source as cited in the specialist research files in `research/`. Most of those sources were read only through search-result extracts, because direct page fetches failed with DNS errors. Each therefore needs checking against the primary document before capital is committed.
- **[ESTIMATE]** marks an analyst figure, with its reasoning given or referenced. **[DATED]** marks a source from before 2025. **[CONFLICT]** marks sources that disagree. **[UNVERIFIED]** marks a weak or secondary source.
- Financial figures come from the model (`model/model.py`, outputs in [model/outputs.md](model/outputs.md)). They are nominal KES unless stated. The value date is 2027. FX starts at KES 129.8/USD and depreciates 4% a year, plus an extra 1.5 points in 2027.
- **Model correction made while writing this plan.** The model's cash waterfall paid a KES 424m dividend in 2031 and then called KES 424m more equity in 2032 to build Phase 2. No board would do that, and it flattered equity IRR by 0.4 points. A second fix stops a negative EBITDA from producing a negative exit value. Both are fixed in `model.py` and the model was re-run. All figures below are the corrected outputs; the effects are listed in section 9.7. Base equity IRR moves from 29.4% to **28.9%** and the survival-weighted figure from 22.4% to **22.3%**.

---

## 1. Executive summary

**What and where.** An integrated plant at peri-urban Kisumu, 60–130 km from the Lake Victoria cage-farming clusters in Siaya and Homa Bay ([technical_operations.md §6](research/technical_operations.md)).
- **Phase 1** (FID Q4 2027, operations from about April 2029): 50 t/day of multi-seed crushing (70% sunflower, 30% non-GM soy), a 15 t/day refinery that fortifies with vitamin A, and a 3 t/h twin-screw line making floating fish feed.
- **Phase 2** (gate tested on 2031 results, built in 2032): crushing rises to 100 t/day with dehulling and solvent extraction, plus a second 3 t/h extrusion line and 20 t/day more refining.

**The thesis, stated honestly.**
- The headline story is a crusher selling into a KES 100–130bn edible-oil import gap ([People Daily, Feb 2025](https://peopledaily.digital/business/trade-cs-lee-kinyanjui-pushes-for-local-alternatives-to-slash-ksh100b-edible-oil-imports/amp); [The Standard, 2025](https://thestandard.ke/sports/business/2001515437/edible-oil-processors-rekindle-push-to-scrap-import-duty-tax); [CONFLICT]). The economics are different. **Extruded fish feed is the business.**
  - In the first full year (2031) feed is about 60% of revenue and about 64% of combined crush and feed gross margin (refining margin excluded), at a modelled feed gross margin of 37%.
  - The crush margin is thin (KES 20k per tonne of seed in 2026 KES) and exposed to policy.
  - The crusher's job is to give the feed line secure non-GM protein and to sell surplus oil and cake.
- Seed supply, not oil demand, is the binding constraint. Kenya's recorded sunflower output is 6–30 kt a year, against a Phase 1 need of about 13.5 kt ([feedstock_supply.md §1](research/feedstock_supply.md)).

**How much.**

| Item | Value |
|---|---|
| Phase 1 capex | USD 9.5m (range 6.6–13.8) = KES 1.40bn as spent |
| Phase 1 total funding, including working capital and pre-operating costs | KES 2.24bn (USD 15.7m) |
| Phase 2 capex | USD 15.3m = KES 2.90bn |
| Peak net equity, whole plan | KES 1.99bn (about USD 13.5m) |
| Peak project funding need | KES 3.31bn |

**Returns against the hurdles** (base case, KES; [model/outputs.md §6, §9](model/outputs.md)):

| Measure | Base | Hurdle or benchmark | Verdict |
|---|---|---|---|
| Project IRR (KES / USD) | 26.1% / 21.2% | Phase 1 WACC 23% | Clears: project NPV at 23% is +KES 423m |
| Equity IRR, conditional on survival (KES / USD) | 28.9% / 24.0% | Greenfield: 35–40% expected, about 45–50% conditional on survival | **Fails** |
| Equity IRR, survival-weighted (30% failure probability) | 22.3% | Greenfield 35–40% | **Fails by 13–18 points** |
| Equity NPV at 35% / 40% | −KES 374m / −556m | 0 | Fails |
| Equity NPV at the 12.25% tax-free infrastructure bond | +KES 3.43bn | 0 | Clears comfortably |
| Equity IRR without exit value | 14.6% | — | **The 2038 exit carries most of the return** |

**Key risks, in rank order:**
1. Feed price and market share, in a regional aquafeed market that is over-supplied (Tunga 45 kt, SamakGro 8 t/h, De Heus 50–100 kt), where Victory Farms makes about 90% of its own feed.
2. Delivered seed cost and volume.
3. Capex overrun.
4. Policy reversals: the CPO duty was already struck down in November 2025, the GMO import ruling is pending, and duty-free import waivers recur.
5. Execution by a founder without sector operating experience.
6. Social licence for cage farming on Lake Victoria (a Senate inquiry opened in October 2026).
7. The election on 10 August 2027.

The single biggest swing is seed cost: equity IRR runs from 38% to 14% across the research range.

**The ask.**
- **Now:** USD 0.8m of Phase 0 development spending (Q4 2026 to Q3 2027) to buy information.
- **Conditional on passing the FID tests:** USD 9.0m of Phase 1 equity, a USD 1.4m standby equity letter, a KES 416m senior loan, USD 1.7m of mezzanine and a seasonal stock-finance line.
- **Conditional on the Phase 2 gate:** about KES 0.7bn of equity, or preferably outside equity, plus a KES 1.6bn DFI loan.

**Recommendation.**
- **Do not commit to Phase 1 on current evidence.** The base case misses the greenfield hurdle under any failure probability: even with zero failure risk the expected equity IRR is 29.3%.
- **Fund Phase 0 as a paid option.** It costs about 9% of Phase 1 equity (6% of peak equity) and tests the four inputs that move the answer most: feed price, feed market share, seed cost and capex. Supplementary runs of the model (section 9.6) show that the survival-weighted IRR clears 35% (35.8%) only if three things happen together: a 10% better feed price, 10% cheaper seed and 15% lower capex, **and** failure risk cut from 30% to 20% or less.
- **Go/no-go gates:**
  - **G0 (FID, Q4 2027):** the quantitative kill and proceed tests in section 12.
  - **G1 (Phase 2, on 2031 audited results):** at least 24 kt of seed *contracted* for 2035, at least 8 kt of feed sales at a gross margin of at least 20%, at least 70% of crude oil refined under the own brand, and positive incremental NPV at 16.5%.
  - **Operating tripwires in 2030:** a debt-service cover ratio (DSCR) below 1.10x, or feed sales below 4 kt.
- **Phase 2 is an option, not part of the base thesis.** Phase 1 alone returns a higher equity IRR (29.7%) and depends far less on exit value: 21.3% without the exit, against 14.6% for the full plan.

---

## 2. Market opportunity

### 2.1 Edible oil

**Size and import dependence.**
- Palm oil is more than 90% of Kenyan oil and fat consumption. USDA puts palm imports at 875 kt in 2024, heading for 1.05 Mt in 2025/26, of which 90–100 kt is re-exported ([OFI Magazine](https://www.ofimagazine.com/news/kenyan-palm-oil-consumption-to-reach-record-high); [Milling MEA/USDA, Jul 2025](https://millingmea.com/kenyas-palm-oil-imports-to-hit-1-05-million-tonnes-in-2025-2026-usda/)).
- AFA's quarterly data show 183,139 t of edible oils worth KES 25.6bn imported in the quarter to June 2025, including only 3,909 t of sunflower and 1,671 t of soy oil ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)).
- **[CONFLICT] Volume.** AFA and the Ministry say about 600 kt is consumed ([The Star, Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)). USDA palm imports alone are about 1 Mt. The research base for food-grade oils and fats is **about 780 kt in 2026**, or about 14 kg per person [ESTIMATE, [market_demand.md §1.1](research/market_demand.md)].
- **[CONFLICT] The import bill.** KES 100bn ([People Daily, Feb 2025](https://peopledaily.digital/business/trade-cs-lee-kinyanjui-pushes-for-local-alternatives-to-slash-ksh100b-edible-oil-imports/amp)), KES 130bn for CPO ([The Standard](https://thestandard.ke/sports/business/2001515437/edible-oil-processors-rekindle-push-to-scrap-import-duty-tax)) and KES 145bn ([The Star, Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)) are all cited.
  - The research's base is about KES 105–115bn in 2025, rising to KES 120–135bn in 2026 [ESTIMATE]. The FAO vegetable-oil index was up 18.3% year on year in September 2026 while volumes held flat ([Fastmarkets/FAO](https://fastmarkets.com/insights/fao-food-price-index-rises-in-september-on-higher-cereal-vegoil-prices-and-benchmark-at-highest-since-november-2022)).
  - The 2023 figure was 720 kt worth KES 98.9bn ([The Star, Mar 2024](https://www.the-star.co.ke/news/infographics/2024-03-27-state-turns-to-local-production-to-cut-sh160bn-edible-oil-import-cost), [DATED]).
- **Local oil from local seed is under 5% of consumption** (below 30–50 kt) [ESTIMATE, [market_demand.md §1.1](research/market_demand.md)]. Bidco needs more than 10 kt a year of local seed but gets about 5 kt ([KNA](https://www.kenyanews.go.ke/?p=23808), date uncertain).
- **Policy push.** In March 2026 the government relaunched a sunflower and soy drive, aiming to halve imports between 2026 and 2030 ([KNA, Aug 2026](https://www.kenyanews.go.ke/sunflower-soybean-initiative-to-curb-edible-oil-import-bill/)). AFA's KES 981m Edible Oil Crops Promotion Project targets 50% local supply by 2028 ([Milling MEA](https://millingmea.com/kenya-accelerates-edible-oil-crops-farming-to-cut-imports-led-by-afa/)).
  - That target is not credible. Even 81,000 ha at 1 t/ha gives about 81 kt of seed, which is about 5% of demand [ESTIMATE, [feedstock_supply.md §5](research/feedstock_supply.md)]. The value of the policy lies in seed distribution and extension, which the plant can use.

**Prices (Sep–Oct 2026).**
- Retail salad oil averaged KES 358.09/L in July 2026, close to the September 2022 peak of KES 379.84 ([Business Daily](https://www.businessdailyafrica.com/bd/economy/cooking-oil-prices-climb-back-to-highs-of-2022-crisis-5548020)).
- KNTC's state-linked "Mama Pima" loose oil sells at KES 185/L wholesale and KES 210/L retail ([Kenya Times, Jul 2026](https://thekenyatimes.com/business/govt-unveils-mama-pima-cooking-oil-dispenser/)). This is a ceiling for commodity oil.
- Benchmarks:
  - CPO about RM4,500–4,600/t ([Bernama](https://www.bernama.com/lite/news.php?id=2544958)).
  - RBD olein USD 1,252.5/t FOB, 8 September 2026 ([Fastmarkets](https://www.fastmarkets.com/insights/correction-to-price-for-refined-bleached-deodorized-palm-olein-on-september-8-2026/)).
  - Crude sunflower oil USD 1,265–1,275/t FOB Black Sea ([Commodity-Board](https://commodity-board.com/russia-takes-the-wheel-in-sunflower-oil-what-it-means-for-prices), [UNVERIFIED aggregator]).
- **Landed parity [ESTIMATE, [market_demand.md §1.2](research/market_demand.md)]:** CPO about KES 185k/t (KES 169/L) and crude sunflower oil about KES 209k/t (KES 190/L), duty-paid.
- **Prices modelled (2026 KES, ex-VAT):**
  - Crude sold to refiners KES 190k/t, which is 5–12% below sunflower import parity [ESTIMATE].
  - Refined bulk oil in 20 L containers KES 264k/t, equal to KES 240/L [ESTIMATE].
  - Both carry 60% of a KES 15k/t haircut for the probability that CPO duty protection is lost (section 7).
- **Refining margin.** The COMESA Competition Commission alleged that refiners sold at KES 333/L against a "fair" KES 274/L ([Khusoko, Dec 2024](https://khusoko.com/2024/12/11/oil-firms-overcharged-kenyans-by-ksh-67-7-billion/), [DATED]). The refining and branding layer has fat margins, which is why the plan refines rather than sells crude to the oligopoly.

### 2.2 Protein meal and compound feed

- **Formal compound feed** is about 2.5 Mt a year: poultry 60%, dairy 29% ([KNA](https://www.kenyanews.go.ke/?p=169703), date unconfirmed). Millers ran at 50–60% of capacity in July 2026 ([The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)). AKEFEMA warned of shortages of soybean meal, sunflower cake and canola in February 2026 ([The Star](https://www.the-star.co.ke/counties/central/2026-02-24-raw-material-crunch-threatens-to-push-animal-feed-cost-higher)).
- **Protein is the scarce input, not pelleting capacity** [ESTIMATE, [market_demand.md §3.1](research/market_demand.md)]. Demand for soy meal equivalent is about 200–300 kt a year [ESTIMATE].
- **GMO status.** A Court of Appeal conservatory order (7 March 2025) bars GM imports pending appeal ([Citizen Digital](https://citizen.digital/article/blow-to-govt-as-court-of-appeal-bars-importation-of-gmos-n358801)). Judgment was expected on 24 April 2026 but has been delayed, per a single source ([Biosafety Information Centre](https://biosafety-info.net/articles/policy-and-regulation/africa/court-of-appeal-halts-government-promotion-of-gmos-in-landmark-ruling/)). While the order holds, non-GM protein earns a premium.
- **Protein prices modelled (2026 KES/t).** These are the weakest-sourced prices in the plan:

| Input | Modelled price | Basis |
|---|---|---|
| Sunflower cake | 40k | One [UNVERIFIED] Nairobi listing ([Jiji](https://jiji.co.ke/viwandani-makadara/feeds-supplements-seeds/sunflower-seed-cake-dTh5NuF0GdsvaWJ01XlkOR3T.html)) |
| Non-GM soybean meal | 95k | Indexbox KES 90–120k/t, [UNVERIFIED] ([Indexbox](https://www.indexbox.io/store/kenya-soya-beans-market-analysis-forecast-size-trends-and-insights/)) |
| Own soy expeller cake | 85k | [ESTIMATE] |

### 2.3 Aquaculture and aquafeed

**Growth.** Cage tilapia output rose from 13,700 t in 2021 to **28,100 t in 2025** from about 7,000 cages (KNBS via [Ecofin](https://www.ecofinagency.com/news-agriculture/1703-53851-kenya-s-fish-farming-boom-draws-new-bet-from-victory-farms)). That is a 19.7% compound annual growth rate [calculation]. Total aquaculture was 33,423 t in 2024 ([The Standard](https://www.standardmedia.co.ke/counties/article/2001544285/kenya-finalises-aquaculture-policy-to-boost-fish-production)). Fish prices rose 16% in 2025 ([The Standard/KNBS](https://www.standardmedia.co.ke/business/article/2001546576/knbs-fish-vegetable-prices-jump-by-double-digits-despite-easing-inflation)).

**Physical headroom.** KMFRI estimates riparian capacity at about 275,000 t a year and 25,427 cages ([WAS 2025](https://www.was.org/Meeting/Program/PaperDetail/166835)).

**Feed demand [ESTIMATE, [market_demand.md §3.2, §4](research/market_demand.md)].**
- Cage output × FCR 1.4–1.9 gives 39–53 kt for 2025. The FCR comes from a Lake Victoria trial at 1.46–1.51 ([WAS abstract](https://was.org/Meeting/Program/PaperDetail/161632)).
- Adding ponds gives a total of about 50–80 kt in 2026 and about 125 kt by 2030 (range 75–190).

**The critical caveat: most cage feed is captive.**
- Victory Farms produces 18–30 kt a year ([The Fish Site](https://thefishsite.com/es/articles/victory-farms-raises-35-million-to-fuel-east-african-tilapia-expansion); [KNA](https://www.kenyanews.go.ke/168926-2/); [CONFLICT]) and makes about 90% of its own feed ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840)).
- The **merchant** Kenyan aquafeed market is therefore only about 20–40 kt in 2026, rising to about 45 kt by 2030 [ESTIMATE].
- This is the largest single uncertainty in the plan.

**Prices.**
- SamakGro's retail list: 4 mm finisher KES 116–130/kg, 3 mm grower KES 144/kg ([SamakGro store](https://take.app/samakgro/p/clzr0xsj9004nirjw3brif1fa), undated).
- WorldFish puts commercial feed at USD 1.00–1.24/kg and more than 60% of production cost ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back)).
- **Modelled (2026 KES):** grow-out KES 125/kg and fry/starter KES 200/kg [ESTIMATE; one 35% CP listing at KES 209/kg, [Jiji](https://jiji.co.ke/293-poultry-feed), UNVERIFIED]. A 5% dealer margin is deducted because these are retail and farm-level prices.

### 2.4 Market sizing (TAM / SAM / SOM)

| Level | Edible oil | Protein meal and aquafeed | Source |
|---|---|---|---|
| TAM | About 780 kt; about KES 156bn at wholesale | Compound feed about 2.5 Mt (KES 125–140bn); aquafeed 50–80 kt (KES 6–10bn) | [market_demand.md §5](research/market_demand.md) [ESTIMATE] |
| SAM | Soft oils a Kenyan crusher can displace: 60–100 kt (KES 12–21bn) | Merchant extruded aquafeed in Kenya and on the Ugandan/Tanzanian lake shores: 30–60 kt (KES 4–8bn) | as above [ESTIMATE] |
| **Plant (model)** | **3.4 kt crude oil in 2031; 8.2 kt in 2036–38** (about 1% of national consumption) | **9.9 kt of feed in 2031 and 17.0 kt in 2038**, which is 15% of a modelled SAM growing 8% a year from 45 kt in 2026 | [model/outputs.md §4](model/outputs.md); mass balance CSV |

**What the plant can and cannot do.**
- At full Phase 2 scale the plant would replace roughly **1% of Kenya's oil imports**. The "KES 100bn gap" is real but is not the investment case: no plausible seed base lets a single plant matter to it.
- In feed the plant needs **15% of the regional merchant market**. In Kenyan merchant terms that is about 25–50% of today's market (9.9 kt against 20–40 kt) ([technical_operations.md §8](research/technical_operations.md)). It is an aggressive share target.

### 2.5 Customer segments

| Segment | Product | Volume, 2031 (model) | Buying behaviour |
|---|---|---|---|
| Mid-size and smallholder cage farms in Siaya, Homa Bay, Busia and Migori; pond farmers | Extruded grow-out feed (3–6 mm) | 8.4 kt | Price- and FCR-sensitive; credit-constrained; buy through depots and dealers, e.g. AquaRech-type depots ([Aller Aqua](https://www.aller-aqua.com/about/news/aller-aqua-partners-with-aquarech-to-ensure-high-quality-quality-feeds-reach-all/)) |
| Hatcheries and fingerling producers | Starter and fry feed (0.3–2 mm, 35–45% CP) | 1.5 kt | Value quality and pellet size. The highest margin; currently import-dependent |
| Institutions, wholesalers, hotels and schools in western Kenya | Refined fortified sunflower oil, 20 L | 2.4 kt | Price parity to palm olein, with a modest health premium [ESTIMATE, [market_demand.md §1.4](research/market_demand.md)] |
| Refiners (Bidco, Menengai, Kapa, Pwani) | Crude oil | 0.6 kt | Oligopsony; local crude bought 5–12% below parity [ESTIMATE] |
| Dairy and layer feed millers in the Rift and Central belt | Sunflower expeller cake | 4.2 kt | Commodity buyers; prices swing with regional export bans and duty waivers |

---

## 3. Competitive landscape and positioning

### 3.1 Named competitors

**Aquafeed.** Regional capacity already several times exceeds Kenyan merchant demand ([market_demand.md §3.3](research/market_demand.md)).

| Competitor | Facts | Threat |
|---|---|---|
| **Tunga Nutrition** (Skretting/Nutreco and Unga JV; brands Skretting and Fugo), Nairobi | Extrusion capacity raised from 24 kt to **45 kt a year**, about February 2026 ([WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi)) | High: multinational formulation and brand |
| **SamakGro** (Victory Farms, Maxim Agri, Gatsby Africa), Naivasha | Sells to third parties. A new USD 3.95m, 8 t/h geothermal plant was announced in July 2026 ([The Fish Site](https://thefishsite.com/es/articles/african-aquaculture-leaders-join-forces-to-build-feed-mill-maxim-agri-victory-farms-gatsby-africa); [ThinkGeoEnergy](https://www.thinkgeoenergy.com/fish-feed-producer-invests-in-geothermal-powered-green-energy-park-in-kenya/?amp=1)) | High: low-cost power; owner of the largest cage farm |
| **Victory Farms Doho mill**, Homa Bay | KES 1.3bn extruded feed mill ([The Standard](https://www.standardmedia.co.ke/business/nyanza/article/2001549421/new-bid-to-improve-fish-production-in-homa-bay)); capacity undisclosed | High if it sells surplus feed in the plant's home market |
| **De Heus Uganda**, Njeru | 50 kt rising to "up to 100 kt"; USD 25m; opened about 2025 ([De Heus](https://www.deheus.com/csr-stories/how-a-de-heus-plant-can-support-fish-farming-in-uganda-and-help-feed-the-nation); [Ecofin](https://www.ecofinagency.com/news-industry/0509-48437-de-heus-invests-25-million-in-ugandan-fish-feed-industry); [CONFLICT on capacity]) | Medium-high: across the lake; blocks feed exports to Uganda |
| **Aller Aqua** imports via AquaRech | Depots in Kakamega, Kisii, Migori, Bondo, Homa Bay, Siaya, Busia and elsewhere ([Aller Aqua](https://www.aller-aqua.com/about/news/aller-aqua-partners-with-aquarech-to-ensure-high-quality-quality-feeds-reach-all/)) | Medium: premium imported brand; shows the distribution model |
| Unga Farm Care (Fugo), Sigma Feeds, Jewlet | Fugo launched in Homa Bay ([Aquafeed.com](https://aquafeed.com/newsroom/news/kenya-unga-farm-care-launches-fish-feed-to-improve-tilapia-business-in-homa-bay)); Sigma has made fish feed since 2010 ([Milling MEA](https://millingmea.com/sigma-feeds/)) | Low-medium |
| Kisumu Fisheries Centre of Excellence (public) | USD 19.3m, includes a feed mill ([Food Business MEA](https://www.foodbusinessmea.com/?p=2133722), date unclear) | Unknown: competitor or toll partner |

**Edible oil and crushing.**
- Bidco, Pwani, Kapa, Menengai and Edible Oil Products dominate refining, mostly of imported CPO ([market_demand.md §1.3](research/market_demand.md)). KAM puts the sector at 13 firms with 2.18 Mt of capacity ([KAM, Oct 2024](https://x.com/KAM_Kenya/status/1841742903820894410), [DATED]).
- Agventure / Pure Mountain crushes just under 10 kt a year of canola from a member and outgrower base ([CPM, Mar 2026](https://www.cpm-magazine.co.uk/wp-content/uploads/sites/9/2026/03/066-68-Kenya-March-26.pdf)).
- Regional seed competitors:
  - Mukwano in Uganda: more than 100,000 contracted farmers and 400 t/day of capacity ([Uganda Invest](https://ugandainvest.go.ug/?p=579)).
  - Mainland Group in Dodoma: USD 28m for 30–35 kt of seed ([Milling MEA](https://millingmea.com/chinese-agribusiness-giant-mainland-group-to-launch-new-sunflower-oil-plant-in-tanzania/)).
  - A USD 130m Arusha sunflower plant ([Milling MEA](https://millingmea.com/tanzania-to-establish-us130m-sunflower-processing-plant-in-arusha/)).

### 3.2 Why this plant could win, and how strong each advantage is

| Source of advantage | Mechanism | Strength |
|---|---|---|
| Secure non-GM protein | Own soy expeller cake covers almost all the feed line's soy-meal need (3.3 kt of 3.3 kt in 2031, mass-balance CSV). This de-links the plant from GMO, waiver and Zambian/Malawian export-ban shocks ([feedstock_supply.md §2.3](research/feedstock_supply.md)) | **Moderate.** The model transfers own cake at market prices, so the base IRR contains **no** integration cost saving. The value is supply security and lower working capital, plus a hedge: if GM imports are allowed, cake revenue falls but feed input costs fall too ([regulatory_tax_risk.md §4.3](research/regulatory_tax_risk.md)) |
| Proximity | 60–130 km to the cage clusters, against about 345 km from Nairobi. Saves about KES 2,200/t (about 2% of price) against Nairobi mills [ESTIMATE: 345 km × KES 6.5/t-km, [feedstock_supply.md §0](research/feedstock_supply.md)] | **Weak to moderate.** Victory Farms' Doho mill is closer still |
| Twin-screw fry and fingerling feeds | Twin-screw extrusion handles small pellets and high-fibre recipes ([technical_operations.md §3.1](research/technical_operations.md)) | Moderate, but replicable by Tunga and SamakGro |
| Farmer bundle | Cake buy-back or a feed discount for seed outgrowers, the Agventure hook ([feedstock_supply.md §4.2](research/feedstock_supply.md)) | Moderate; builds seed loyalty, not feed share |
| EAC-origin oil | Oil crushed from EAC seed should trade duty-free within the EAC, while oil refined from imported crude pays 25% ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/bidco-pushes-for-review-of-25pc-duty-rule-for-eac-exports-2120464), [DATED]) | Upside only; unverified with KRA and EAC |
| Outgrower network | Takes years to build: Agventure took more than 10 years to reach about 10 kt | **The most durable moat, if achieved.** It is also the hardest execution task |

**Judgement.** The plant enters the feed market as a regional challenger against better-capitalised multinationals and a vertically integrated market leader. It has **no strong moat in feed**: its edge is cost and service at the lake. Two things would be needed for a durable advantage:
- An outgrower base that rivals cannot quickly copy.
- Anchor offtake relationships with mid-size cage farms that are not Victory Farms.

The plan must assume competitors cut prices in response. The tornado's low feed price (KES 110/kg grow-out) gives an equity IRR of 21.1%.

---

## 4. Products and business model

### 4.1 Product mix and pricing (model base)

| Product | 2031 volume | 2031 revenue (KES m) | 2038 revenue (KES m) | Price basis, 2026 KES ex-VAT |
|---|---|---|---|---|
| Extruded grow-out feed (28–32% CP) | 8.4 kt | 1,395 | 3,614 | KES 125/kg list; 5% dealer margin and a 5% new-entrant discount in operating years 1–2 deducted |
| Starter and fingerling feed (35–45% CP) | 1.5 kt | 397 | 1,028 | KES 200/kg [ESTIMATE] |
| Refined fortified sunflower/soy oil (20 L) | 2.4 kt | 840 | 3,095 | KES 264k/t [ESTIMATE]; 5% distribution cost |
| Crude oil to refiners | 0.6 kt | 156 | 575 | KES 190k/t [ESTIMATE] |
| Sunflower cake or meal | 4.2 kt | 202 | 459 | KES 40k/t; dehulled meal 1.1× in Phase 2 |
| Surplus soy cake | 0.04 kt | 4 | 156 | KES 85k/t |
| Soapstock and acid oil | 0.1 kt | 9 | 35 | 30% of crude value |
| **Total** | | **3,004** | **8,961** | Tradables escalate with the USD-drift × FX index |

Source: `model/pnl_annual.csv`.
- **Revenue mix:** feed is 60% of revenue in 2031, falls to 46% in 2035 as Phase 2 lifts oil volumes, and recovers to 52% in 2038 [calculation].
- **Gross margin mix:** feed contributes about 64% of combined crush and feed gross margin in 2031 and about 51% in 2035, with the refining margin excluded from both [calculation from [model/outputs.md §5](model/outputs.md)]. Phase 2 therefore moves the business toward the policy-exposed crush.

### 4.2 Price linkages: how risk is shared

- **Seed.** The delivered seed price absorbs 50% of any change in the value of oil plus cake per tonne of seed. This follows the floating, parity-linked contract recommended in [feedstock_supply.md §4.2](research/feedstock_supply.md): a floor plus a share of import parity, announced before planting.
  - This is a design choice the plant must actually win from farmers. The tornado shows that with **fixed-price seed** the oil-price swing roughly doubles (equity IRR 19.2% to 32.2%).
  - Bidco's outgrowers deserted a fixed price that was below spot ([Business Daily](https://www.businessdailyafrica.com/bd/markets/bidco-taps-farmers-to-cover-edible-oil-supply-shortfall-1970404), [DATED]).
- **Feed.** Feed prices absorb 70% of changes in competitors' ingredient costs [ESTIMATE]. In practice Tunga and SamakGro set the market price and the plant follows.

### 4.3 Channel strategy

- **Feed.**
  - About half of volume goes direct to mid-size cage farms, with delivery from the plant and from a Homa Bay or Bondo depot. The other half goes through dealers and depots at about 10% margin. The model blends this to 5% of feed revenue.
  - A feed sales force and farmer extension cost 3% of feed revenue [ESTIMATE].
  - Credit terms are 21 days on average.
  - Victory Farms is **not** a target customer ([regulatory_tax_risk.md §4.5](research/regulatory_tax_risk.md)).
- **Refined oil.** Bulk 20 L containers to institutions, wholesalers and hotels in western Kenya and Uganda border towns. Branded 1 L retail is deferred; the plan avoids a supermarket brand war with Bidco.
  - 50% of crude is refined in 2029, rising to 65% in 2030 and 80% from 2031 [ESTIMATE].
  - Public-sector sales are capped at 10% of revenue because of the risk of government arrears: pending bills stood at KES 466bn in March 2026 ([Capital FM](https://capitalfm.co.ke/news/2026/06/kenya-pending-bills-sh465-87-billion-cob-march-2026)).
- **Crude oil and cake.** Monthly parity-linked pre-sales of 30–50% to refiners and to Rift and Central feed millers ([financing_capital.md §7](research/financing_capital.md)).

### 4.4 Offtake agreements: required before FID

No offtake agreement exists today. The financing file's FID conditions are signed LOIs for at least 50% of crude oil or cake and at least 8–10 kt a year of seed ([financing_capital.md §6](research/financing_capital.md)). This plan adds a third: **LOIs from at least five non-Victory cage farms for at least 5 kt a year of grow-out feed** (half of the 2031 volume), at prices consistent with a net realisation of at least KES 119/kg in 2026 KES [plan recommendation]. Possible counterparties:
- **Crude oil:** Bidco, Menengai or Kapa procurement.
- **Cake:** Rift Valley dairy and layer millers.
- **A toll or protein-supply arrangement with a multinational feed maker** (Tunga, SamakGro or De Heus), as an alternative to competing head-on ([market_demand.md §3.3](research/market_demand.md)).

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
| Seed crushed (kt) | 6.0 | 11.0 | 13.5 | 13.5 | 20.0 | 23.0 | 26.0 | 27.0 |

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

**Scale required [ESTIMATE].** At 0.9 t/ha delivered and 30% side-selling, the 2031 outgrower share (30% of 9.45 kt of sunflower) needs about 4,500 ha, or 4,500–9,000 smallholders. By 2036 (50% of 18.9 kt) it needs about 15,000 ha, or 15,000–30,000 smallholders.

**Partner.** Farm Africa's soy aggregation centres in Homa Bay serve about 6,000 farmers ([The Standard, Jul 2026](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)). They are a ready partner.

**Evidence gap.** No quantified side-selling rate exists for East African oilseeds. The model uses 15/30/50% for low/base/high [ESTIMATE]. The Phase 0 pilot (section 12) is designed to measure it.

### 5.4 Seasonality and working capital

- About 70% of seed is bought June to October. Lean-season prices are 50–90% higher ([feedstock_supply.md §7](research/feedstock_supply.md); Homa Bay middleman spread in [Nation 2026](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966)).
- The model's safety stock (1.5 months) was **calibrated by the modeller** so that peak stock is about 41% of annual crush (8.2 kt per 20 kt). That sits inside the research's 7–12 kt range.
- Year-end working capital is KES 661m in 2031 and KES 2.0bn by 2038. Peak intra-year revolver draws are KES 353m in Phase 1 and KES 1.05bn (nominal) by 2038 ([model/outputs.md §3](model/outputs.md)).
- The steady-state seasonal peak checks against the research: KES 807m per 20 kt (2026 KES), within its KES 650–950m range ([model/outputs.md §10](model/outputs.md)).

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
- **Phase 2 is smaller** than the technical file's 150 t/day and +6 t/h. Neither the seed path nor feed demand can fill the larger plant. Forced through at that specification, equity IRR falls to 25.6% and project NPV at 23% to +KES 30m ([model/outputs.md §7](model/outputs.md)).
- **No solvent extraction in Phase 1.** At 50 t/day the solvent gain of about USD 0.95m a year does not justify about USD 3m of plant plus hexane-safety risk for a first-time operator ([technical_operations.md §1.2](research/technical_operations.md)). The minimum efficient scale is above 75–200 t/day ([Missouri EM0602](https://extension.missouri.edu/media/wysiwyg/Extensiondata/Pub/pdf/energymgmt/em0602.pdf), [DATED]; [AMPC](https://www.ampc.montana.edu/documents/briefings/briefing86.pdf), [DATED]).

### 6.3 Mass balance, 2031 (Phase 1 steady state; model)

```
Seed crushed 13,500 t  = sunflower 9,450 t (full press, 31% oil) + soy 4,050 t (extruder-expeller, 12% oil)
 ├─ crude oil 3,416 t  (sun 2,930 + soy 486)
 │    ├─ to feed (mash + coating) ............ 234 t
 │    ├─ to refinery 2,545 t -> RBD 2,418 t + soapstock 127 t
 │    └─ sold crude to refiners .............. 636 t
 ├─ sunflower cake 6,048 t -> feed 1,806 t; sold to dairy/poultry millers 4,242 t
 ├─ soy cake 3,321 t       -> feed 3,281 t; sold 40 t
 └─ process losses (impurities, moisture, foots) 715 t
Feed: mash 10,172 t (own cake/oil + purchased maize, pollard, omena, cottonseed cake, premix)
      -> 9,918 t finished (grow-out 8,430 t; starter 1,488 t); 2.5% shrink
```

- Source: `model/mass_balance_annual.csv`. All closure checks pass ([model/outputs.md §10](model/outputs.md)).
- **Phase 2 steady state (2036):** 27 kt crushed (18.9 kt sunflower solvent-extracted with dehulling, 8.1 kt soy), 8.2 kt crude oil, 8.9 kt sunflower meal, 1.9 kt hulls and 14.6 kt of feed. The hulls cover about 48% of the steam need.
- Refinery use peaks at 63%. Gate (c) tests the share of crude that is refined, not refinery utilisation.

### 6.4 Feed formulation

The base grow-out formula is 29.7% CP: sunflower cake 20%, soy cake 30%, omena/fishmeal 7%, cottonseed cake 5%, maize 18%, pollard 13%, plus oil, bran and premix ([technical_operations.md §3.3](research/technical_operations.md)).
- **Raw-material cost:** about KES 72/kg blended in 2031 (2026 KES; [model/outputs.md §10](model/outputs.md)), against a cash cost of KES 88–93/kg.
- **Fibre is the binding constraint.** Ugandan trials found 15% sunflower cake best ([LRRD](https://lrrd.org/lrrd24/5/aany24084.htm), [DATED]).
- **Omena supply and aflatoxin risk** argue for a 0–3% fishmeal variant using soy, BSF or blood meal [ESTIMATE].
- **Nutritionist sign-off and KMFRI feeding trials are a Phase 0 deliverable.**

### 6.5 Utilities and energy

- **Grid power:** KES 20/kWh all-in, plus a KES 1,100/kVA monthly demand charge. Sources: the EPRA 2023 schedule ([EPRA](https://www.epra.go.ke/wp-content/uploads/2023/01/ABRIDGED-KPLC-TARIFF-2023.pdf), [DATED]) plus KES 3.87/kWh of pass-throughs in June 2026 ([People Daily](https://peopledaily.digital/business/explainer-how-epras-new-electricity-bill-will-affect-households-and-businesses/amp)).
- **Tariff risk.** Kenya Power has warned of a rise of more than 30% from county wayleave charges ([Serrari](https://serrarigroup.com/kenya-power-warns-of-30-increase-in-electricity-prices-amid-mounting-wayleave-charges-and-debt-crisis/)).
- **Energy cost 2031:** KES 76m in 2026 KES, matching the technical file's KES 76–84m.
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
| Investment deduction | 100% in year 1 (outside Nairobi and Mombasa) [CONFLICT on the KES 250m / 1bn / 2bn threshold]. If it is denied, the 50% + 25% reducing-balance regime costs **0.4 points** of equity IRR | [PwC](https://taxsummaries.pwc.com/kenya/corporate/deductions); [regulatory_tax_risk.md row 3](research/regulatory_tax_risk.md) |
| Tax losses | 5-year expiry (Finance Act 2025). None expire in the base case | [The Standard](https://thestandard.ke/sports/amp/opinion/2001528930/how-businesses-can-navigate-new-tax-loss-restrictions) |
| Foreign interest (mezzanine) | Deductible up to 30% of EBITDA, with 3-year carry-forward; 15% WHT grossed up | [Grant Thornton](https://www.grantthornton.co.ke/insights/interest-restriction-rule/) |
| VAT | Oil 16%. Feed inputs zero-rated (proposals to exempt them were dropped in 2025 and 2026). Finished feed exempt or zero-rated [CONFLICT]; 2% of feed revenue modelled as irrecoverable input VAT | [Feed Business MEA, May 2026](https://www.feedbusinessmea.com/2026/05/26/finance-bill-2026-how-proposed-tax-shifts-will-impact-feed-industry-value-chain/) |
| IDF and RDL on imported equipment | 2.5% and 2.0% | [Dawan/PwC, Jan 2026](https://www.dawan.africa/news/pwc-urges-importers-to-seek-refunds-after-high-court-strikes-down-10percent-palm-oil-duty) |
| Feed regulator levy | 0.5% of feed revenue (expected value) | [regulatory_tax_risk.md §4.4](research/regulatory_tax_risk.md) [ESTIMATE] |
| Dividends and exit | 5% dividend WHT for a resident individual; 15% CGT [UNVERIFIED] | [PwC WHT](https://taxsummaries.pwc.com/kenya/corporate/withholding-taxes) |

**Effective tax rate.**
- The 100% investment deduction defers corporate tax. **No CIT is paid until 2035.** Cumulative tax from 2027 to 2038 (KES 1.87bn) equals about 22% of cumulative pre-tax profit [calculation from `model/pnl_annual.csv`]. The rate converges to 30% and above once allowances are used.
- Shareholder taxes (dividend WHT and CGT) cut equity IRR from 28.9% to 27.5%.
- Distributed profit bears a statutory 33.5% for a resident individual ([regulatory_tax_risk.md row 28](research/regulatory_tax_risk.md)). A Kenyan HoldCo holding at least 12.5% receives dividends tax-free and defers the second layer ([regulatory_tax_risk.md §2.5](research/regulatory_tax_risk.md)).

### 7.3 Incentives and structuring

- **SEZ route (not in base).** 10% CIT for 10 years ([CDH, Feb 2025](https://www.cliffedekkerhofmeyr.com/en/news/publications/2025/Practice/Tax-Exchange-Control/tax-and-exchange-control-alert-6-february-Not-so-special-after-all-An-analysis-of-the-impact-of-the-Business-Laws-Amendment-Act-2024-on-taxation-of-Special-Economic-Zones)) and an AFA levy exemption on EAC oil crops ([The Star, Apr 2025](https://www.the-star.co.ke/news/2025-04-18-no-import-levy-on-nuts-oil-crops-from-epzs)).
  - It is worth only **+1.2 points** of equity IRR in the model, and it ignores the risk that domestic sales are treated as imports.
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

Because the base case already weights these shocks by probability, each moves equity IRR only **0.7–1.5 points** when switched fully on or off (tornado, [model/outputs.md §8](model/outputs.md)).

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
| **General Manager / CEO** | Phase 0, by month 6 | 10+ years running a crushing or feed plant in East or Southern Africa, from Bidco, Mukwano, Unga, Tunga, De Heus, ETG or similar; P&L ownership | KES 600k/month base [ESTIMATE, [technical_operations.md §4.3](research/technical_operations.md)], plus equity incentive (proposed 3–5% vesting over 4 years, [plan recommendation]) |
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
| Supply | Farm Africa, LBDA and county agriculture departments; licensed Ugandan aggregators; a WRS collateral manager | Seed and stock finance |
| Strategic co-investor (preferred) | A mid-size cage-farm group (feed offtake), a Rift feed miller (cake offtake) or a family office | Reduces failure probability and commercial risk ([financing_capital.md §6](research/financing_capital.md)) |

### 8.5 The founder's role

The founder's comparative advantages are patient equity in an equity-scarce market (Kenyan startups raised about USD 86m in Q3 2026, more than 92% of it as debt; [Business Today](https://businesstoday.co.ke/african-ventures-raise-us-674million-in-q3/)) and the ability to design and analyse evidence. Proposed responsibilities:
- Chair; capital allocation; DFI and lender relations.
- **Design and analysis of the Phase 0 experiments.** For example, randomise outgrower contract terms (floating against fixed price, with and without a cake buy-back) across farmer groups in the 2027 long rains to estimate side-selling and supply response [plan recommendation]. The model's CSVs are Stata-ready for this.
- Not day-to-day operations.

---

## 9. Financial projections

All figures are from `model/model.py` as corrected (section 9.7). They are nominal KES m unless stated. **Read IRRs as ±10 points:** most inputs are estimates and there are no binding quotes.

### 9.1 Annual summary (base case)

| KES m | 2029 | 2030 | 2031 | 2032 | 2033 | 2034 | 2035 | 2036 | 2037 | 2038 |
|---|---|---|---|---|---|---|---|---|---|---|
| Seed crushed (kt) | 6.0 | 11.0 | 13.5 | 13.5 | 20.0 | 23.0 | 26.0 | 27.0 | 27.0 | 27.0 |
| Aquafeed sold (kt) | 2.6 | 6.4 | 9.9 | 10.7 | 11.6 | 12.5 | 13.5 | 14.6 | 15.7 | 17.0 |
| Refined oil sold (kt) | 0.7 | 1.6 | 2.4 | 2.4 | 4.4 | 5.1 | 5.7 | 5.9 | 5.9 | 5.9 |
| Revenue | 915 | 2,015 | 3,004 | 3,320 | 4,792 | 5,720 | 6,755 | 7,540 | 8,214 | 8,961 |
| EBITDA | 65 | 392 | 770 | 791 | 1,174 | 1,455 | 1,770 | 2,011 | 2,222 | 2,460 |
| EBITDA margin | 7.1% | 19.4% | 25.6% | 23.8% | 24.5% | 25.4% | 26.2% | 26.7% | 27.1% | 27.4% |
| Net income | −142 | 163 | 541 | 463 | 526 | 811 | 1,024 | 928 | 1,088 | 1,279 |
| CFADS | −115 | 230 | 608 | 577 | 852 | 1,169 | 1,346 | 1,233 | 1,375 | 1,509 |
| DSCR (x) | – | 1.30 | 2.68 | 1.94 | 2.18 | 1.93 | 2.77 | 3.32 | 4.06 | 4.91 |
| Capex incl. sustaining | 210 | 0 | 24 | 2,314 | 678 | 75 | 80 | 85 | 90 | 96 |
| Equity injected | 213 | 0 | 0 | 714 | 0 | 0 | 0 | 0 | 0 | 0 |
| Distributions | 0 | 0 | 0 | 0 | 328 | 709 | 871 | 872 | 1,046 | 1,195 |
| EBITDA (USD m) | 0.44 | 2.54 | 4.81 | 4.75 | 6.78 | 8.07 | 9.44 | 10.32 | 10.96 | 11.67 |
| KES/USD | 148.1 | 154.0 | 160.2 | 166.6 | 173.3 | 180.2 | 187.4 | 194.9 | 202.7 | 210.8 |

Pre-operating years: EBITDA is −112 in 2027 and −51 in 2028. Equity injected is 391 in 2027 and 676 in 2028.

**Cost structure (2031).** Seed is KES 1,086m (36% of revenue). Purchased feed ingredients are KES 495m. Energy is KES 104m, labour KES 87m, dealer margin KES 90m and irrecoverable feed VAT KES 36m (`model/pnl_annual.csv`).

**Benchmarks.** Phase 1 EBITDA in 2031 is KES 565m in 2026 KES. That is above the financing file's rough KES 400m estimate, because feed margins are higher than that file assumed.

### 9.2 Unit economics (2026 KES)

| | 2031 (Phase 1) | 2035 (Phase 2) | Research benchmark |
|---|---|---|---|
| Crush gross margin, per t of seed | 20,395 | 25,002 | About 12k ([feedstock_supply.md §8](research/feedstock_supply.md)) to about 31k ([market_demand.md §6](research/market_demand.md)) |
| Feed gross margin, per t of feed | 49,452 (37%) | 49,219 (37%) | Cash cost KES 88–93/kg against a KES 110–150 price ([technical_operations.md §3.3](research/technical_operations.md)) |
| EBITDA per t of seed | 41,851 | 39,451 | – |

The 37% feed gross margin is at the **top** of the research range. It is the first number to verify, using distributor quotes and toll-produced test sales.

### 9.3 Funding need

| | KES m | Note |
|---|---|---|
| Phase 1 uses, 2027–29 | 2,241 (USD 15.7m) | Capex 1,402; Phase 0 and pre-operating 199; interest, fees and DSRA 166; working capital 342; other 133 |
| Peak net equity (whole plan) | **1,994** (about USD 13.5m) | Reached in 2032 |
| Peak project funding need | 3,313 | |
| Equity payback | 2036 (Phase 1 only: 2033) | |

Source: workbook sheet "Cash flow & funding". The other uses are principal repaid in 2029 (38), net VAT on capex (34) and minimum cash (61).

### 9.4 Returns

| Metric | Full plan (base) | Phase 1 only |
|---|---|---|
| Project IRR, KES / USD | 26.1% / 21.2% | 27.0% / 22.1% |
| Project IRR, KES, no terminal value | 12.7% | 19.2% |
| Equity IRR, KES / USD | **28.9% / 24.0%** | 29.7% / 24.7% |
| Equity IRR, KES, no terminal value | **14.6%** | 21.3% |
| Equity IRR after dividend WHT and CGT | 27.5% | 28.3% |
| Project NPV at 23% / 16.5% | +423 / +1,881 | +387 / +1,383 |
| Equity NPV at 12.25% (bond) / 35% / 40% | +3,426 / −374 / −556 | +2,400 / −250 / −406 |
| Min DSCR from 2030 | 1.30 | 1.30 |

**Phase 2 on its own terms.**
- Incremental project IRR is 23.8% and incremental NPV at 16.5% is +KES 497m. It adds value at the steady-state cost of capital but **dilutes** equity IRR.
- It also nearly doubles reliance on the exit (equity IRR without terminal value: 14.6% for the full plan against 21.3% for Phase 1 only).
- **Phase 2 is justified by NPV at the cost of the capital that would fund it, ideally cheaper outside equity at a step-up valuation. It is not justified by the founder's IRR.**

**The exit carries the return.**
- The 2038 terminal value (5.0× EBITDA of KES 2,460m, giving EV KES 12.3bn or about USD 58m) is most of the equity value.
- At 4× / 7× the equity IRR is 26.9% / 32.2%. Reaching 35% would need 9.1× [supplementary run].

### 9.5 Scenarios

| | Bear | Base | Bull | Stress (all adverse; not a forecast) | Phase 2 at research spec |
|---|---|---|---|---|---|
| Phase 2 | No-go | Go | Go | No-go | Forced go |
| Project IRR, KES / USD | −0.6% / −5.8% | 26.1% / 21.2% | 46.8% / 42.5% | n/a | 23.2% / 18.5% |
| Equity IRR, KES / USD | −4.9% / −9.9% | 28.9% / 24.0% | 55.1% / 50.6% | n/a | 25.6% / 20.7% |
| Project NPV at 23% | −1,800 | 423 | 3,683 | −3,935 | 30 |
| Equity NPV at 35% | −1,616 | −374 | 1,314 | −2,899 | −607 |
| EBITDA 2031 / 2035 | 113 / 236 | 770 / 1,770 | 1,268 / 3,397 | −380 / −643 | 770 / 1,706 |
| Peak net equity | 2,886* | 1,994 | 858 | 10,174* | 2,821 |
| Equity payback | not by 2038 | 2036 | 2033 | not by 2038 | 2037 |

*In bear and stress the model keeps injecting equity to fund losses, which overstates peak equity. A real owner would stop; the survival view models that stop as failure plus liquidation.

**Scenario definitions** ([model/outputs.md §7](model/outputs.md)):
- **Bear:** each market and cost driver half-way to its adverse bound; seed supply ×0.85; the CPO, GMO and Tanzanian levy shocks all certain; exit at 4.5×.
- **Bull:** each driver half-way to its favourable bound; seed supply ×1.12; no policy shocks; exit at 6.0×.

### 9.6 Sensitivities and break-evens

**Tornado** (equity IRR in KES; one driver at a time; base 28.9%):

| Driver (low / high setting) | Equity IRR, low | Equity IRR, high | Swing (points) |
|---|---|---|---|
| Delivered seed cost (×0.79 / ×1.26) | 38.4% | 13.5% | 24.9 |
| Capex (×0.70 / ×1.45) | 38.0% | 19.9% | 18.1 |
| Feed prices (grow-out KES 110–150, starter 160–250) | 21.1% | 38.6% | 17.5 |
| Feed market share (8% / 25% of SAM) | 20.3% | 35.3% | 14.9 |
| Oil prices with fixed-price seed | 19.2% | 32.2% | 13.0 |
| Merchant SAM growth (4% / 14%) | 24.0% | 34.1% | 10.0 |
| Oil prices (with 50% seed pass-through) | 25.6% | 33.0% | 7.4 |
| Sunflower oil yield (27% / 34%) | 25.3% | 31.6% | 6.3 |
| KES depreciation (2% / 7%) | 26.6% | 32.6% | 5.9 |
| Feed dealer margin (10% / 0%) | 26.0% | 31.9% | 5.9 |
| Seed supply (×0.70 / ×1.25) | 24.9% | 30.3% | 5.4 |
| Exit multiple (4× / 7×) | 26.9% | 32.2% | 5.3 |
| Policy items (CPO duty, GMO, SEZ, Tanzanian levy, investment deduction) | | | 0.4–1.5 each |

The full table is in [model/outputs.md §8](model/outputs.md). On the seed × oil grid, equity IRR falls to 6.0% at seed ×1.26 and oil ×0.85, and rises to 41.3% at seed ×0.79 and oil ×1.15.

**Single-driver break-evens to a 35% equity IRR, conditional on survival** [supplementary runs of `model.py`; base inputs, gate auto, senior debt held at base sizing]:

| Driver | Value needed for 35% | Compared with the research range |
|---|---|---|
| Feed price | +12.5% (grow-out about KES 141/kg, starter about KES 225/kg) | Within the range (110–150) |
| Delivered seed cost | ×0.87 (about KES 50k/t blended sunflower) | Within the range (45–72k) |
| Capex | ×0.79 (Phase 1 about USD 7.5m) | Within the range (6.6–13.8) |
| Feed market share | 24% of SAM | Near the top of the range (8–25%) |
| Oil prices | +25% | Outside the range |
| Exit multiple | 9.1× | Outside the range (4–7×) |

**Survival-weighted break-evens** (30% failure probability). To reach 35% the feed price must rise 35% (about KES 168/kg, above the research's high case), or seed must fall to ×0.61 (below the research's low case). Capex, share, oil price or exit multiple cannot do it alone, even at their extremes. **No single driver within its research range closes the gap.**

**What combination would clear the hurdle?** [supplementary runs; reproducible with `assumptions_override.csv` keys `p_feed_grow=137500`, `p_feed_start=220000`, `seed_cost_mult=0.90`, `capex_mult=0.85`, `p_fail`]:

| Case | Conditional equity IRR | Survival-weighted IRR | Peak net equity |
|---|---|---|---|
| Base (failure probability 30%) | 28.9% | 22.3% | KES 1,994m |
| Base, failure probability 15% | 28.9% | 25.9% | KES 1,994m |
| **Case A:** feed price +10%, seed −10%, capex −15% (failure probability 30%) | 42.6% | 32.2% | KES 973m |
| **Case A with failure probability 20%** | 42.6% | **35.8%** | KES 973m |
| Case A with failure probability 15% | 42.6% | 37.5% | KES 973m |
| Feed share 20% and feed price +8% (failure probability 30%) | 37.8% | 28.6% | KES 1,508m |

**This is the investment logic of the plan.** Phase 0 must produce evidence that moves *several* inputs favourably at once, and must lower the failure probability: contracted offtake and seed, an experienced GM, and firm capex quotes.

### 9.7 Survival-weighted returns against the hurdles

| Branch | Probability | Equity IRR | Equity NPV at 35% |
|---|---|---|---|
| Failure: bear operations to 2030, liquidation in 2031 at 35% of capex and 70% of working capital | 30% | −64.2% | −1,451 |
| Survive; Phase 2 no-go | 35% | 29.7% | −250 |
| Survive; Phase 2 go | 35% | 28.9% | −374 |
| **Expected (probability-weighted cash flows)** | | **22.3%** | **−654** (−759 at 40%) |

Source: [model/outputs.md §9](model/outputs.md). The 30% failure probability, the 35% liquidation recovery and the 50% chance that Phase 2 goes ahead are judgement. The 30% is anchored on the screening report's example.

**Against the hurdles:**
- **Greenfield, 35–40% expected:** fails at every failure probability. Even with zero failure risk the expected equity IRR is 29.3%. At 30% failure risk, survivors would need 45–50%; the base gives 29.3%.
- **Established business, 25–30%:** the expected IRR reaches 25% only if failure risk is about 19% or less (failure probability sweep: 0% → 29.3%; 10% → 27.0%; 15% → 25.9%; 20% → 24.7%; 30% → 22.3%; 45% → 18.2%; 60% → 13.3%).
- **Tax-free infrastructure bond, 11.75–12.74%** ([Serrari](https://serrarigroup.com/cbk-opens-ksh150bn-tax-free-infrastructure-bond-sale/)): the expected equity IRR beats it unless failure risk exceeds about 60–65%. The base equity NPV at 12.25% is +KES 3.43bn. The bond is tax-free, whereas the equity IRR after shareholder tax is 27.5% conditional on survival.
- **Bank lending, about 14.4%** ([Capital FM](https://capitalfm.africa/private-sector-credit-growth-accelerates-to-10-6pc-in-september/)): the project IRR (26.1%) is well above the cost of debt, which is why leverage would help if the plant could carry more of it (section 10).

**Model corrections made while writing this plan** (re-run on 19 October 2026):
1. **Retain gate-year cash for Phase 2.** The waterfall had paid a KES 424m dividend in 2031 and then called KES 1,138m of equity in 2032. The cash is now retained when Phase 2 goes ahead, and the 2032 equity call falls to KES 714m.
   - Equity IRR falls from 29.4% to 28.9% (USD from 24.4% to 24.0%; no-TV from 14.9% to 14.6%).
   - Equity NPV at 35% moves from −341 to −374; survival-weighted IRR from 22.4% to 22.3%.
   - Peak net equity and project returns are unchanged.
2. **Exit EV floored at zero.** This affects only the stress case's project NPV (−4,266 becomes −3,935).

---

## 10. Financing plan and capital structure

### 10.1 Phase 1 sources (2027–29)

| Instrument | KES m | USD m (2028 FX) | Terms (model) | Likely providers |
|---|---|---|---|---|
| Founder and co-investor equity (net) | 1,279 | 8.98 | Ordinary equity | Founder; preferably a strategic co-investor for USD 1.5–3m ([financing_capital.md §6](research/financing_capital.md)) |
| Standby equity for cost overruns | (undrawn) | 1.4 | 15% of capex; required by lenders | Founder |
| Senior KES term loan | 416 | 2.92 | 15.5% floating; 7 years including 18 months' grace; quarterly instalments; first charge, debenture, 6-month DSRA; lock-up at DSCR 1.30×; default at 1.10× | KCB, Equity, Stanbic, NCBA, Co-op; ideally with IFC or BII risk-sharing ([BusinessTech Africa](https://www.businesstechafrica.co.za/article/african-smes-are-finding-another-way-to-borrow-money)) |
| Mezzanine (USD) | 242 | 1.70 | 13% all-in plus 15% WHT gross-up; 8 years; 3-year grace; 2 years PIK | AgDevCo: precedents of USD 9.5m to Agventure ([AgDevCo PR](https://www.agdevco.com/site/assets/files/2133/agventure_press_release_nov_2024.pdf), [DATED]) and USD 15m to Victory Farms ([WeAreAquaculture](https://weareaquaculture.com/news/finance/tilapia-producer-victory-group-secures-15m-follow-on-investment-from-agdevco)) |
| Grants | 42 | 0.30 | Outgrower and ESIA co-funding only | AECF, foundations, IFAD-programme co-funding [UNVERIFIED] |
| Seasonal stock-finance revolver | 161 at end-2029 (intra-year peak 353) | 1.13 | 14.5%; advances 65% of seed stock under collateral management or WRS | Lead bank plus a collateral manager |

Source: [model/outputs.md §3](model/outputs.md).

**Debt capacity is the binding financing fact.**
- The financing file proposed USD 4.5m of senior debt. On the model's ramp, the plant can carry only **KES 416m (USD 2.9m)** at a minimum DSCR of 1.30× over 2030–34. Equity fills the gap, so Phase 1 long-term funding is about 65% equity and grants, not 50%.
- **The 2030 DSCR is exactly 1.30×.** There is no headroom: a 15% shortfall in 2030 CFADS would breach the 1.10× default covenant.
- Lenders should therefore be asked for one of:
  - a 24-month grace period ([financing_capital.md row 6](research/financing_capital.md));
  - repayments sculpted to CFADS;
  - a covenant holiday in operating year 2.
- Alternatively, cut senior debt further and add equity [plan recommendation].

**Currency.** The crush margin is partly USD-indexed, because oil and cake are priced off import parity ([financing_capital.md §1](research/financing_capital.md)). USD debt is about 37% of Phase 1 term debt, inside the at-most-50% guideline. Pwani Oil's 2022 shutdown "for lack of dollars" ([The Star](https://www.the-star.co.ke/news/2022-06-06-pwani-oil-shuts-plant-blames-lack-of-dollars), [DATED]) argues for committed USD trade lines for premix, fishmeal and spares, for example via the AfDB–Family Bank USD 10m line ([fundsforNGOs, Oct 2026](https://news.fundsforngos.org/2026/10/14/afdb-family-bank-10-million-trade-finance-line-kenya-smes-foreign-currency/)).

### 10.2 Phase 2 sources (2032–33)

| Instrument | KES m | Terms |
|---|---|---|
| Retained 2031 cash | about 420 | Gate year |
| New equity | 714 | Existing shareholders in the model |
| Phase 2 DFI loan in KES (TCX-hedged) | 1,593 | 55% of Phase 2 capex; 14%; 9 years; 2-year grace |
| Revolver upsized | to KES 0.6–0.7bn year-end | |

Possible lenders are IFC, Proparco (precedent: USD 18.7m to Kenya Nut Company, [Africa PE News](https://www.africaprivateequitynews.com/p/proparco-backs-kenya-nut-company-with-18-7m-loan)), FMO and AATIF.

**Recommended variation (not modelled).** Fund the Phase 2 equity with a 25–40% minority from an outside fund at a step-up valuation, rather than with founder money. Fund targets of about 22% in USD ([financing_capital.md §1](research/financing_capital.md), [UNVERIFIED]) cost less than the founder's 35–40% hurdle. The model does not show the resulting dilution or accretion.

### 10.3 Use of funds, Phase 1 (KES m nominal, 2027–29)

| Use | KES m |
|---|---|
| Capex including land, contingency, IDF/RDL | 1,402 |
| Phase 0 and pre-operating | 199 |
| Interest during build and ramp-up | 92 |
| DSRA | 64 |
| Working-capital build | 342 |
| Fees, 2029 principal, VAT timing, minimum cash | 142 |
| **Total** | **2,241** |

These uses are funded by the sources in section 10.1 plus KES 100m of 2029 operating EBITDA.

### 10.4 Phasing of the capital commitment

| Stage | Commitment | Decision gate |
|---|---|---|
| Phase 0 (Q4 2026 – Q3 2027) | USD 0.8m (KES about 110m), expensed | Approve now |
| FID (Q4 2027) | USD 9.0m equity plus USD 1.4m standby; debt signed | G0 tests (section 12) |
| Phase 2 (2032) | About KES 0.7bn equity, or outside equity; KES 1.6bn DFI loan | G1 on 2031 audited results |

---

## 11. Risk register and mitigants

The register is ranked by expected impact on equity value. Probabilities are [ESTIMATE] unless cited. IRR effects are from the model's tornado or scenarios.

| # | Risk | Probability (2027–31) | Impact | Mitigants | Early-warning indicator |
|---|---|---|---|---|---|
| 1 | **Feed price war and merchant-share shortfall.** Regional capacity (Tunga 45 kt, SamakGro 8 t/h, De Heus 50–100 kt) exceeds merchant demand. Victory Farms is 90% captive | High (about 50% that prices or share land below base) | Feed price at its low bound: equity IRR 21.1%. Share at 8%: 20.3% | Anchor LOIs before FID; starter and fingerling niche; depot and credit service; toll or protein-supply deal with a multinational as a fallback | Competitor list prices; dealer quotes; 2030 feed tonnage below 4 kt |
| 2 | **Seed cost and volume.** Thin, contested supply; the Bidco outgrower precedent | About 40% that year-1 throughput is below 60% of plan ([feedstock_supply.md §10](research/feedstock_supply.md)) | Seed cost ×1.26: equity IRR 13.5%. Supply ×0.70: 24.9% | Floating parity-linked contracts; three-country sourcing; Uganda weighted; Tanzania capped at 25%; cake/feed buy-back; Phase 0 pilot | Pilot delivery rate; side-selling above 30% |
| 3 | **Policy reversal on oil.** CPO duty lost (60%); KNTC-style duty-free oil imports (25%) | 60% / 25% ([regulatory_tax_risk.md §7](research/regulatory_tax_risk.md)) | −KES 12–18k/t on oil; certain removal: −0.5 points | Underwrite at the probability-weighted value; feed carries the margin; refine for the 20 L institutional segment; seed price linked to parity | EAC gazette each June; the COFEK judgment; any appeal |
| 4 | **Capex overrun and delay** | About 30% for more than 20% overrun [ESTIMATE] | Capex ×1.45: equity IRR 19.9% | Three written quotes per package; fixed-price EPC for civil works; 15% contingency; USD 1.4m standby equity; hedge USD capex | Quotes above USD 12m (kill test) |
| 5 | **Management and execution** (founder without sector experience) | High without mitigation | Drives the 30% failure probability. Cutting it to 15% adds 3.6 points of expected IRR | Experienced GM hired before FID; technical partner; independent board members with sector experience | GM not hired by month 9 |
| 6 | **GMO ruling allowing GM imports** | 40% by end-2028 ([regulatory_tax_risk.md §7](research/regulatory_tax_risk.md)) | Protein meals −20–30%. Partly hedged because feed input costs also fall. Certain: −0.7 points | Size the feed line to absorb most own cake; never accept GM material | Court of Appeal judgment ([Biosafety Information Centre](https://biosafety-info.net/articles/policy-and-regulation/africa/court-of-appeal-halts-government-promotion-of-gmos-in-landmark-ruling/)) |
| 7 | **Lake Victoria social licence.** Senate petition (5 Aug 2026), hearings (2 Oct 2026), fish kills, the 5% aquaculture levy | 40% zoning or pause in parts of Homa Bay; 10% broad moratorium | Feed demand growth cut from about 19% to 8–10% a year. SAM growth at 4%: equity IRR 24.0% | Diversify buyers across Siaya, Busia and Migori and into Uganda; support zoning; feed quality that lowers FCR and waste; a poultry/dairy pellet option | Senate committee report; KeFS licensing data |
| 8 | **Election, 10 Aug 2027** | 30% for 2 weeks or more of disruption; 50% for KES depreciation above 6% in 2027 ([regulatory_tax_risk.md §7](research/regulatory_tax_risk.md)) | Capex delay; FX on imported plant (+1.5 points of depreciation already in the base) | **FID after the result is settled (Q4 2027)**; Phase 0 spending only before then; 65% of CEOs are delaying capex ([The Standard](https://thestandard.ke/sports/amp/business/2001556263/political-anxiety-casts-shadow-on-kenyas-investment-outlook)) | Petition timetable; KES forwards |
| 9 | **FX** (KES depreciation, USD mezzanine, imported spares and premix) | Base 4% a year; tail 20–25% shock | KES IRR rises with faster depreciation (PPP in the model); USD IRR flat (24.2–23.9%) | Mezzanine kept at 37% or less of term debt; ask for a KES option; forward cover for debt service; USD trade lines | CBK reserves; forward premium |
| 10 | **Aflatoxin and quality incident** | 15–25% for a material recall in 5 years [ESTIMATE] | Loss of brand and KEBS mark | Lot testing; release limit; no groundnut; Tanzanian cake excluded from fish feed | Rejection rates by origin |
| 11 | **Working capital, VAT refunds and eTIMS** | 60% for refunds delayed more than 6 months, if in a refund position | Not modelled; 1–3% of revenue locked up | Structure the entity as a net VAT payer (oil); eTIMS reverse invoicing; WRS stock finance | KRA refund ageing |
| 12 | **DSCR covenant breach in 2030** | About 30% [ESTIMATE; the base is exactly at 1.30×] | Lock-up or default; forced equity cure | Negotiate 24-month grace or sculpting; standby equity; a lower senior quantum | Quarterly CFADS from 2029 |
| 13 | **Tanzanian levy or ban; regional seed competition** | 70% levy; 25% ban in some season | Levy certain: −0.3 points; volume loss | Cap Tanzania at 25%; Uganda licensed aggregators | TRA notices; Kajiado flows |
| 14 | **Exit risk:** no Kenyan agro-processing multiple observed; thin buyer universe | – | Exit at 4×: 26.9%; without terminal value: 14.6% | Build a strategic buyer universe early (section 13); keep Phase 1-only optionality | Strategic approaches; regional M&A comparables |
| 15 | Power cost and reliability; wayleave-driven tariff rise above 30% | 30% [ESTIMATE] | Electricity at KES 25/kWh: −0.5 points | Standby genset; hull-fired boiler in Phase 2; check SEZ/geothermal options | EPRA schedule |
| 16 | Hexane safety (Phase 2 only) | Low probability, severe impact | Fatality, plant loss | Phase 2 only with an experienced operator; hazardous-area zoning; insurance | – |
| 17 | Government arrears; price controls on cooking oil | 70% delays if selling to the state; 10% price controls | Receivables; 10–20% margin compression | Public-sector sales capped at 10%; B2B bulk channel | – |

---

## 12. Implementation plan

### 12.1 Timeline

| Period | Milestones |
|---|---|
| **Q4 2026** | Incorporate HoldCo, OpCo and PropCo; eTIMS; recruit the procurement/outgrower manager; start the GM search; commission the feed market study, offtake soundings and capex quotes; send a teaser to AgDevCo and two banks; tax opinion |
| **Q1 2027** | Outgrower pilot contracts signed for the long rains (2,000–3,000 ha, randomised contract terms); seed lab tests; toll-pressing pilot; site shortlist and land option; start the EIA |
| **Q2–Q3 2027** | Pilot harvest (July–September): measure delivery and side-selling; toll-extruded feed trial sales; KMFRI feeding trials; indicative debt terms; LOIs; GM hired; **pause on commitments during the 10 August 2027 election window** |
| **Q4 2027 – FID (G0)** | Re-run the model on Phase 0 data; board decision against the section 12.2 tests; sign EPC and OEM contracts and debt |
| 2028 | Construction (15 months; range 12–20); power connection; KEBS pre-certification; second outgrower season |
| **About April 2029 – COD** | Commissioning; KEBS marks per SKU; feed launch with an entrant discount |
| 2029–2031 | Ramp-up: crushing 6 → 11 → 13.5 kt; feed 2.6 → 6.4 → 9.9 kt |
| **Early 2032 – Phase 2 gate (G1)** | On 2031 audited results |
| 2032–2033 | Phase 2 build (if go); outside equity raise |
| 2036–2038 | Exit window (section 13) |

### 12.2 Gate G0 (FID): explicit kill criteria and proceed criteria

**Kill: abandon or restructure if any one of these holds at the end of Phase 0** [plan recommendation; thresholds set at or near the research's adverse bounds]:

| # | Test | Kill threshold | Model reference |
|---|---|---|---|
| K1 | Kenyan merchant aquafeed demand (cage-farm survey plus distributor data) | Below 20 kt a year in 2027 | Bottom of the research range; the model's SAM is 45 kt, including Uganda and Tanzania |
| K2 | Achievable grow-out feed price (dealer and distributor quotes, trial sales), list-equivalent before dealer margin | Below KES 115/kg in 2026 KES | Base 125. At 110, equity IRR is 21.1% |
| K3 | Delivered blended sunflower seed cost (signed aggregator and outgrower terms plus pilot actuals) | Above KES 65k/t | Base 57k. At ×1.12, equity IRR is about 23% |
| K4 | Seed under contract or credible import agreement for 2029 | Below 8 kt | [financing_capital.md §6](research/financing_capital.md) FID condition |
| K5 | Outgrower pilot outcome | Side-selling above 50%, or delivered yield below 0.6 t/ha | Research adverse bounds |
| K6 | Firm Phase 1 capex quotes (scope as in section 6.2) | Above USD 12m | Base 9.5m. At ×1.45, equity IRR is 19.9% |
| K7 | Lab-tested oil content of target-county seed | Implies full-press yield below 28% | Base 31% |
| K8 | Committed debt | Senior plus mezzanine below KES 600m, or senior rate above 17.5% | Base KES 658m at 15.5% / 13% |
| K9 | Management | No sector-experienced GM signed | Section 8 |
| K10 | Policy | Broad moratorium on new cage licences in Siaya and Homa Bay adopted | [regulatory_tax_risk.md §7](research/regulatory_tax_risk.md) rank 5 |

**Proceed: FID only if all kill tests pass AND, when the model is re-run with the Phase 0 values, the survival-weighted KES equity IRR is at least 35% at a failure probability the board can defend.** On current inputs that means evidence for roughly the following:
1. Feed realisation of at least KES 137/kg list-equivalent, **or** feed LOIs implying at least 20% share.
2. Delivered seed of KES 51k/t or less.
3. Phase 1 capex of USD 8.1m or less.

**plus** risk reducers that justify a failure probability of 20% or less:
- feed LOIs of at least 5 kt a year from five or more non-Victory farms;
- LOIs for at least 50% of crude oil or cake;
- at least 10 kt of seed contracted;
- an experienced GM in post.

If the kill tests pass but the proceed test fails, **restructure rather than build**. The options below are unmodelled and should be evaluated in Phase 0:
- **Feed-mill-first:** a 3 t/h extrusion line buying protein, with toll crushing. This cuts capex and seed risk.
- **Acquire an under-used existing feed mill.** Millers run at 50–60% utilisation ([The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)).
- **Joint venture with a strategic** (a cage-farm group or a multinational feed maker) that brings offtake.

### 12.3 Gate G1 (Phase 2, on 2031 audited results)

Phase 2 goes ahead only if all of the following hold:
- (a) **At least 24 kt of seed contracted** (signed outgrower and import agreements, not the supply path) for 2035.
- (b) 2031 feed sales of at least 8 kt at a gross margin of at least 20% (model: 9.9 kt at 37%).
- (c) At least 70% of crude for sale refined under the own brand (model: 80%).
- (d) Positive incremental NPV at 16.5% (model: +KES 497m).

Two plan recommendations are added:
- (e) A minimum DSCR of at least 1.5× in 2031.
- (f) Phase 2 equity priced by an outside investor at a valuation of at least the Phase 1 equity invested.

The model's gate (a) uses the assumed supply path, which makes the test circular. Contracts must replace it.

### 12.4 Operating tripwires (2029–31)

A board review of turnaround, sale or wind-down is triggered if any of these occur [plan recommendation]:
- 2030 EBITDA below KES 200m (model 392; bear −57);
- 2030 feed sales below 4 kt (model 6.4);
- seed crushed in 2030 below 7 kt (model 11.0);
- DSCR below 1.10× in any test period.

The survival tree's failure branch (liquidation in 2031 at 35% of gross capex) is the cost of acting late. Acting on these tripwires early is how recovery is maximised.

### 12.5 The first 12 months: information-buying programme (Phase 0, USD 0.8m)

| # | Workstream | What it measures | Indicative cost [ESTIMATE] | Answers |
|---|---|---|---|---|
| 1 | **Feed market study:** census of a sample of cage farms in Siaya, Homa Bay, Busia and Migori; Victory Farms' true share; dealer margins; payment terms | Merchant demand, price, share | USD 60–90k | K1, K2; SAM, share |
| 2 | **Distributor and dealer quotes**, plus **toll-extruded trial sales** of 200–500 t of own-formula feed under a provisional brand, via an existing mill or the Kisumu Centre of Excellence | Realised net price; customer repeat rate; FCR feedback | USD 80–150k (partly recovered through sales) | K2; the 37% margin |
| 3 | **Outgrower pilot** (2,000–3,000 ha) with randomised contract designs (floating against fixed price; cake buy-back) and weigh-and-pay | Side-selling, yield, supply elasticity, programme cost per tonne | USD 250–400k ([financing_capital.md §6](research/financing_capital.md)) | K4, K5; seed cost |
| 4 | **Seed quality:** NIR or Soxhlet tests on 20–30 lots from target counties and Ugandan aggregators; toll-pressing of 20–50 t | Oil content, yield, aflatoxin incidence by origin | USD 30–50k | K7 |
| 5 | **Capex:** three written CIF Mombasa quotes each for oil equipment (Chinese/Indian/European) and extrusion (Famsun, Muyang, Andritz/Bühler); civil-works bill of quantities; power connection quote | Capex | USD 50–100k (FEED) | K6 |
| 6 | **Offtake LOIs:** crude oil (Bidco, Menengai, Kapa); cake (Rift millers); feed (cage farms); protein-supply option with a multinational | Offtake | Staff time | Proceed criteria |
| 7 | **Financing:** AgDevCo, two banks, IFC/AGF risk-sharing, collateral manager, WRS eligibility of oilseeds | Debt quantum and terms | USD 30–60k (legal) | K8 |
| 8 | **Legal and tax:** investment-deduction threshold opinion; VAT ruling on feed; eTIMS reverse invoicing; GMO and CPO litigation monitoring; land due diligence | Tax and regulatory | USD 40–80k | Section 7 |
| 9 | **EIA, site and permits** | Licensing timeline | KES 8–30m ([regulatory_tax_risk.md row 24](research/regulatory_tax_risk.md)) | Critical path |
| 10 | **GM recruitment** (retained search) | Management | USD 40–60k | K9 |

---

## 13. Exit options and valuation

**Valuation basis.**
- The base exit is 5.0× 2038 EBITDA [ESTIMATE, [financing_capital.md §8](research/financing_capital.md)], giving EV of KES 12.3bn (about USD 58m) and equity of about KES 11.4bn after net debt.
- Anchors:
  - KPC's IPO at about 8.1× EV/EBITDA (regulated infrastructure; an upper bound) ([african-markets](https://www.african-markets.com/en/stock-markets/nse/kenya-pipeline-company-ipo-subscribed-at-105-7-listing-on-the-nairobi-securities-exchange-scheduled-for-march-10)).
  - US lower-middle-market private equity at 5.5–6.4× ([Capitalpad](https://capitalpad.com/lower-middle-market-ebitda-multiples/)).
- **No Kenyan or East African agro-processing transaction multiple was found.** That is an evidence gap.

**Exit routes, ranked by likelihood** [judgement, [financing_capital.md §8](research/financing_capital.md)]:
1. **Trade sale to a feed or aquafeed strategic** (Nutreco/Skretting via Tunga, De Heus, or Victory Farms/SamakGro) seeking local non-GM protein and lake-side capacity. This is strongest if the GMO import ban persists.
2. **Trade sale to an edible-oil refiner** (Bidco, Kapa, Pwani, Menengai) wanting EAC-origin soft oil and an outgrower base.
3. **A regional agri-trader** (ETG, Olam/ofi, Mainland Group) [UNVERIFIED appetite].
4. **PE secondary or buy-out of the founder** by the Phase 2 fund or another fund (Catalyst, Phatisa).
5. **NSE listing.** Unlikely below about USD 50m EV.

**What the exit is worth to the return.**

| Exit assumption | Equity IRR |
|---|---|
| 4× | 26.9% |
| 5× (base) | 28.9% |
| 7× | 32.2% |
| No exit value | 14.6% |
| Phase 1 only, no exit value | 21.3% |

Because the return is back-loaded and exit-dependent, an investor should value the strategic-buyer universe as an asset to build from day one: a protein-supply or toll relationship with a multinational doubles as exit preparation.

**Interim liquidity.** Distributions begin in 2033 and total KES 5.0bn over 2033–38 in the base case. Equity payback is 2036 (2033 for Phase 1 only).

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
| Labour | 115+ jobs plus field staff | Statutory wages and above; OSH; contractor standards |
| Land | Change of user; community claims | Industrial-zoned plot; title due diligence; no involuntary resettlement |

### 14.2 Development impact (indicative; [ESTIMATE] unless stated)

- **Smallholder income.** About 4,500–9,000 contracted farmers by 2031 and 15,000–30,000 by 2036 (section 5.3), paid by mobile money at harvest. Seed gross revenue at the KES 52k/t contract price is about KES 0.15bn in 2031 and about KES 0.5bn in 2036 (2026 KES).
- **Import substitution.** About 7.5 kt of oil a year by 2036, worth about USD 11m a year at landed parity (7.5 kt × about USD 1,500/t). About 9 kt a year of non-GM protein meal replaces regional and imported meal. Both are small against national totals (about 1% of oil consumption). Their value is local value addition rather than macro significance.
- **Fish-feed access.** Locally made, tested floating feed for small and mid-size cage farmers, who face feed at more than 60% of production cost ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back)). FCR improvements lower both cost and lake nutrient loading.
- **Jobs.** About 70 direct jobs in Phase 1, about 115 after Phase 2, plus 6–10 extension staff and indirect jobs in aggregation and haulage.
- **Nutrition.** Vitamin A-fortified oil for the institutional segment.
- **Measurement.** The randomised outgrower pilot gives credible, not anecdotal, impact evidence. That is valuable to DFIs and grant funders.

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
| Crude oil to refiners | 165k | 190k | 210k KES/t | [ESTIMATE] from crude sunflower import parity |
| Refined bulk oil | 231k | 264k | 302k KES/t | [ESTIMATE]; Mama Pima KES 185/L benchmark |
| CPO duty protection × probability lost | 12k | 15k × 60% | 18k | [regulatory_tax_risk.md §7](research/regulatory_tax_risk.md) |
| Sunflower cake | 32k | 40k | 50k KES/t | Jiji listing [UNVERIFIED]; [DATED] series |
| Non-GM soybean meal (bought) / own soy cake | 80k / 65k | 95k / 85k | 120k / 100k | Indexbox [UNVERIFIED]; [ESTIMATE] |
| Grow-out feed / starter feed | 110 / 160 | 125 / 200 | 150 / 250 KES/kg | SamakGro list (undated); WorldFish; starter [ESTIMATE] |
| Feed dealer margin; new-entrant discount | 0%; 0% | 5%; 5% (years 1–2) | 10%; 10% | [ESTIMATE] |
| Merchant aquafeed SAM 2026; growth | 30 kt; 4% | 45 kt; 8% | 60 kt; 14% | [market_demand.md §4–5](research/market_demand.md) [ESTIMATE] |
| Maximum feed share of SAM | 8% | 15% | 25% | [ESTIMATE] |
| Refined share of crude for sale | 50% | 80% | 95% | [ESTIMATE] |
| Starter share of feed tonnes | 5% | 15% | 25% | [ESTIMATE] |
| Grid electricity | 16 | 20 | 25 KES/kWh | EPRA 2023 [DATED] plus 2026 pass-throughs |
| Labour, Phase 1 | 50 | 61 | 80 KES m/yr | [technical_operations.md §4.3](research/technical_operations.md) |
| Maintenance | 2.5% | 3.5% | 5% of equipment | [technical_operations.md row 33](research/technical_operations.md) |
| Phase 1 / Phase 2 capex | ×0.70 | USD 9.49m / 15.25m | ×1.45 | [technical_operations.md §4.1](research/technical_operations.md) [ESTIMATE, ±40%] |
| Phase 0 development | 0.6 | 0.8 | 1.0 USD m | [financing_capital.md §6](research/financing_capital.md) |
| Senior rate / tenor / grace | 14% / 5y / 12m | 15.5% / 7y / 18m | 17.5% / 8y / 24m | [financing_capital.md rows 5–6](research/financing_capital.md) [ESTIMATE] |
| Mezzanine (USD) | 11% | 13% plus WHT gross-up | 16% | [financing_capital.md row 9](research/financing_capital.md) [ESTIMATE] |
| DSCR sizing and lock-up | 1.20 | 1.30 | 1.40 | [financing_capital.md row 14](research/financing_capital.md) |
| Phase 2 DFI loan: share / rate / tenor | 45% / 13% | 55% / 14% / 9y | 60% / 16% | [financing_capital.md §6](research/financing_capital.md) |
| CIT; investment deduction | 10% (SEZ); 50% | 30%; 100% | 30%; 100% | [regulatory_tax_risk.md rows 1–3](research/regulatory_tax_risk.md) |
| Irrecoverable feed VAT; feed levy | 1%; 0 | 2%; 0.5% | 3.5%; 1% | [ESTIMATE] |
| Exit multiple | 4.0× | 5.0× | 7.0× | [financing_capital.md row 27](research/financing_capital.md) [ESTIMATE] |
| WACC Phase 1 / steady state | 19% / 14% | 23% / 16.5% | 27% / 19% | [financing_capital.md §5](research/financing_capital.md) |
| Failure probability; liquidation recovery; P(Phase 2 go) | 15%; 20%; 30% | 30%; 35%; 50% | 45%; 50%; 70% | Judgement, anchored on the [screening report](../../reports/Profitable%20business%20opportunities%202026.md) |
| Seed safety stock; bad debts | 0.5 mo; 0.25% | 1.5 mo; 0.5% | 2.5 mo; 1% | **Modeller's judgements, not in the research** |

---

## Appendix B. Evidence-quality notes

| Input | Grade* | Comment |
|---|---|---|
| Edible-oil import volumes and bill | B | Official AFA and USDA series exist, but conflict by ±25%; bill estimates range KES 100–160bn [CONFLICT]. This does not drive returns |
| Cage output growth | B | KNBS via secondary press; the Victory Farms share is unresolved [CONFLICT]. **This drives the feed SAM** |
| Merchant aquafeed market size and share | **C** | Derived (output × FCR − captive share). No survey. **The highest-value Phase 0 item** |
| Feed prices | C | Undated retail list and a WorldFish farm-level range; no ex-mill or distributor quote. **The 37% margin sits on this** |
| Seed volumes and delivered cost | **C** | National statistics conflict by up to 10×; delivered cost is a build-up estimate; no side-selling data |
| Oil prices (crude and refined, local) | C | Import parity is well sourced (B). No public price at which refiners buy local crude |
| Cake and meal prices | C | Mostly [DATED] or marketplace listings |
| Capex | C | Bottom-up estimate (±40%); listings, not quotes; comparators are full-scope (Mainland USD 28m, De Heus USD 25m) |
| Process yields | C | International or older literature; Kenyan seed oil content unmeasured |
| Tax and duty regime | B | Statutes cited through practitioner summaries; several [CONFLICT]s (deduction threshold, feed VAT, IDF/RDL, CPO duty status) |
| Policy probabilities | C | Judgemental, informed by event history |
| Debt terms | C | No disclosed term sheets for any Kenyan agri DFI deal; structuring assumptions only |
| Exit multiple | C | No Kenyan comparables; US LMM benchmarks with a country discount |
| Failure probability | C | The screening report's illustrative 30%; Kenyan survival data are dated and micro-firm-based |

*A = audited or regulator data at a close comparable; B = sourced market data with some conflict; C = estimate, listing or inference.

**General caveats.**
- Most web sources were read through search-result extracts only.
- KNA page dates are often crawl dates, not publication dates.
- Every comparable is a survivor (Victory Farms, Agventure); failures are not reported, so the evidence base is biased upward ([screening report](../../reports/Profitable%20business%20opportunities%202026.md)).
- **Not modelled:** the SEZ route; VAT refund delays; eTIMS disallowance of informal seed purchases; EAC duty remission (upside); dilution or accretion from outside Phase 2 equity; a monthly cash model (the model is annual with a seasonal profile).
- **The model treats the Phase 2 gate with perfect foresight** of each scenario's prices. In practice the decision is made under uncertainty.

---

## Appendix C. Items to verify in due diligence

**Market and commercial**
1. Victory Farms' actual share of KNBS cage output, and whether Doho or SamakGro sells surplus feed in Nyanza.
2. Ex-mill and distributor prices for grow-out and starter feed from Tunga/Fugo, SamakGro, Aller Aqua/AquaRech and De Heus; dealer margins; credit terms.
3. Utilisation and pricing behaviour of Tunga (45 kt), SamakGro's new 8 t/h plant and De Heus Njeru.
4. Prices refiners pay for local crude sunflower oil (Bidco, Menengai, Kapa procurement); crude quality specification.
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
20. IDF/RDL rates and any manufacturer concessions; CGT rate; minimum tax repeal.
21. The Livestock Bill 2026 text (feed levies, registration); the Food and Feed Safety Act 2026 obligations.
22. The outcome of the Senate cage inquiry; the aquaculture levy appeal.
23. eTIMS reverse-invoicing mechanics for smallholder seed purchases.
24. SEZ domestic-sale customs treatment (only if the SEZ route is considered).

**Financing and legal**
25. Indicative terms from AgDevCo (including a KES option), two banks (with IFC, BII or AGF risk-sharing) and a collateral manager.
26. Land title, change of user, the Land Control Board, and the PropCo lease structure under Article 65.
27. Kenyan or regional agro-processing M&A multiples; strategic interest from feed multinationals.

**Model**
28. Independent review of `model/model.py`: tax computation, the debt-sizing loop, survival-tree construction, and the gate logic (gate (a) uses the assumed supply path).
