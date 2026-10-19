# Market demand and pricing: oilseed crushing + animal/aqua feed mill (Kenya, with EAC)

Prepared 19 October 2026. FX for conversions: KES 129.8/USD (base). Density of vegetable oil 0.91 kg/L (1 t ≈ 1,099 L).
Conventions: **[ESTIMATE]** = my own figure, with reasoning given. **[DATED]** = source data older than 2025. **[CONFLICT]** = sources disagree. **[UNVERIFIED]** = weak or secondary source. All web pages were seen through search-result summaries only. Direct fetches failed with DNS errors, so check the figures against the primary documents before committing capital.

---

## 0. Key assumptions for the model

| # | Parameter | Low | Base | High | Unit | Source / basis |
|---|---|---|---|---|---|---|
| 1 | KES/USD | 125 | 129.8 | 145 | KES per USD | Brief; high case = depreciation stress [ESTIMATE] |
| 2 | Kenya edible oil & fat consumption, 2026 | 650 | 780 | 950 | kt/yr | Range spans 600 kt (AFA via [The Star, Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)) to ~0.9–0.95 Mt (USDA palm imports 1.0–1.05 Mt less ~0.1 Mt re-exports, [Milling MEA/USDA, Jul 2025](https://millingmea.com/kenyas-palm-oil-imports-to-hit-1-05-million-tonnes-in-2025-2026-usda/)). Base is near Q2-2025 AFA imports annualised (733 kt) plus a little local output [ESTIMATE] |
| 3 | Edible oil demand growth to 2030 | 2.5 | 3.5 | 5.0 | %/yr | [ESTIMATE]: population ~2%/yr plus income/urbanisation. USDA's palm import path (875 kt 2024 → 1.05 Mt 2025/26) is faster but includes restocking/re-exports |
| 4 | Crude palm oil (CPO) FOB Malaysia | 1,000 | 1,150 | 1,350 | USD/t | RM4,500–4,600/t (Jun 2026, [Bernama](https://www.bernama.com/lite/news.php?id=2544958)) at RM4.04–4.08/USD (Sep–Oct 2026, [Bernama](https://bernama.com/en/market/news.php?id=2620367)) = ~USD 1,110–1,135. RBD olein FOB Malaysia USD 1,252.5 (8 Sep 2026, [Fastmarkets](https://www.fastmarkets.com/insights/correction-to-price-for-refined-bleached-deodorized-palm-olein-on-september-8-2026/)) |
| 5 | CPO landed Mombasa, duty-paid | 160,000 | 185,000 | 220,000 | KES/t | [ESTIMATE] FOB 1,150 + freight/insurance ~60 + 10% duty ([The Standard](https://thestandard.ke/sports/business/2001515437/edible-oil-processors-rekindle-push-to-scrap-import-duty-tax)) + IDF/RDL ~5.5% + port/clearing ~30 = USD 1,428/t ≈ KES 185k/t ≈ **KES 169/L** |
| 6 | Crude sunflower oil (CSFO) FOB Black Sea | 1,100 | 1,270 | 1,450 | USD/t | Russia ~1,265, Ukraine ~1,275 (10–11 Sep 2026); EU 1,385–1,390 ([Commodity-Board](https://commodity-board.com/russia-takes-the-wheel-in-sunflower-oil-what-it-means-for-prices)) [UNVERIFIED aggregator] |
| 7 | CSFO landed Mombasa, duty-paid | 180,000 | 209,000 | 240,000 | KES/t | [ESTIMATE] FOB 1,270 + Red Sea-affected freight ~100 + 10% duty (assumed same CET band as CPO, verify) + levies 5.5% + 30 = USD 1,612/t ≈ **KES 190/L** |
| 8 | Local crude sunflower oil, ex-crusher, sold to refiners | 165,000 | 190,000 | 210,000 | KES/t | [ESTIMATE] 5–12% below CSFO import parity (consistency, volume and quality-risk discount). Floor ≈ CPO parity, because refiners can switch feedstock |
| 9 | Refined sunflower oil, bulk/ex-works (own brand or toll) | 231,000 | 264,000 | 302,000 | KES/t | [ESTIMATE] = KES 210/240/275 per L. KNTC "Mama Pima" bulk at KES 185/L wholesale, 210/L retail ([Kenya Times, Jul 2026](https://thekenyatimes.com/business/govt-unveils-mama-pima-cooking-oil-dispenser/)) sets a state-subsidised floor for loose palm olein |
| 10 | Retail cooking oil (national average, salad oil) | 330 | 358 | 380 | KES/L | KNBS KES 358.09/L, Jul 2026; 342.98 Dec 2025; peak 379.84 Sep 2022 ([Business Daily](https://www.businessdailyafrica.com/bd/economy/cooking-oil-prices-climb-back-to-highs-of-2022-crisis-5548020)) |
| 11 | Sunflower cake (expeller, ~28–34% CP) | 32 | 40 | 50 | KES/kg | KES 25→35/kg [DATED ~2022–23] ([Business Daily](https://www.businessdailyafrica.com/bd/markets/commodities/zambia-material-export-sends-feed-prices-record-high-3531764)); Nairobi listing KES 40/kg, 50 kg bags ([Jiji](https://jiji.co.ke/viwandani-makadara/feeds-supplements-seeds/sunflower-seed-cake-dTh5NuF0GdsvaWJ01XlkOR3T.html)) [UNVERIFIED] |
| 12 | Soybean meal (non-GM, ~44–46% CP), delivered Nairobi | 80 | 95 | 120 | KES/kg | Indexbox KES 90–120k/t (2026) [UNVERIFIED]; soybeans KES 75→100/kg (Aug 2024, [The Star](https://the-star.co.ke/news/star-farmer/2024-08-06-feed-millers-stare-at-shortage-as-soybean-prices-surge-by-over-sh15)) [DATED]; CBOT Dec-26 SBM ~USD 357/short ton ≈ USD 394/t ([Feedstuffs](https://www.feedstuffs.com/commodities/soybean-meal)); GMO premium applies |
| 13 | Cottonseed cake | 30 | 38 | 45 | KES/kg | [ESTIMATE]: no 2025–26 price found; set just under sunflower cake on CP, gossypol limits |
| 14 | Omena/fishmeal (feed grade) | 120 | 160 | 220 | KES/kg | [ESTIMATE] from human-grade wholesale >KES 200/kg (2 kg tin >KES 400, Feb 2026, [KNA](https://www.kenyanews.go.ke/?p=132930)) |
| 15 | Extruded floating tilapia grow-out feed (28–32% CP), ex-mill | 110 | 125 | 150 | KES/kg | SamakGro 4 mm finisher KES 2,900–3,240/25 kg = 116–130/kg; 3 mm grower 3,600 = 144/kg ([SamakGro store](https://take.app/samakgro/p/clzr0xsj9004nirjw3brif1fa), undated); WorldFish USD 1.00–1.24/kg = KES 130–161 ([WorldFish](https://worldfishcenter.org/node/15263)) |
| 16 | Fry/starter/high-protein (35–45% CP) feed | 160 | 200 | 250 | KES/kg | [ESTIMATE]; one retail 35% CP 3 mm listing at KES 209/kg ([Jiji](https://jiji.co.ke/293-poultry-feed)) |
| 17 | Dairy/layers compound feed | 45 | 50 | 60 | KES/kg | ~KES 3,500/70 kg (Feb 2026, [The Star](https://www.the-star.co.ke/counties/central/2026-02-24-raw-material-crunch-threatens-to-push-animal-feed-cost-higher)) |
| 18 | Cage tilapia output, Kenya, 2026 | 30 | 34 | 38 | kt | 28.1 kt in 2025 (KNBS via [Ecofin](https://www.ecofinagency.com/news-agriculture/1703-53851-kenya-s-fish-farming-boom-draws-new-bet-from-victory-farms)) × 1.07–1.35 [ESTIMATE] |
| 19 | Feed conversion ratio, cage tilapia (commercial) | 1.4 | 1.6 | 1.9 | kg feed/kg fish | Trial FCR 1.46–1.51 on Lake Victoria ([WAS 2023 abstract, Kaminski et al.](https://was.org/Meeting/Program/PaperDetail/161632)); commercial losses push it higher [ESTIMATE] |
| 20 | Total Kenya aquafeed demand, 2026 (all buyers) | 50 | 65 | 80 | kt | [ESTIMATE] = cage output × FCR + pond sector (~8–10 kt fish × ~1.5, part on-farm) |
| 21 | of which merchant (non-captive) demand | 20 | 30 | 40 | kt | [ESTIMATE] excludes Victory Farms' ~90% in-house feed ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840)) |
| 22 | Kenya aquaculture output, 2030 | 50 | 80 | 120 | kt | 33.4 kt in 2024 ([Standard](https://www.standardmedia.co.ke/counties/article/2001544285/kenya-finalises-aquaculture-policy-to-boost-fish-production)); Victory Farms alone targets 100 kt by 2030 ([KNA](https://www.kenyanews.go.ke/168926-2/)); [ESTIMATE] |
| 23 | Formal compound feed production, Kenya | 2.2 | 2.5 | 2.8 | Mt/yr | ~2.5 Mt; poultry 60%, dairy 29% ([KNA](https://www.kenyanews.go.ke/?p=169703), date not confirmed) |
| 24 | Sunflower seed price to crusher (context for margin) | 45 | 60 | 80 | KES/kg | FAOSTAT-based farmgate KES 46.86/kg (Jun 2026, [Selina Wamucii](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds)) [UNVERIFIED]; Bungoma buyer KES 100/kg (undated, [African Mirror](https://theafricanmirror.africa/news/kenyas-adaptive-farmers-turn-to-sunflower/)) |
| 25 | CPO import duty in force | 0 | 10 | 10 | % | 10% since 1 Jul 2024; refiners are lobbying for 0% ([Milling MEA](https://millingmea.com/kenyas-edible-oil-prices-set-to-rise-amid-import-duty-dispute/)). Low case = duty scrapped, which removes ~KES 15k/t of protection |

---

## 1. Edible oil

### 1.1 Consumption, imports and the import gap

- **Palm dominates.** USDA: Kenya imported 875,000 t of palm oil in 2024 (8th-largest importer in the world), on track for ~1.0 Mt in 2025, forecast 1.05 Mt in 2025/26, close to the 2020 peak of 1.1 Mt. Palm is >90% of national oil-and-fat consumption. Re-exports are forecast at 90,000 t (2025) and 100,000 t (2026). Malaysia supplies ~90%. Crude was >90% of imports 2019–23, but refined palm's share jumped to 24% in 2024 after the crude duty squeezed refining margins ([OFI Magazine](https://www.ofimagazine.com/news/kenyan-palm-oil-consumption-to-reach-record-high); [Food Business MEA](https://www.foodbusinessmea.com/kenyas-palm-oil-imports-to-hit-1-05-million-tonnes-in-2025-2026-usda/), Jul 2025).
- **AFA quarterly data (quarter to June 2025):** 183,139 t of edible oils worth KES 25.61bn (182,209 t a year earlier). Palm 168,418 t (KES 23bn, down from 172,174 t); **sunflower 3,909 t** (KES 601m, up from 1,773 t); **soy oil 1,671 t** (KES 252m, −32%; suppliers USA, Germany, Uganda) ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)). Implied CIF unit value ≈ KES 136,600/t for palm and KES 153,900/t for sunflower (my calculation).
- **2024 full year (AFA via a secondary site):** palm products 793,539 t (KES 108.8bn, ≈ KES 137k/t); sunflower 8,949 t (KES 1.32bn); soy 6,546 t (KES 1.63bn) ([Tradologie](https://www.tradologie.com/edible-oil-importers/edible-oil-importers-in-kenya/)) [UNVERIFIED]. Ukraine supplied ~6,950 t of crude sunflower/safflower oil in 2024 (same source).
- **2023:** 720,000 t of crude and refined vegetable oil, KES 98.9bn (CS Linturi, [The Star, Mar 2024](https://www.the-star.co.ke/news/infographics/2024-03-27-state-turns-to-local-production-to-cut-sh160bn-edible-oil-import-cost)) [DATED].
- **[CONFLICT] Import bill:** KES 100bn/yr (Trade CS, Feb 2025, [People Daily](https://peopledaily.digital/business/trade-cs-lee-kinyanjui-pushes-for-local-alternatives-to-slash-ksh100b-edible-oil-imports/amp)); CPO "worth KES 130bn" a year ([The Standard](https://thestandard.ke/sports/business/2001515437/edible-oil-processors-rekindle-push-to-scrap-import-duty-tax), 2025); KES 145bn (2022) and claims of KES 150–160bn (Capital FM, KNA Aug 2026) ([Star, Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import); [Capital FM](https://capitalfm.africa/govt-eyes-local-edible-oil-supply-through-sunflower-soybean-farming/)). **My base:** ~KES 105–115bn in 2025. The 2026 bill is likely **KES 120–135bn** [ESTIMATE], because the FAO vegetable-oil index was +18.3% y/y in Sep 2026 (198.6 points; [FAO via Fastmarkets](https://fastmarkets.com/insights/fao-food-price-index-rises-in-september-on-higher-cereal-vegoil-prices-and-benchmark-at-highest-since-november-2022)) while volumes held flat. The 145–160bn figures look like 2022 crisis-price numbers or include soap-grade fats.
- **[CONFLICT] Volume:** AFA and the Ministry say ~600 kt/yr consumed, 90–95% imported ([Star, Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)). An older AFA figure says 900 kt demand with 34% "local production" ([Milling MEA](https://millingmea.com/kenya-steps-up-oilseed-farming-drive-to-cut-import-bill/)). USDA palm imports alone are ~1.0 Mt. Reconciliation [ESTIMATE]: USDA counts industrial palm (stearin for soap and fats) and re-exports. AFA's quarterly series annualises to ~733 kt. The "34% local" almost certainly counts **local refining of imported crude**, not local oilseed. **Base for food-grade oils and fats: ~780 kt (2026), i.e. ~14 kg per capita for ~55m people.**
- **Domestic oilseed-based production is tiny.** Bidco needs >10,000 t/yr of sunflower and soy seed but local farmers supply ~5,000 t ([KNA](https://www.kenyanews.go.ke/?p=23808), date uncertain). Sunflower seed production has been put at ~6,000 t ([Selina Wamucii/FAOSTAT](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds)) [UNVERIFIED; FAOSTAT likely undercounts informal cross-border seed]. Kajiado crushers buy Tanzanian seed across the border ([Nation](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502)). **[ESTIMATE] Local oil from local oilseed (sunflower, cotton, soy, coconut, canola) is probably <30–50 kt, i.e. <5% of consumption.**
- **Policy:** In March 2026 the Agriculture CS launched a sunflower and soybean drive; targets are at least 50% local supply by 2028 and halving imports 2026–2030 ([Star](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import); [KNA, Aug 2026](https://www.kenyanews.go.ke/sunflower-soybean-initiative-to-curb-edible-oil-import-bill/)). AFA's KES 981m Edible Oil Crops Promotion Project (from Jul 2023) covers sunflower, canola, soy and coconut ([Milling MEA](https://millingmea.com/kenya-accelerates-edible-oil-crops-farming-to-cut-imports-led-by-afa/)). **Judgement:** the 2028 target is not credible, because it would need roughly 1.1 Mt of sunflower seed. It does give a policy tailwind for seed, extension and offtake support.

### 1.2 Prices

- **Retail:** national average for salad oil KES 358.09/L in Jul 2026 (KNBS), up from 342.98 in Dec 2025 and 21.75 below the Sep 2022 peak of 379.84 ([Business Daily](https://www.businessdailyafrica.com/bd/economy/cooking-oil-prices-climb-back-to-highs-of-2022-crisis-5548020)). Streamline also reports KES 358 ([Streamline](https://streamlinefeed.co.ke/news/kenya-cooking-oil-prices-hit-sh358-per-litre)) [UNVERIFIED secondary].
- **State-linked bulk benchmark:** KNTC "Mama Pima" dispensers sell to vendors at KES 185/L, recommended retail KES 210/L (Jul 2026, [Kenya Times](https://thekenyatimes.com/business/govt-unveils-mama-pima-cooking-oil-dispenser/)). This is close to my CPO landed estimate of KES 169/L plus refining, so it is effectively a cost-plus price for loose olein.
- **Refiner margin evidence:** the COMESA Competition Commission found Kenyan manufacturers sold at an average KES 333/L against a "fair price" of KES 274/L, an alleged KES 67.7bn overcharge ([Khusoko, Dec 2024](https://khusoko.com/2024/12/11/oil-firms-overcharged-kenyans-by-ksh-67-7-billion/)) [DATED]. This points to an oligopolistic refining/branding layer with fat gross margins. Those margins are the prize, but also the incumbents' weapon.
- **Global benchmarks (Sep–Oct 2026):** CPO ~RM4,500–4,650 (Jun 2026 futures; [Bernama](https://www.bernama.com/lite/news.php?id=2544958)); RBD olein FOB Malaysia USD 1,252.5/t ([Fastmarkets](https://www.fastmarkets.com/insights/correction-to-price-for-refined-bleached-deodorized-palm-olein-on-september-8-2026/)); CSFO FOB Black Sea USD 1,265–1,275/t, falling for a third month in Sep 2026, while palm rose ([Commodity-Board](https://commodity-board.com/russia-takes-the-wheel-in-sunflower-oil-what-it-means-for-prices)). **Sunflower's premium over palm is ~USD 100–150/t FOB.**
- **Landed import parity [ESTIMATE]:** CPO ≈ **USD 1,430/t ≈ KES 185k/t ≈ KES 169/L**; CSFO ≈ **USD 1,610/t ≈ KES 209k/t ≈ KES 190/L**. Assumptions: freight ~USD 60 (Malaysia) and ~100 (Black Sea, via Red Sea or Cape); 10% CET duty; IDF + RDL ~5.5% (verify the current Finance Act rates); port and clearing ~USD 30/t. **Cross-check:** AFA's Q2-2025 CIF unit value of ~KES 137k/t, lifted ~18% for 2026 prices, gives ~KES 161k/t CIF, consistent with ~KES 180–190k/t duty-paid.
- **Duty structure:** CPO 10% since 1 Jul 2024 under the EAC CET (from 0%), and refiners petition for removal ([Milling MEA](https://millingmea.com/kenyas-edible-oil-prices-set-to-rise-amid-import-duty-dispute/); [Business Daily](https://www.businessdailyafrica.com/bd/economy/edible-oil-processors-petition-treasury-over-import-duty-tax-4709318)). Refined oils: 25% CET per Bidco ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/bidco-pushes-for-review-of-25pc-duty-rule-for-eac-exports-2120464)) [DATED; some 2022 CET-review references suggest a 35% band, so verify]. Oilseeds (soy, cotton, sunflower seed) carry 10% CET ([Milling MEA](https://millingmea.com/kenyan-feed-millers-face-soybean-shortage-as-prices-surge-by-over-us0-12/)).
- **EAC rules of origin:** oils refined from imported crude are treated as foreign and pay 25% when crossing EAC borders ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/bidco-pushes-for-review-of-25pc-duty-rule-for-eac-exports-2120464)) [DATED]. **Oil crushed from EAC-grown seed should qualify for duty-free intra-EAC trade.** That is a structural export advantage for a local crusher over palm refiners (verify with KRA/EAC).

### 1.3 Refiners and sourcing

| Firm | Known facts | Sourcing |
|---|---|---|
| Bidco Africa (Thika) | Largest refiner; also Bidco Uganda (Kalangala palm, 40,000 ha NOPP, USD 200m invested by 2024, [Uganda Invest](https://ugandainvest.go.ug/?p=579)) | Mainly imported CPO; local sunflower/soy contract farming around Nakuru; needs >10 kt seed, gets ~5 kt locally ([KNA](https://www.kenyanews.go.ke/?p=23808)) |
| Pwani Oil (Mombasa) | Fresh Fri, Salit; shut its plant in 2022 for lack of dollars ([The Star, 2022](https://www.the-star.co.ke/news/2022-06-06-pwani-oil-shuts-plant-blames-lack-of-dollars)) [DATED] | Imported CPO |
| Kapa Oil Refineries | Oils, margarine, soaps ([Fuzu](https://www.fuzu.com/company/kapa-oil-refineries)) | Imported CPO (no detail found) |
| Menengai Oil Refineries (Nakuru) | Named as a major importer/refiner ([Milling MEA](https://millingmea.com/?p=2007624)) [DATED] | Imported CPO; no sourcing detail found |
| Edible Oil Products / Golden Africa / Savannah (Zuri) | Savannah's Zuri brand imports Polish sunflower oil ([Zuri](https://zuri.odoo.com/)) | Imported |

- **Do refiners buy local crude, and at what discount?** No public evidence of formal offtake pricing was found. **[ESTIMATE]** Refiners' alternative is CPO at ~KES 185k/t. For crude sunflower they will pay up to sunflower import parity (~KES 209k/t) only if they run a dedicated soft-oil line. Small, irregular lots of local crude (high FFA, phosphatides, moisture) typically trade **5–12% below the relevant import parity**, so the realistic local crude price is **KES 180–195k/t**. A crusher that refines and packs its own sunflower oil keeps the ~KES 50–80k/t refining-and-brand margin, but must build distribution against Bidco/Pwani/Kapa.

### 1.4 Consumer preference (sunflower vs palm)

- No Kenyan consumer survey was found. Palm is >90% of oils and fats consumed ([OFI/USDA](https://www.ofimagazine.com/news/kenyan-palm-oil-consumption-to-reach-record-high)). Imported sunflower oil more than doubled y/y in Q2 2025, but from a ~2% base ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)). Euromonitor covers the topic but is paywalled ([Euromonitor](https://www.dri.co.jp/auto/report/euromonitor/221103-edible-oils-in-kenya.html)).
- **Judgement [ESTIMATE]:** demand is very price-elastic, with retail near its 2022 record. The "health" sunflower segment is an urban middle-class niche, perhaps 5–10% of volume (40–80 kt), and can carry a 10–20% retail premium. A local sunflower oil should be priced at **parity to a modest premium over palm olein**, not at European sunflower prices.

### 1.5 EAC export potential

- **Tanzania:** needs ~732 kt/yr of edible oil; local output fluctuates 100–300 kt, so the deficit averages ~400 kt. Its new 10-year National Edible Oil Strategy targets self-sufficiency and net exports by 2035, prioritising sunflower and palm ([The Citizen, 2025](https://thecitizen.co.tz/tanzania/business/how-new-edible-oil-strategy-aims-to-lower-sh500-6-billion-import-bill-5542338)). Older figures: 570 kt demand vs 205 kt produced ([The Citizen](https://thecitizen.co.tz/tanzania/business/tanzania-eyes-edible-oils-market-3649214)) [DATED]. Tanzania is also Kenya's main source of sunflower cake and informal seed. In the medium term it is a **competitor and a feedstock source**, more than a market.
- **Uganda:** no import data found. Bidco Uganda's Kalangala palm gives Uganda an EAC-origin palm supply that can enter Kenya competitively (rules-of-origin treatment needs verifying).
- **Judgement:** EAC export of oil is an upside, not a base case. Cake and aquafeed exports to Uganda and Tanzania face De Heus and Tunga plants located inside those countries (section 3).

---

## 2. Oilseed cake and meal

### 2.1 Prices (thin data; mostly [DATED] or [UNVERIFIED])

| Product | Data point | Date | Source |
|---|---|---|---|
| Sunflower cake | KES 25 → 35/kg after the Zambia export ban | ~2022–23 [DATED] | [Business Daily](https://www.businessdailyafrica.com/bd/markets/commodities/zambia-material-export-sends-feed-prices-record-high-3531764) |
| Sunflower cake | KES 40/kg (50 kg bags, Nairobi Industrial Area); KES 70/kg retail 1 kg | 2026 listing [UNVERIFIED] | [Jiji](https://jiji.co.ke/viwandani-makadara/feeds-supplements-seeds/sunflower-seed-cake-dTh5NuF0GdsvaWJ01XlkOR3T.html) |
| Soybeans | KES 75 → 100/kg; AKEFEMA KES 97 → 115/kg | Aug 2024 [DATED] | [The Star](https://the-star.co.ke/news/star-farmer/2024-08-06-feed-millers-stare-at-shortage-as-soybean-prices-surge-by-over-sh15); [Milling MEA](https://millingmea.com/kenyan-feed-millers-face-soybean-shortage-as-prices-surge-by-over-us0-12/) |
| Soya (meal/beans) | KES 65 → 130/kg after the Zambia ban | ~2022–23 [DATED] | [Business Daily](https://www.businessdailyafrica.com/bd/markets/commodities/zambia-material-export-sends-feed-prices-record-high-3531764) |
| Soybean meal | KES 90,000–120,000/t to feed mills | 2026 [UNVERIFIED] | [Indexbox](https://www.indexbox.io/store/kenya-soya-beans-market-analysis-forecast-size-trends-and-insights/) |
| Soybean meal, global | CBOT Dec-26 ~USD 357/short ton ≈ USD 394/t; Oct-26 ~USD 299/short ton (Jun snapshot) | 2026 | [Feedstuffs](https://www.feedstuffs.com/commodities/soybean-meal); [Barchart](https://www.barchart.com/futures/quotes/ZMV26) |
| Cottonseed cake | Shortages reported; no price | [DATED] | [Nation](https://www.nation.africa/kenya/business/blow-for-farmers-as-costs-of-feeds-hit-record-high-3532110) |
| Omena (human grade) | 2 kg tin >KES 400 wholesale (doubled); sack >KES 20,000 | Feb 2026 | [KNA](https://www.kenyanews.go.ke/?p=132930) |

**[ESTIMATE] Price logic.** Kenyan non-GM SBM trades at roughly 1.8–2.2× CBOT (≈ KES 51k/t at CBOT) because of the GMO restrictions, regional sourcing (Zambia, Malawi, Uganda), road freight and 10% CET. Base **KES 95/kg**. Sunflower cake is priced at ~40–45% of SBM on protein and fibre, base **KES 40/kg**. Cake prices are strongly countercyclical to regional export bans (Zambia, Malawi, Tanzania), so model a high case of +25–30%.

### 2.2 Buyers and import dependence

- AKEFEMA: >80% of critical feed ingredients (soybean, sunflower meal, cottonseed meal) are imported ([KNA](https://www.kenyanews.go.ke/?p=169703)). Another report says 80% comes from Uganda, Tanzania, Malawi and Zambia; another says >60% ([Milling MEA](https://millingmea.com/kenya-feed-shortages-spur-push-for-gm-sourced-raw-materials-to-ease-crisis/)) [CONFLICT 60% vs 80%].
- Feb 2026: AKEFEMA warned of shortages of maize germ, soybean meal, canola and sunflower cake ([The Star](https://www.the-star.co.ke/counties/central/2026-02-24-raw-material-crunch-threatens-to-push-animal-feed-cost-higher)). Jul 2026: millers at 50–60% capacity ([The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)). Sep 2026: duty-free import of 360,000 t of yellow maize planned ([GNA](https://gna.org.gh/2026/09/kenya-mulls-duty-free-maize-imports-amid-shortage/)). Jul 2026: the government announced a National Feed Strategy with a reported KES 465bn ([The Star](https://www.the-star.co.ke/news/2026-07-16-government-to-set-aside-sh465-billion-to-tackle-animal-feed-crisis)) [UNVERIFIED amount; may be a typo for 4.65bn].
- **Buyers of cake:** >300 feed manufacturers (2024); poultry is 60% and dairy 29% of commercial feed ([KNA](https://www.kenyanews.go.ke/?p=169703)). Dairy and layer mashes are the main sinks for sunflower and cotton cake. Fish and broiler feeds need SBM or fishmeal.
- **Soybean meal import volume:** no 2025 tonnage found (USDA GAIN KE2026-0006 should have it; [FAS](https://www.fas.usda.gov/data/kenya-grain-and-feed-annual-10)). **[ESTIMATE]** 2.5 Mt of compound feed × ~8–12% SBM inclusion = **200–300 kt/yr of soy meal or bean equivalent demand**, mostly imported regionally, plus ~150–250 kt of sunflower and cotton cake.
- **GMO status:** a Court of Appeal conservatory order (Mar 2025) bars the import or commercialisation of GE products pending the Kenya Peasants League appeal ([Citizen](https://citizen.digital/article/blow-to-govt-as-court-of-appeal-bars-importation-of-gmos-n358801); [OFI](https://www.ofimagazine.com/news/kenyas-court-of-appeal-issues-injunction-on-genetically-engineered-products)). Judgment was scheduled for 24 Apr 2026 ([KNA](https://www.kenyanews.go.ke/?p=159340)), and **the outcome was not found**. While the ban holds, GM SBM from Argentina, Brazil or the US is excluded and the price of local or non-GM protein stays high. That is favourable to a local soy/sunflower crusher, but **a court ruling lifting the ban is the key downside price risk for cake** (−20–30% on SBM [ESTIMATE]).

---

## 3. Animal feed and aquafeed

### 3.1 Formal feed industry

- ~2.5 Mt/yr of compounded feed (poultry 60%, dairy 29%, rest pig, aqua and other) ([KNA](https://www.kenyanews.go.ke/?p=169703)). Kenya meets ~40% of 55 Mt dry-matter livestock feed needs, a 33 Mt deficit mostly in forage, not compound feed ([The Star, Jul 2026](https://www.the-star.co.ke/news/2026-07-16-government-to-set-aside-sh465-billion-to-tackle-animal-feed-crisis)). Feed is 60–70% of livestock production cost.
- **Price:** ~KES 3,500 per 70 kg of dairy/layers feed (Feb 2026), i.e. ~KES 50/kg. Older range KES 3,500–4,500 (2024) ([The Star](https://www.the-star.co.ke/counties/central/2026-02-24-raw-material-crunch-threatens-to-push-animal-feed-cost-higher)).
- **Market value [ESTIMATE]:** 2.5 Mt × KES 50–55/kg ≈ **KES 125–140bn/yr**. Utilisation of 50–60% means **ample existing pelleting capacity**. A new mash/pellet line for poultry or dairy feed adds little; **the scarce asset is protein**.

### 3.2 Aquaculture and aquafeed demand

- **Output:** aquaculture 33,423 t in 2024 (KES 9.9bn), +5%, out of 168,424 t total fish; cages 76.4% (25,547 t) ([Standard](https://www.standardmedia.co.ke/counties/article/2001544285/kenya-finalises-aquaculture-policy-to-boost-fish-production)). KeFS gives 33,289 t [minor CONFLICT]. Commercial cage output rose from 13,700 t (2021) to **28,100 t (2025) from ~7,000 cages** (KNBS via [Ecofin](https://www.ecofinagency.com/news-agriculture/1703-53851-kenya-s-fish-farming-boom-draws-new-bet-from-victory-farms); [SeafoodSource](https://www.seafoodsource.com/news/kenya-s-senate-petitioned-to-control-the-spread-of-cage-fish-farming-in-lake-victoria)), a **19.7%/yr CAGR**. A June 2026 report says aquaculture is ">40,000 t" ([The Star](https://www.the-star.co.ke/counties/nyanza/2026-06-30-africas-fish-supply-is-falling-behind-surging-demand-fao)) [UNVERIFIED year].
- **Cage numbers and counties:** 1,663 (2016) → 3,696 (2019 frame survey; Siaya 2,989 (81%), Homa Bay 479, Busia 120, Kisumu 85, Migori 23) ([Standard](https://standardmedia.co.ke/article/2001342622/why-lake-victoria-could-be-running-out-of-fish); [Business Daily](https://www.businessdailyafrica.com/bd/data-hub/siaya-tops-uptake-of-high-yielding-cage-fishing-2223742)) [DATED] → ~7,000 (2025). **Siaya and Homa Bay are the core feed-delivery geography**, with a mill or depot ideally at or near Kisumu, Bondo or Homa Bay.
- **FCR:** 1.46–1.51 in a Lake Victoria cage trial at 2.9–5.9 kg/m³, 138 days, ~500 g harvest ([WAS abstract](https://was.org/Meeting/Program/PaperDetail/161632); [Stirling](https://dspace.stir.ac.uk/handle/1893/35666)). Commercial base 1.6 [ESTIMATE].
- **Feed demand [ESTIMATE]:** cages 28.1 kt × 1.4–1.9 = **39–53 kt (2025)**; ponds ~8 kt fish × ~1.5 at partial commercial-feed use = ~5–10 kt. **Total ~45–60 kt in 2025, ~50–80 kt in 2026.** An older review estimated 34 kt demand and ~7 kt imported ([FAO AGRIS review](https://agris.fao.org/search/zh/records/647470b8425ec3c088f1d16d); [The Fish Site](https://thefishsite.com/articles/how-can-kenya-fulfil-its-untapped-aquaculture-potential-proscovia-alando)) [DATED], which is consistent with the lower 2021–22 output.
- **Captive vs merchant (critical):** Victory Farms (Homa Bay) produces ~18,000 t/yr ([ASC/various](https://thefishsite.com/es/articles/victory-farms-raises-35-million-to-fuel-east-african-tilapia-expansion)), or 25,000 t ([KNA](https://www.kenyanews.go.ke/168926-2/)), targeting 30,000 t in 2026 ([WeAreAquaculture](https://weareaquaculture.com/news/finance/tilapia-producer-victory-group-secures-15m-follow-on-investment-from-agdevco)) and 100,000 t by 2030 [CONFLICT on baseline]. It makes ~90% of its feed in-house, cutting feed cost ~30% ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840)). **If Victory Farms is 18–25 kt of KNBS's 28.1 kt cage output, then 65–90% of cage feed demand is captive.** The **merchant market is only ~20–40 kt** (smaller cage operators, ponds, Uganda/Tanzania spill-over). Either KNBS undercounts or Victory Farms dominates. This is the single biggest uncertainty for the feed business case.
- **Imported vs locally extruded share [ESTIMATE]:** before Tunga's 2026 expansion, ~20% imported (7 kt of 34 kt, [DATED]). Imports come from Aller Aqua's Zambia and Egypt plants via AquaRech, which has depots in Kakamega, Kisii, Nyamira, Migori, Bondo, Homa Bay, Siaya, Vihiga, Kirinyaga and Busia ([Aller Aqua](https://www.aller-aqua.com/about/news/aller-aqua-partners-with-aquarech-to-ensure-high-quality-quality-feeds-reach-all/)), plus Israeli feed. Jewlet imports all its grow-out pellets ([The Fish Site](https://thefishsite.com/articles/helping-to-generate-east-african-aquaculture-success-enos-were-jewlet-fish-farms-kenya)). The 2026 local extrusion build-out (below) will push the imported share toward ~10% [ESTIMATE].
- **Prices:** SamakGro (Victory Farms' feed arm) retail list: 4 mm finisher Low-Pro KES 2,900, Plus 3,000, High-Pro 3,240 per 25 kg (KES 116–130/kg); 3 mm grower KES 3,600 (KES 144/kg) ([SamakGro](https://take.app/samakgro/p/clzr0xsj9004nirjw3brif1fa)) [undated]. WorldFish puts commercial feed at USD 1.00–1.24/kg (KES 130–161) and >60% of production cost ([WorldFish](https://worldfishcenter.org/blog/feed-holding-kenyas-aquaculture-boom-back)). A 35% CP 3 mm retail listing is at KES 209/kg ([Jiji](https://jiji.co.ke/293-poultry-feed)) [UNVERIFIED]. **Base ex-mill grow-out price KES 125/kg.**

### 3.3 Competitors and capacity (aquafeed)

| Player | Location | Capacity / facts | Source |
|---|---|---|---|
| Tunga Nutrition (Skretting/Nutreco + Unga JV), brands Skretting & Fugo | Nairobi | New extrusion plant took capacity from 24,000 to **45,000 t/yr**; inaugurated ~Feb 2026; also targets UG, TZ and RW | [WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi) |
| Unga Farm Care (Fugo) | Nairobi; Homa Bay launch | Floating tilapia feed "cheaper than imported"; original 2017 plant 5,000 t | [Aquafeed.com](https://aquafeed.com/newsroom/news/kenya-unga-farm-care-launches-fish-feed-to-improve-tilapia-business-in-homa-bay); [Feed Planet](https://feedplanetmagazine.com/blog/new-fish-feed-plant-in-kenya-780) [DATED] |
| SamakGro (Victory Farms + Maxim Agri + Gatsby Africa) | Naivasha; new plant at Olkaria Green Energy Park | Existing mill (~35 kt ingredients/yr); new **USD 3.95m, 8 t/h (~40–50 kt/yr) geothermal-powered plant** announced Jul 2026, commissioning date undisclosed. Sells to third parties | [The Fish Site](https://thefishsite.com/es/articles/african-aquaculture-leaders-join-forces-to-build-feed-mill-maxim-agri-victory-farms-gatsby-africa); [Food Business MEA](https://www.foodbusinessmea.com/?p=2161573); [ThinkGeoEnergy](https://www.thinkgeoenergy.com/fish-feed-producer-invests-in-geothermal-powered-green-energy-park-in-kenya/?amp=1) |
| Sigma Feeds | Nairobi | Fish feed since 2010; multi-species | [Milling MEA](https://millingmea.com/sigma-feeds/) |
| Aller Aqua (imports) | Zambia/Egypt plants; Kisumu distribution via AquaRech | Largest fish-feed producer in Africa | [Aller Aqua](https://www.aller-aqua.com/about/news/aller-aqua-partners-with-aquarech-to-ensure-high-quality-quality-feeds-reach-all/) |
| De Heus Uganda | Njeru/Jinja, Lake Victoria | **50,000 t/yr (2023 plan) → "up to 100,000 t" at full capacity**; opened ~2025 | [De Heus](https://www.deheus.com/csr-stories/how-a-de-heus-plant-can-support-fish-farming-in-uganda-and-help-feed-the-nation); [Aquafeed.com](https://aquafeed.com/newsroom/news/de-heus-officially-opens-fish-feed-factory-in-uganda) [CONFLICT on capacity] |
| Tunga Uganda | Kampala (former flour mill) | Animal feeds and concentrates | [WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi) |
| Ugachick | Gayaza, Uganda | USD 1.2m floating fish-feed plant (2010); current status unknown | [Poultry World](https://www.poultryworld.net/home/ugachick-starts-fish-feed-plant/) [DATED] |
| Jewlet | Kenya | Hatchery and starter feed; imports grow-out pellets | [The Fish Site](https://thefishsite.com/articles/helping-to-generate-east-african-aquaculture-success-enos-were-jewlet-fish-farms-kenya) |
| Isinya Feeds, "Ranaan" | — | No aquafeed data found | — |

**Judgement:** regional extruded-feed capacity (Tunga 45 kt + SamakGro ~40–80 kt + De Heus 50–100 kt + Aller Aqua imports) already exceeds Kenyan **merchant** demand (~20–40 kt) several times over, and roughly matches total regional demand. **A new stand-alone merchant aquafeed extruder in 2027–28 would enter an over-supplied, price-competitive market against multinationals.** The defensible angles are:
- (i) a **cost advantage from in-house protein** (own soy/sunflower meal);
- (ii) **integration with own cages** (Victory Farms' model, a 30% feed saving);
- (iii) a **toll or offtake arrangement** supplying meal to Tunga, SamakGro or De Heus, rather than competing with them.

Uganda and Tanzania: Tanzania's commercial fish-feed use rose from 1,182 t (2021) to 6,211 t (2023), with >50% imported ([UNCST](https://nru.uncst.go.ug/bitstreams/4670621e-4062-4039-9bc1-f274e4da36df/download)) [DATED]. Uganda's sector was "completely dependent on imported feeds" before De Heus ([RVO roadmap](https://www.rvo.nl/files/file/2022-05/Aquaculture-Road-Map-Uganda-Opportunities-in-the-aquaculture-value-chain.pdf)) [DATED].

---

## 4. Demand growth to 2030

| Item | 2025 | 2026 | 2030 base | 2030 range | Basis |
|---|---|---|---|---|---|
| Edible oil consumption (kt) | ~755 | ~780 | ~895 | 760–1,050 | 3.5%/yr base [ESTIMATE]; USDA palm imports 875 kt (2024) → 1.05 Mt (2025/26) ([USDA via Milling MEA](https://millingmea.com/kenyas-palm-oil-imports-to-hit-1-05-million-tonnes-in-2025-2026-usda/)) |
| Edible oil import bill (KES bn) | 105–115 | 120–135 | 130–150 | 100–180 | Price × volume [ESTIMATE] |
| Cage tilapia output (kt) | 28.1 | ~34 | ~65 | 45–110 | 19.7% historic CAGR, tapering; social licence (Senate petition) is a cap ([SeafoodSource](https://www.seafoodsource.com/news/kenya-s-senate-petitioned-to-control-the-spread-of-cage-fish-farming-in-lake-victoria)) |
| Total aquaculture (kt) | ~38 | ~42 | ~80 | 50–120 | Government: total fish 168 kt → 450 kt ([The Star, Mar 2026](https://www.the-star.co.ke/news/2026-03-24-ps-njagi-how-well-turn-the-tide-to-hit-sh300bn-blue-economy-target)); older target of 400 kt aquaculture by 2030 is not credible |
| Aquafeed demand (kt) | 45–60 | 50–80 | ~125 | 75–190 | Output × FCR 1.6 |
| Merchant aquafeed demand (kt) | 15–30 | 20–40 | ~45 | 25–80 | Depends on Victory Farms' captive share |
| Formal compound feed (Mt) | ~2.5 | ~2.5 | ~3.0 | 2.7–3.3 | [ESTIMATE] 3–5%/yr from poultry; 2026 drought dip |

The fish supply gap is put at 50 kt rising to 75 kt by 2030 at constant per-capita consumption ([Farm Africa, 2024](https://www.farmafrica.org/wp-content/uploads/2024/07/aquaculture-for-jobs-incomes-and-food-security.pdf)) versus >400 kt (KNBS Economic Survey 2024, via WorldFish) [CONFLICT]. Fish prices rose 16% in 2025 (Economic Survey 2026, [Standard](https://www.standardmedia.co.ke/business/article/2001546576/knbs-fish-vegetable-prices-jump-by-double-digits-despite-easing-inflation)), evidence of excess demand.

---

## 5. Market sizing (TAM / SAM / SOM)

### (a) Crude and refined oil

| Level | Definition | Volume | Value (2026, base prices) |
|---|---|---|---|
| **TAM** | All Kenyan edible oil and fat consumption | ~780 kt (650–950) | ~KES 156bn at wholesale ~KES 200k/t; ~KES 305bn at retail (KES 358/L) |
| | + EAC deficit (Tanzania ~400 kt; Uganda n/a) | +400 kt | +~KES 75bn [ESTIMATE] |
| **SAM** | Crude/refined **soft oils** (sunflower, soy, canola) that a Kenyan crusher can realistically displace: current soft-oil imports (~16 kt in 2024) + local soft oil (~30–50 kt) + premium-segment switching from palm (~5–10% of market) | **60–100 kt** | **KES 12–21bn** at KES 200–210k/t |
| **SOM** | One 150–300 t/day seed crusher (sunflower ~38–42% oil, expeller + solvent ~36–38% recovery; soy ~18%) at 75–85% utilisation | **~10–25 kt oil/yr** by year 3–5 (~1.5–3% of national consumption; 15–25% of SAM) | **KES 2–5bn/yr** |

**Binding constraint:** seed, not demand. 25 kt of sunflower oil needs ~65–70 kt of seed, more than 10× Kenya's recorded sunflower output. It requires an outgrower programme of ~45–60k ha at 1.2–1.5 t/ha [ESTIMATE] and/or Tanzanian/Ugandan seed imports at 10% CET. Seed availability, not oil offtake, should set plant size.

### (b) Cake and finished feed

| Level | Definition | Volume | Value (2026, base prices) |
|---|---|---|---|
| **TAM** | Kenyan formal compound feed | ~2.5 Mt | ~KES 125–140bn |
| | of which oilseed meals/cakes used by millers | ~350–550 kt [ESTIMATE] | ~KES 20–35bn |
| | Aquafeed, all Kenyan buyers | 50–80 kt | KES 6–10bn |
| **SAM** | (i) Merchant protein-meal sales to Kenyan millers (non-GM SBM + sunflower cake) | ~350–550 kt | KES 20–35bn |
| | (ii) Merchant extruded aquafeed, Kenya + nearby Uganda/Tanzania lake shores | 30–60 kt | KES 4–8bn |
| **SOM** | Cake from own crush (sunflower ~55–58% of seed; soy ~78%) | ~25–55 kt | KES 1.0–3.5bn (sunflower cake at 40/kg; SBM at 95/kg) |
| | Own-brand aquafeed by year 3–5 (10–25% merchant share) | 5–12 kt | KES 0.6–1.5bn |
| | Aquafeed if integrated with own cages (captive) | +5–15 kt | Transfer-priced; value shows up in fish margin |

**Judgement on product mix:**
- Sunflower cake is a **dairy and layer** ingredient. Its high fibre limits tilapia grow-out inclusion to ~10–20% [ESTIMATE], so a **sunflower crusher does not by itself make a competitive fish feed**.
- For aquafeed and broilers, a **soybean** line (full-fat extrusion or expeller SBM) is the better protein play, but soy oil yield is only ~16–18%. The business then becomes a meal business with oil as a by-product.
- A plant that can switch between sunflower and soy is recommended for the model [ESTIMATE].

---

## 6. Quick margin sanity check [ESTIMATE, for the modelling team]

Sunflower, per tonne of seed at KES 60/kg: oil 0.36 t × KES 190k = 68.4k, plus cake 0.56 t × KES 40k = 22.4k, gives revenue **KES 90.8k** against seed cost KES 60k. **Gross crush margin ≈ KES 31k/t of seed (~34%)** before processing (~KES 6–10k/t), freight and financing. At seed KES 80/kg the margin falls to ~KES 11k/t and the crush is marginal. **The model is very sensitive to the seed–oil price spread; run a 2-D sensitivity on seed price × CPO parity.**

---

## 7. Gaps and uncertainties

1. **Total edible oil consumption** is uncertain by ±25% (600 kt AFA vs ~1 Mt USDA palm imports). The 34% "local production" claim almost certainly counts refining of imported crude. Get USDA GAIN *Kenya Oilseeds and Products Annual 2026* and KRA HS 1507–1515 data.
2. **No public price at which refiners buy local crude sunflower oil.** The 5–12% discount is my estimate. Get quotes from Bidco, Menengai and Kapa procurement before finalising.
3. **Cake and meal prices for 2025–26 are largely unsourced.** The best data are 2022–24 or marketplace listings. Get an AKEFEMA price sheet or quotes from 3–4 Nairobi/Nakuru millers.
4. **Victory Farms' share of KNBS cage output** (18–30 kt vs 28.1 kt total) decides whether the merchant aquafeed market is ~20 kt or ~40+ kt. This is the largest single swing factor for the feed mill.
5. **Aquafeed over-capacity:** Tunga 45 kt (2026), SamakGro new 8 t/h plant, and De Heus 50–100 kt in Uganda. Their actual utilisation and pricing behaviour are unknown.
6. **GMO litigation:** the outcome of the 24 Apr 2026 Court of Appeal judgment was not found. If the ban is lifted, SBM prices could fall sharply and erode the cake/meal economics.
7. **Duty regime:** the CPO duty could be removed (refiners are lobbying), which would cut local crude's protection by ~KES 15–18k/t. The refined-oil CET (25% vs 35%), the crude sunflower band, IDF/RDL rates and EAC rules-of-origin treatment of locally crushed oil all need checking with KRA and the EAC gazette.
8. **Seed supply:** no reliable data on Kenyan sunflower or soy area, yield or price in 2025–26. Tanzania's new self-sufficiency strategy could restrict seed and cake exports to Kenya.
9. **Consumer preference:** no survey found. The sunflower premium segment size (5–10%) is my estimate.
10. **Tilapia farmgate price:** no reliable 2026 figure (KES 300–500/kg retail per weak sources), which matters for the farmers' ability to pay for feed.
11. **Uganda edible oil imports and Uganda/Tanzania aquafeed prices:** not found.
12. Source dating: several KNA pages show today's date in the header rather than the publication date, so the dates of some KNA-sourced figures (2.5 Mt feed, Bidco seed need) are uncertain.
