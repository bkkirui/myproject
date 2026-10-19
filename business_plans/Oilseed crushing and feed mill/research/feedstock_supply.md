# Feedstock supply: oilseeds for an integrated crusher and feed mill (Kenya, Lake Victoria focus)

*Agronomy and supply-chain workstream. Prepared 19 Oct 2026. FX: KES 129.8/USD ([macro notes](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_macro_investment_climate.md)). Implied cross rates from the price sources: about TZS 2,370/USD and UGX 3,790/USD. These are derived from Selina Wamucii's USD/local-currency pairs and are approximate.*

**Conventions.** Each fact carries a source URL and a date. **[ESTIMATE]** marks my own figure, with its reasoning. **[DATED]** marks evidence from before 2025, or with no publication date shown. **[CONFLICT]** marks disagreement between sources. Most web pages could not be fetched directly (DNS errors), so many figures come from search-result extracts. Kenya News Agency (KNA) page headers often show crawl dates rather than publication dates, so a KNA date is treated as uncertain unless the content dates itself.

**Reference plant.** Unless stated otherwise, volumes refer to a 20,000 t/yr seed crusher. That is about 67 t/day over 300 days. It sits in western Kenya (Kisumu/Busia corridor), near the Lake Victoria cage farms and the Uganda supply. The volumes scale linearly. Section 9 explains why a larger plant is not supportable on current supply.

---

## 0. Key assumptions for the model

| Parameter | Low | Base | High | Unit | Source / basis |
|---|---|---|---|---|---|
| **Kenya sunflower farmgate price (spot)** | 33 | 47 | 60 | KES/kg | Low: Bidco KES 33 [DATED] ([KNA](https://www.kenyanews.go.ke/?p=23808)). Base: FAOSTAT-based KES 46.86, Jun 2026 ([Selina Wamucii](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds)). High: canola parity KES 60, Mar 2026 ([CPM](https://www.cpm-magazine.co.uk/wp-content/uploads/sites/9/2026/03/066-68-Kenya-March-26.pdf)). |
| Kenya sunflower contract price needed to hold outgrowers | 45 | 52 | 65 | KES/kg | [ESTIMATE]: spot base plus a 10% premium. It must beat Tanzanian buyers pulling Kajiado seed across the border ([Nation, mid-2026](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502)) and must clear the KES 25-50 "won't plant" band ([KNA](https://www.kenyanews.go.ke/nakuru-county-government-embarks-on-promoting-oil-crop-farming-to-cut-cooking-oil-imports/), [DATED]). |
| Tanzania sunflower farmgate | 27 | 35 | 47 | KES/kg | US$0.21 = TZS 497, Jun 2026 ([Selina TZ](https://www.selinawamucii.com/insights/prices/tanzania/sunflower-seeds/)). TZS 622 in 2021 ([UDOM](https://repository.udom.ac.tz/items/8d88b37b-488e-4af0-baef-4b622430929f/full), [DATED]). TZS 850 ([Citizen](https://www.thecitizen.co.tz/tanzania/business/-why-sunflower-has-economic-potentials-locally-and-globally-3529182), [DATED]). |
| Uganda sunflower farmgate | 22 | 32 | 41 | KES/kg | US$0.17 = UGX 645 export unit value, Aug 2026 ([Selina UG](https://www.selinawamucii.com/insights/prices/uganda/sunflower-seeds/)). UGX 1,200 farmgate in Adjumani ([Monitor](https://www.monitor.co.ug/uganda/magazines/farming/adjumani-farmers-ask-govt-to-regulate-sunflower-price-4085558), [DATED]). |
| Kenya soybean farmgate | 45 | 70 | 115 | KES/kg | Base: KES 70, Homa Bay, 23 Jul 2026 ([Standard](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)). Low: Bidco KES 45 [DATED]. High: AKEFEMA KES 115, Aug 2024 ([Star](https://the-star.co.ke/news/star-farmer/2024-08-06-feed-millers-stare-at-shortage-as-soybean-prices-surge-by-over-sh15), [DATED]). |
| Canola (rapeseed) contract price | 40 | 60 | 65 | KES/kg | Agventure guaranteed price about KES 60/kg, Mar 2026 ([CPM](https://www.cpm-magazine.co.uk/wp-content/uploads/sites/9/2026/03/066-68-Kenya-March-26.pdf)). KES 40 is an older figure ([KNA](https://www.kenyanews.go.ke/?p=11680), [DATED]). |
| **Delivered sunflower seed, Kenyan outgrower** | 51,000 | 62,000 | 81,500 | KES/t at gate | [ESTIMATE] build-up in §8. Contract price + aggregation 2-4.5k + haulage 1.5-4k + shrink 1-3k + programme cost (extension, credit losses) 1.5-5k. |
| Delivered sunflower seed, Kenyan spot/aggregator | 40,000 | 55,000 | 72,000 | KES/t | [ESTIMATE] §8 |
| Delivered sunflower seed, Uganda | 38,000 | 47,000 | 61,500 | KES/t | [ESTIMATE] §8. About 450 km haul plus border costs. |
| Delivered sunflower seed, Tanzania | 37,500 | 50,000 | 69,500 | KES/t | [ESTIMATE] §8. About 650-750 km haul plus border costs, informal-trade risk and aflatoxin rejects. |
| Delivered soybean (Kenya/Uganda) | 60,000 | 75,000 | 100,000 | KES/t | [ESTIMATE] from farmgate prices plus logistics |
| Delivered canola (Rift Valley) | 60,000 | 66,000 | 72,000 | KES/t | [ESTIMATE]: KES 60/kg plus about 300 km haul |
| **Blended delivered seed cost (steady-state mix, §9)** | **45,000** | **57,000** | **72,000** | **KES/t** | [ESTIMATE] weighted by the year-4 mix. Equals USD 347 / 439 / 555. |
| Imported Black Sea sunflower seed, landed Kisumu | 100,000 | 112,000 | 125,000 | KES/t | [ESTIMATE]: €0.58-0.60/kg FOB Odesa, Sep 2026 ([commodity-board](https://commodity-board.com/sunflower-seeds-under-pressure-while-oil-finds-support-in-tight-black-sea-flows)), plus freight, 10% CET and inland haulage. **Not viable.** |
| Sunflower oil yield, expeller (seed basis) | 25 | 30 | 34 | % | Undehulled 19.7% on small Tanzanian expellers; dehulled 31-35% ([COSTECH/Lazaro](https://repository.costech.or.tz/items/e23c10cb-6682-4441-9c02-4446353268f9/full), [DATED]). Seed oil 35-42% with 7-8% residual in full-press cake ([vendor](https://www.oilexpeller.com/?p=1702)). |
| Sunflower cake yield | 64 | 67 | 72 | % of seed | [ESTIMATE]: 100 minus oil yield minus 2-3% process loss |
| Sunflower cake crude protein | 28 | 32 | 44 | % | 44% from dehulled seed ([COSTECH](https://repository.costech.or.tz/items/e23c10cb-6682-4441-9c02-4446353268f9/full)). The undehulled 28-32% is [ESTIMATE] from standard feed tables. |
| Soybean oil yield, expeller | 10 | 12 | 14 | % | [ESTIMATE]: seed 18-20% oil, expeller residual about 6-8% |
| Soy expeller cake crude protein | 40 | 43 | 45 | % | [ESTIMATE], standard tables |
| Canola oil yield, expeller | 30 | 33 | 36 | % | [ESTIMATE]: seed 40-44% oil |
| Canola cake crude protein | 32 | 35 | 37 | % | [ESTIMATE] |
| Road haulage, trunk (bulk/bagged) | 4.0 | 6.5 | 9.0 | KES/t-km | Derived: Mombasa–Nairobi 20 ft container KES 80-100k for about 480 km at about 25 t gives 6.7-8.3 ([Standard, 2022](https://www.standardmedia.co.ke/evewoman/young-women/article/2001440335/transport-association-asks-members-to-increase-transportation-charges-countrywide), [DATED]). Mombasa–Kampala about KES 116k for about 1,170 km gives about 4.0 ([Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/weekly-protests-hit-seamless-flow-of-cargo-from-mombasa-port-4700470), undated). Base adds 2026 fuel inflation. |
| Haulage, farm to aggregation (feeder roads) | 12 | 18 | 30 | KES/t-km | [ESTIMATE]: short hauls on poor roads cost 2-4x trunk rates |
| Storage cost (warehouse, bagged) | 60 | 120 | 530 | KES/t/month | NCPB KES 3 per 50 kg bag per month = KES 60/t (2020 directive, [Business Daily](https://www.businessdailyafrica.com/bd/news/boost-for-cereal-farmers-as-drying-costs-slashed-2452566), [DATED]). WRS KES 48 per 90 kg bag in month 1 = KES 533/t, then KES 100/t ([Logistics Business Africa](https://www.logisticsbusinessafrica.co.za/warehouse-receipt-system-in-kenya-open-doors-to-maize-farmers/), [DATED]). |
| Storage shrink/handling loss | 0.3 | 0.5 | 1.0 | %/month | [ESTIMATE]. Malawi farm-level loss is 5-12% of harvest when losses occur ([AgEcon](https://ageconsearch.umn.edu/record/313565/files/ajar12237.pdf)). |
| Share of annual seed bought Jun–Oct | 55 | 70 | 80 | % | [ESTIMATE] from the harvest calendars in §7 |
| Peak seed inventory (20 kt plant) | 7,000 | 10,000 | 12,000 | t | [ESTIMATE] §7 |
| Working-capital cost of seed carry | 1,500 | 2,300 | 3,500 | KES/t processed | [ESTIMATE]: average inventory × 14.4% lending rate ([macro notes](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_macro_investment_climate.md)) |
| Outgrower side-selling / non-delivery | 15 | 30 | 50 | % of contracted output | [ESTIMATE]. No quantified EAC oilseed rate found. Bidco reports crop switching ([Business Daily](https://www.businessdailyafrica.com/bd/markets/bidco-taps-farmers-to-cover-edible-oil-supply-shortfall-1970404), [DATED]). |
| Outgrower delivered yield | 0.6 | 0.9 | 1.3 | t/ha | Nakuru about 1.06 t/ha (9,500 t from 9,000 ha) ([KNA](https://www.kenyanews.go.ke/?p=179463), 2026). Kajiado 800-1,200 kg/acre, i.e. 2-3 t/ha, a county claim ([Nation](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502)). Treated as optimistic. |
| Fish-feed aflatoxin limit (KS 2289-1:2016) | – | ≤10 total; ≤5 B1 | – | ppb | [WTO TBT notification](https://members.wto.org/crnattachments/2016/TBT/KEN/16_4795_00_e.pdf) [DATED but current standard] |
| Aflatoxin rejection rate on Tanzanian/regional cake or seed | 5 | 15 | 40 | % of lots | [ESTIMATE]. 61.5% of Tanzanian sunflower-cake samples exceeded limits (secondary citation, [TJS/UDSM](https://tjs.udsm.ac.tz/index.php/tjs/article/download/2043/979/3470)). Cake up to 598 ng/g in Dodoma ([PLOS One/PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC5395219)). Seed bought dry and screened should be much lower. |
| EAC CET on extra-EAC oilseeds (soy, sunflower, cottonseed) | – | 10 | – | % | [Milling MEA](https://millingmea.com/kenyan-feed-millers-face-soybean-shortage-as-prices-surge-by-over-us0-12/) (2024). Intra-EAC originating goods are 0% under the EAC Customs Union [ESTIMATE: standard rule, not re-verified for 2026]. |
| Duty on crude palm oil (competing oil) | 0 | 10 | 25 | % | 10% since 1 Jul 2024 ([Milling MEA](https://millingmea.com/cooking-oil-prices-surge-following-new-import-duty/)). The 25% proposal was withdrawn with the Finance Bill 2024. Lobbying to scrap the 10% continues. |

---

## 1. Kenyan domestic oilseed production, 2023–2026

### 1.1 The headline numbers are poor and contradictory

- **Edible-oil demand.** Two figures circulate: about 600,000 t/yr, with imports covering 90–95% ([The Star, 14 Mar 2026](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)), and about 900,000 t/yr ([The Star, 27 Mar 2024](https://www.the-star.co.ke/news/infographics/2024-03-27-state-turns-to-local-production-to-cut-sh160bn-edible-oil-import-cost)). **[CONFLICT]** In 2023 Kenya imported 720,000 t of crude and refined vegetable oil worth KES 98.9bn (same Star 2024 source). In the quarter to June 2025 it imported 183,139 t worth KES 25.6bn, mostly palm oil ([Nation](https://nation.africa/kenya/business/value-of-edible-oil-imports-up-to-sh26bn-prices-jump-5292348)).
- **Domestic oil-crop output.** AFA, via The Star (2024), puts output at about 80,000 t of edible-oil crops. Another figure is 306,000 t, or "34% of 900,000 t" ([KNA](https://www.kenyanews.go.ke/?p=170375); [KIPPRA](https://kippra.or.ke/leveraging-on-the-sunflower-value-chain-for-job-creation-in-kenya/)). **[CONFLICT]** The 34% probably counts local refining or fats (for example animal fat and cottonseed) and is not oilseed crushing of Kenyan seed. For feedstock planning, **use the 80,000 t (seed, all crops) order of magnitude** and treat it as optimistic.

### 1.2 By crop

| Crop | Area / output (best available) | Yield | Farmgate price | Main counties | Assessment for the crusher |
|---|---|---|---|---|---|
| **Sunflower** | National: 3.6 kt (2023) vs 3.7 kt (2022), Economic Survey via [KIPPRA](https://kippra.or.ke/leveraging-on-the-sunflower-value-chain-for-job-creation-in-kenya/) (units unclear). 6,000 t (FAOSTAT via [Selina](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds)). Nakuru alone: >9,000 ha and about 9,500 t ([KNA](https://www.kenyanews.go.ke/?p=179463), 2026). AFA aimed to go from about 50,000 to 250,000 acres ([Star, Oct 2023](https://www.the-star.co.ke/news/2023-10-11-kenya-to-boost-sunflower-production-afa-boss), [DATED]). **[CONFLICT]** **[ESTIMATE]** National output is 10–30 kt/yr in 2025/26: about 20,000 ha × 0.6–1.2 t/ha. | 0.6–1.2 t/ha typical [ESTIMATE]. County claims of 800–1,200 kg/acre in Kajiado ([Nation](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502)), 700 kg/acre in Taita Taveta, "25 bags/acre" for hybrids ([KNA](https://www.kenyanews.go.ke/county-rolls-out-sunflower-project-to-boost-production-of-edible-oils/)) | KES 47 (FAOSTAT-based, Jun 2026). Bidco KES 33 [DATED]. Bungoma contract presser paid KES 100 ([How We Made It In Africa](https://www.howwemadeitinafrica.com/770-per-acre-why-kenyan-farmers-are-turning-to-sunflowers/152439/), [DATED]; a niche premium) | Nakuru, Narok, Kajiado (Loitokitok), Trans Nzoia, Uasin Gishu, Bungoma, Busia, Kakamega, Siaya, Kisumu, Migori, Meru, Laikipia, Taita Taveta ([Milling MEA, Kakamega](https://millingmea.com/kenyas-kakamega-county-farmers-encouraged-to-adopt-sunflower-cultivation-for-economic-growth/); [LBDA Kisumu](https://millingmea.com/lbda-expands-sunflower-farming-drive-to-boost-farmer-incomes-in-kisumu/)) | **Primary crop.** Drought-tolerant, bimodal in the west. Small national base: a 20 kt plant would need about 70–200% of current national output without an outgrower build-up. |
| **Soybean** | 2,000 t/yr vs demand >200,000 t (Farm Africa/Nation 2026, [Nation](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966)). 17,417 t in 2024, +72% (FAOSTAT via [Selina](https://www.selinawamucii.com/insights/prices/kenya/soya-beans/)). **[CONFLICT]** One processor alone wanted 3,000–3,500 t but got about 200 t (Promasidor, [Business Daily](https://www.businessdailyafrica.com/bd/data-hub/why-high-earning-soybeans-yet-take-root-kenya-3595298), [DATED]). Homa Bay is now the leading county (KNBS 2025, via Nation). | 0.56–1.1 t/ha on farms vs 3.0–3.6 potential ([UoN thesis](https://ir-library.ku.ac.ke/bitstreams/fb954d03-d40f-45cc-8cd2-d5cad4f854d9/download), [DATED]). 0.8 t/ha on about 2,500 ha ([TL bulletin 2013](https://tropicallegumeshub.com/wp-content/uploads/2020/06/BTL20-October-2013-Ken.pdf), [DATED]) | KES 70 (Homa Bay, Jul 2026, [Standard](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)). Seed KES 320/kg at KALRO Mkulima shops (Mar 2026, [Star](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)). KALRO released 7 new varieties in Mar 2025 ([Star](https://www.the-star.co.ke/counties/2025-03-17-researchers-launch-new-soybean-varieties)) | Homa Bay, Migori, Busia, Kakamega, Bungoma, Siaya, Kisii | **Secondary crop, a feed rather than an oil play.** About 12% expeller oil. Competes with direct feed use (full-fat soy). Non-GM status is valuable while the GMO order stands. |
| **Canola/rapeseed** | Agventure presses "just under 10,000 t/yr", about 50:50 member farms and outgrowers ([CPM, Mar 2026](https://www.cpm-magazine.co.uk/wp-content/uploads/sites/9/2026/03/066-68-Kenya-March-26.pdf)). Pure Mountain capacity is 5–7 kt; the group works with about 25,000 ha ([Capital FM](https://capitalfm.africa/canola-farming-pioneers-drive-sustainable-farming/)). Nakuru gave out 5 t of canola seed for 1,250 acres ([KNA](https://www.kenyanews.go.ke/nakuru-county-government-embarks-on-promoting-oil-crop-farming-to-cut-cooking-oil-imports/)) | About 1.5–2.5 t/ha on large farms [ESTIMATE] | KES 60 guaranteed with cake buy-back (Agventure, Mar 2026) | Narok, Nakuru, Uasin Gishu, Nyandarua, Laikipia, Meru (wheat-rotation highlands) | **Best margin per tonne, but supply is locked** inside the Agventure cooperative. Treat as an opportunistic 5–10% at most. Glucosinolates limit fish-feed inclusion of cake [ESTIMATE]. |
| **Cottonseed** | 3,863 t of seed cotton from 12,152 ha in 2023, about 30,000 households (AFA Yearbook 2025 via [AllAfrica, Jul 2026](https://allafrica.com/stories/202607290371.html); the host page is uncertain). That implies about 2,300–2,500 t of cottonseed [ESTIMATE: 60–65% of seed cotton]. 7 ginneries operating ([KNA](https://www.kenyanews.go.ke/government-to-revive-the-cotton-industry/)) | About 0.32 t/ha seed cotton (calculated) | Seed cotton KES 52, raised to KES 65–72 ([Star, Mar 2024](https://www.the-star.co.ke/counties/nyanza/2024-03-26-siaya-farmers-receive-sh25m-cotton-seeds-to-boost-yields); [KNA](https://www.kenyanews.go.ke/government-raises-price-of-cotton/)) | Busia, Siaya, Homa Bay, Kisumu, Migori, Baringo, Kwale, Lamu | **Negligible volume.** Gossypol limits inclusion. Opportunistic only. |
| **Groundnut** | No national 2024/25 figure found. Busia targeted 35 t in one season ([KNA](https://www.kenyanews.go.ke/county-promotes-groundnuts-to-alleviate-poverty/)). Homa Bay farmers are switching out of groundnut because aflatoxin deters manufacturers ([Nation 2026](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966)) | <1 t/ha [ESTIMATE] | Food market prices far above crush parity [ESTIMATE] | Homa Bay, Migori, Busia, Siaya, Kisii | **Exclude.** High aflatoxin risk (Kenyan samples up to 2,377 µg/kg, [Ndung'u 2013](https://www.m.elewa.org/JABS/2013/65/Abstract3-ndungu.html), [DATED]). The food market outbids crushers. |
| **Sesame** | 6,005 t in 2024 (+57%); 1,655 t exported, US$1.9m (FAOSTAT via [Selina](https://www.selinawamucii.com/insights/prices/kenya/sesame-seeds/)) | Low | About US$0.87/kg, about KES 113–121 | Coast, Lower Eastern, Lake | **Exclude.** An export and confectionery crop at about 2x crush parity. |
| **Castor** | Not researched in depth; no current data found | – | – | Semi-arid Eastern/Coast | **Exclude** from food/feed. The cake is toxic (ricin) and needs separate lines. |

**Judgement.** Kenya's own oilseed supply is about two orders of magnitude smaller than its edible-oil gap. The binding constraint is **seed, not crushing capacity**. The Star (Mar 2026) reports that many processing factories are "underutilised due to shortage of raw materials". One KNA-reported processor needs >10,000 t/yr of sunflower and soy but local farmers supply about 5,000 t ([KNA](https://www.kenyanews.go.ke/?p=138895)). Kenyan feed millers ran at 50–60% capacity in Jul 2026 ([The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)).

---

## 2. Regional supply

### 2.1 Tanzania (sunflower)

- **Scale.** The Ministry of Agriculture reported >480,000 t of seed in 2022/23 on >520,000 ha of oilseeds, mainly Singida, Rukwa, Iringa, Dodoma and Njombe ([Milling MEA](https://millingmea.com/tanzania-to-establish-us130m-sunflower-processing-plant-in-arusha/)). Singida alone has 234,149 ha, with Dodoma, Njombe and Rukwa next (>84,000 ha each) ([Sci Reports/PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC10873336)). The Nation cites 2025 Ministry data of "about 3 million t" ([Nation](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502)). **[CONFLICT]**: 3 Mt looks implausible against 205–250 kt of oil output. **Use about 0.5–1.0 Mt.**
- **Tanzania is itself oil-deficit and adding crush capacity.** It produces about 205,000 t of oil against demand of 570,000 t ([The Exchange](https://theexchange.africa/tanzania-seeks-investment-to-curb-cooking-oil-shortage/)). Older estimates are about 250 kt vs 600–700 kt **[CONFLICT, minor]**. A US$130m Arusha sunflower plant was signed in Dec 2024 ([Milling MEA](https://millingmea.com/tanzania-to-establish-us130m-sunflower-processing-plant-in-arusha/)). A Dodoma plant needs 30–35 kt of seed. Under Agenda 10/30, additional seed is "primarily directed to domestic processing" ([UkrAgroConsult](https://ukragroconsult.com/en/news/tanzania-plans-to-double-sunflower-production-and-develop-oil-exports/)).
- **Export rules.** **No current formal ban on raw sunflower seed exports was found.** The only legal text found is a 1965 revocation of 1954 export rules ([TanzLII](https://tanzlii.org/en/akn/tz/act/gn/1965/26/eng@2002-07-31)). However:
  - Formal raw-seed exports are tiny: US$244k in 2023, about 8% to Kenya ([TrendEconomy](https://trendeconomy.com/data/h2/Tanzania/1206)). Kenya's recorded 2024 sunflower-seed imports from Tanzania were about US$3k ([Trading Economics](https://tradingeconomics.com/kenya/imports/tanzania/oil-seed-oleagic-fruits-grain-seed-fruit)). **Seed trade is overwhelmingly informal.**
  - **Flow direction.** In mid-2026 the Nation reported Kajiado (Loitokitok) farmers trucking Kenyan seed **into** Tanzania because Tanzanian buyers pay more than local brokers. **Tanzania is currently a net seed sink at the Namanga/Loitokitok border, not a source.**
  - **[CONFLICT/ERROR]** The Nation quotes Tanzanian retail of "TZS 40–70/kg". At about KES 2–4/kg that is implausible; it is probably TZS 400–700 or KES 40–70. I treat it as unusable.
  - **Policy risk.** Tanzania has form on ad hoc export restrictions for food crops, and Kenya–Tanzania levy disputes (AFA cereal and legume fees, a Namanga blockade) recur ([Business Daily](https://www.businessdailyafrica.com/bd/economy/kenya-new-food-tax-risks-trade-spat-with-tanzania-4725780)). **[ESTIMATE]** P(material restriction on raw-seed exports in any given year) is about 20–30%.
- **Prices.** Farmgate is US$0.21/kg (TZS 497) as of Jun 2026, FAOSTAT-based ([Selina](https://www.selinawamucii.com/insights/prices/tanzania/sunflower-seeds/)). TZS 622/kg in Singida in 2021, a level the study found loss-making for farmers ([UDOM](https://repository.udom.ac.tz/items/8d88b37b-488e-4af0-baef-4b622430929f/full), [DATED]).
- **Cake rather than seed.** Kenya historically imports **sunflower cake** from Tanzania, at KES 25 then 30 and later 35/kg ([Nation](https://nation.africa/kenya/business/animal-feed-cost-jumps-on-weakening-shilling-3225038); [Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/30-animal-feeds-firms-close-shop-two-months-3560934), both [DATED]). Small Tanzanian expeller cake has very high aflatoxin: 2.7–536 ng/g in Morogoro and 1.4–598 ng/g in Dodoma ([PLOS One](https://pmc.ncbi.nlm.nih.gov/articles/PMC5395219)), and a reported 61.5% of feed-cake samples exceeded limits. **It is unfit for fish feed without lot-by-lot testing.**

**Judgement.** Tanzanian seed is a **swing source of 5–30%** and should not be in the base case at more than about 25%. It is cheapest at farmgate but competes with a domestic crush build-out and an import-substitution policy. Its quality (aflatoxin, moisture, foreign matter) is the worst of the options.

### 2.2 Uganda (soybean, sunflower)

- **Soybean.** About 250,000 t/yr, 70% in the north. About 40% is consumed locally and the balance traded informally, "mostly Kenya" ([Monitor](https://www.monitor.co.ug/uganda/oped/commentary/govt-vegetable-oilseeds-project-excites-north-but--4016020), [DATED]). FAOSTAT gives 150,000 t for 2023 ([Tridge](https://www.tridge.com/tridge-woods/soybean/UG)). **[CONFLICT]** Either way, Uganda is **Kenya's largest single soy source**. AKEFEMA links the 2024 price spike to a poor Ugandan harvest ([Milling MEA](https://millingmea.com/kenyan-feed-millers-face-soybean-shortage-as-prices-surge-by-over-us0-12/)).
- **Sunflower.** Total oilseed output is about 80,000 t vs consumption of about 480,000 t ([Monitor/NAADS](https://www.monitor.co.ug/uganda/news/national/lango-acholi-get-shs7-billion-for-oilseed-growing-4337080)). Domestic raw material is less than 20% of crusher needs ([IdeasHouse/NAADS](https://ideashouse.news/naads-distributes-76-tons-of-sunflower-seed-to-farmers-in-northern-uganda-to-boost-oil-crop-production/)). Mukwano works with more than 100,000 Lango farmers and runs 400 t/day of milling capacity ([UIA](https://ugandainvest.go.ug/?p=579); [Publicis EA](https://publicisteastafrica.com/tanzanian-sunflowers-bloom-into-new-opportunities-a-local-transformation/)). The government spent UGX 5bn on sunflower seed and UGX 2bn on soy seed in FY2023/24. UN Comtrade (via Tridge) shows 2024 sunflower-seed exports going mainly to Kenya and Tanzania; volumes were not found.
- **Prices.** The sunflower export unit value is US$0.17/kg (UGX 645), down 54% y/y as of Aug 2026 ([Selina](https://www.selinawamucii.com/insights/prices/uganda/sunflower-seeds/)). Farmgate is UGX 1,200/kg in Adjumani ([Monitor](https://www.monitor.co.ug/uganda/magazines/farming/adjumani-farmers-ask-govt-to-regulate-sunflower-price-4085558), [DATED]). Soy export unit values ran US$0.05–0.65/kg in 2024 (Tridge; noisy).
- **Logistics.** Lira to Kisumu is about 450 km via Malaba or Busia. About 1,000 trucks a day cross at Malaba, with delays ([Star, 2023](https://www.the-star.co.ke/business/kenya/2023-09-14-transporters-hit-as-malaba-border-delays-persist), [DATED]).

**Judgement.** Uganda is the **most natural regional source** for a western-Kenya plant: closest, EAC duty-free, bimodal and non-GM. It is contested by Mukwano (sunflower) and by Kenyan feed millers (soy). Plan on 25–35% from Uganda via 2–4 licensed aggregators in Lira/Soroti/Tororo, with quality specifications and pre-shipment testing.

### 2.3 Zambia and Malawi (soybean)

- **Zambia.** It has a history of banning soybean and sunflower-meal exports, with licensing frustrations ([Global Farmer Network](https://globalfarmernetwork.org/the-government-of-kenya-should-allow-imports-of-gm-soya-beans/), [DATED]). ZNFU has lobbied for "regulated exports" ([Zambia Monitor](https://www.zambiamonitor.com/?p=19015), [DATED]). In 2023 dominant buyers paid very low prices and farmers planted less than half the 2023 crop area in 2024 ([AllAfrica, Mar 2025](https://allafrica.com/stories/202503190003.html)). **New 2025–26 development:** China approved Zambian soybean origin in Apr 2025, and the first shipment was dated 10 Oct 2026 ([commodity-board](https://commodity-board.com/pierwszy-adunek-soi-z-zambii-do-chin-symboliczny-krok-i-duzy-potencja)). That adds a deep-pocketed competing buyer for Zambian non-GM soy. Wholesale prices of US$1.74–2.62/kg from Selina are implausible (probably retail or flour) and are not used. **[DATA QUALITY]**
- **Malawi.** It imposed and lifted three soy export bans between 2010 and 2012; a ban can cut farmer net revenue by 56% ([IFPRI MaSSP 2014](https://massp.ifpri.info/2014/05/09/soya-export-bans-and-applying-net-map-to-trade-policy-reform-in-malawi/), [DATED]). An undated *Nation (Malawi)* report mentions rationing of 5,000 t per exporter (exact URL and date unverified). Export prices were US$0.33–0.81/kg in 2024 (Tridge; noisy).
- AKEFEMA (2024): Zambia and Malawi, "traditional sources of soybean for Kenya, have stopped exporting".
- **Landed cost** [ESTIMATE]. COMESA origin is duty-free into Kenya (Zambia and Malawi are COMESA members). Lusaka to Kisumu by road is about 2,300 km, roughly KES 12–18/kg, or by rail and road via Dar. On a farmgate of US$0.40–0.50/kg (KES 52–65), that gives about **KES 70–90/kg delivered**. This is uncompetitive with Uganda except in shortage years.

**Judgement.** Zambia and Malawi are a **0–10% opportunistic soy source** with a high policy-interruption probability (about 30–50% per year that some restriction binds [ESTIMATE]). Do not underwrite them.

### 2.4 Extra-regional imports (price anchors)

| Item | Price | Date | Source | Landed Kisumu [ESTIMATE] |
|---|---|---|---|---|
| Sunflower seed, FOB Odesa | €0.576–0.595/kg | Sep 2026 | [commodity-board](https://commodity-board.com/sunflower-seeds-under-pressure-while-oil-finds-support-in-tight-black-sea-flows) | About KES 105–115/kg after freight, 10% CET and inland haulage. **About 2x local; not viable.** |
| Sunflower meal, FOB Black Sea | US$245–260/t | Aug 2026 | [cbonds](https://cbonds.fr/indexes/183665/) | About KES 48–52/kg: CIF about US$320, +10%, +KES 5 inland. **This caps the value of sunflower cake.** |
| Soybean meal (48%), CIF Rotterdam | US$403/t; 2026 YTD range 354–425 | 31 Aug 2026 | [cbonds/World Bank](https://cbonds.fr/indexes/154082/) | About KES 67–72/kg if legal. Argentine/Brazilian meal is GM and **blocked** while the Court of Appeal order stands (§5). |
| Crude palm oil (competing oil) | US$1,007.51/t (Indonesia reference, Sep 2026). Malaysia Oct reference US$1,091 | Sep–Oct 2026 | [IDN Financials](https://www.idnfinancials.com/news/68245/cpo-reference-price-rises-1-1-to-usd-1-007-51-per-tonne-in-september); [Bernama](https://www.bernama.com/en/news.php?id=2604287) | About KES 150–166/kg at Mombasa after freight and 10% duty. **This is the ceiling on local crude oil value.** |

---

## 3. Oil content, extraction yields, cake quality and seed quality

| Seed | Seed oil % | Expeller oil yield (seed basis) | Solvent yield | Cake residual oil (expeller) | Cake CP % | Notes |
|---|---|---|---|---|---|---|
| Sunflower (hybrid, black) | 38–44 [ESTIMATE] | 30–34% (twin-press, partly dehulled) | 38–42% | 7–8% full press; 15–20% pre-press ([vendor](https://www.oilexpeller.com/?p=1702)) | 28–32 undehulled; about 44 dehulled ([COSTECH](https://repository.costech.or.tz/items/e23c10cb-6682-4441-9c02-4446353268f9/full)) | Crude fibre about 17% even in dehulled cake, which limits tilapia inclusion to about 15–25% [ESTIMATE] |
| Sunflower (open-pollinated, striped) | 25–35 [ESTIMATE] | **19.7% undehulled** on small Tanzanian expellers; 31–35% dehulled ([COSTECH](https://repository.costech.or.tz/items/e23c10cb-6682-4441-9c02-4446353268f9/full), [DATED]) | – | high | 25–30 | Undehulled oil often failed TBS quality limits |
| Soybean | 18–20 | 10–14% | 17–19% | 6–8% | 40–45 expeller; 44–48 solvent | Must be heat-treated to destroy trypsin inhibitors. Extruder-expeller is the standard small-plant route [ESTIMATE] |
| Canola | 40–44 | 30–36% | 40–42% | 8–12% | 32–37 | Glucosinolates and fibre limit fish inclusion [ESTIMATE] |
| Cottonseed | 15–20 | 12–15% | 17–18% | 5–8% | 30–41 | Gossypol; needs delinting and dehulling [ESTIMATE] |
| Groundnut | 45–50 | 38–42% | – | 6–8% | 45–50 | Aflatoxin, exclude |

Undocumented ranges are standard processing-handbook values and are marked [ESTIMATE]. The reported 35–50% protein for sunflower cake ([PJSIR](https://pjsir.org/multidisciplinary-archive/Volume%2035%201992/Issue%207-8/Article%2017%20Vol%2035%20Issue%207-8%201992.pdf), [DATED]) applies to dehulled material.

**Implications for the model**
1. **Buy seed on oil content.** The difference between 25% and 32% expeller yield is about KES 12,000/t of seed in product value [ESTIMATE: 7 points × KES 175/kg crude oil, less extra cake credit]. A NIR seed analyser and an oil-content-based price grid are essential, and the outgrower programme must supply hybrids.
2. **Partial dehulling** raises both oil yield and cake protein, which makes the cake usable in fish feed. Capex and dehulling decisions belong to the plant-design workstream.
3. **Expeller only vs solvent.** At 20 kt/yr, solvent extraction rarely pays [ESTIMATE]. Accept 7–10% residual oil in cake. That oil is valuable energy in fish feed.

**Seed quality specifications** [ESTIMATE, industry norms]
- Moisture ≤9% for sunflower and ≤12% for soy at intake.
- Foreign matter ≤2–3%.
- Aflatoxin: screen every lot (lateral-flow kits). The fish-feed product must meet total aflatoxin ≤10 ppb and AFB1 ≤5 ppb (KS 2289-1:2016, via [WTO TBT](https://members.wto.org/crnattachments/2016/TBT/KEN/16_4795_00_e.pdf)). Kenya's legal limit for groundnuts is 15 ppb ([Hoffmann/EastAfrican](https://www.theeastafrican.co.ke/tea/opinion/columnists/hoffmann-what-kenya-must-do-to-get-toxins-out-of-food-supply-1432104)).
- Hull contamination is a key aflatoxin vector: in a Tanzanian feed study, "all sunflower seed hull samples were contaminated" ([TJS/UDSM](https://tjs.udsm.ac.tz/index.php/tjs/article/download/2043/979/3470)).
- KALRO and KEBS raised alarms about aflatoxin in Kenyan grains in 2025/26 ([Milling MEA](https://millingmea.com/?p=2040788)).
- A Kenyan study reports "significant non-compliance" in compound feed and feed ingredients ([AgEcon/Kibugu](https://ageconsearch.umn.edu/record/334006/files/Kibugu20995.pdf)).

---

## 4. Outgrower and contract-farming models

### 4.1 Evidence from oilseeds in the region

| Scheme | Model | Outcome / evidence |
|---|---|---|
| **Bidco (Nakuru, Meru)** | Contracts for sunflower and soy. Equity Bank input loans. Pledged KES 30–35/kg for sunflower in Meru ([Business Daily](https://www.businessdailyafrica.com/bd/news/counties/bidco-set-to-buy-sh120m-sunflower-seeds-from-farmers-in-meru-2301152), [DATED]) | Bidco's own account: farmers "shifted to producing other crops that promise higher market prices" (maize, wheat, beans), "frustrating the partnership" ([Business Daily](https://www.businessdailyafrica.com/bd/markets/bidco-taps-farmers-to-cover-edible-oil-supply-shortfall-1970404), [DATED]). **Failure mode: an uncompetitive fixed price against alternative crops.** |
| **Agventure / Pure Mountain (canola)** | A cooperative of commercial farmers (Laikipia, Nakuru, Meru, Narok, Uasin Gishu, Nyandarua). Guaranteed price about KES 60/kg. Cake buy-back for the farmers' own livestock. About 50% of throughput from members ([CPM, Mar 2026](https://www.cpm-magazine.co.uk/wp-content/uploads/sites/9/2026/03/066-68-Kenya-March-26.pdf)). AgDevCo USD 9.5m ([prior notes](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_agribusiness_manufacturing.md)) | **Works.** Aligned incentives (farmer-owners), a rotation crop for wheat farmers, mechanised larger farms, and a cake buy-back that adds a second hook. Scale is about 10 kt/yr after more than 10 years. |
| **Mukwano (Uganda, Lango)** | Seed distribution to more than 100,000 farmers, with buy-back ([UIA](https://ugandainvest.go.ug/?p=579)) | Sustained scale, but Ugandan domestic supply is still less than 20% of crusher needs. Uganda contract research reports contractual problems on both sides and farmers dropping out ([UC eScholarship](https://escholarship.org/uc/item/97g2r7mk)). |
| **Farm Africa soy aggregation (Homa Bay)** | Village aggregation centres, quality check and weigh-and-pay, interest-free loans and resilient seed for about 6,000 farmers ([Standard, Jul 2026](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)) | Volumes are still tiny. Middlemen buy at harvest for "<KES 80 per 4 kg tin", about KES 20/kg, and resell at more than KES 150 (about KES 37/kg) in the dry season ([Nation 2026](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966)). **[CONFLICT]** with the KES 70/kg quoted in the Standard. The crop for the tin price is ambiguous. |
| **Bungoma micro-presser** | Bought 20 t from 20 neighbours at KES 100/kg and sells cake at KES 70/kg ([How We Made It In Africa](https://www.howwemadeitinafrica.com/770-per-acre-why-kenyan-farmers-are-turning-to-sunflowers/152439/), [DATED]) | Shows that farmers respond to price. Cake at KES 70 is a retail niche price, not a bulk benchmark. |
| **Tanzania (SNV and others)** | Trust-based contracts in which the buyer supplies services ([ACE Europe/IOB 2013](https://www.iob-evaluatie.nl/binaries/iob-evaluatie/documenten/deelstudies/2013/11/01/mid-term-evaluatie-van-snv-programmas-in-benin-ethiopie-tanzania-en-vietnam/Ace-Europe_In-depth_study_of_support_to_edible_oil_value_chains_in_Tanzania_201311.pdf), [DATED]) | Embedded services reduce side-selling. |
| One Acre Fund (soy) | Trials in Kenya and Rwanda. Soy yield potential about 5 t/ha, but "below potential and not competitive with common bean" at farmer level ([OAF](https://oneacrefund.org/sites/default/files/2023-09/Soybean_and_Rhizobium_Ag_Innovations.pdf), [DATED]) | A caution against soy-heavy outgrower plans in Kenya. |

General literature: resource-providing contracts (inputs on credit) raise input use and yields ([Ruml & Qaim, Ghana oil palm](https://doaj.org/article/e525c025321847de8365c8406d24d2e1)). Results are "mixed" and contracts are often "merely a signal of intentions" ([Univ. of Cologne](https://geosciences.uni-koeln.de/index.php?id=17283)). Prior notes found that "benefits fade when support stops" ([prior notes](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_agribusiness_manufacturing.md)). **No quantified side-selling rate for EAC oilseeds was found.** I use 15/30/50% (low/base/high) [ESTIMATE], based on the general contract-farming literature and the Bidco account.

### 4.2 Design principles that the evidence supports [judgement]
1. **A floating, transparent price** (for example a floor plus a share of the oil/cake import-parity price, announced before planting) rather than a fixed price that loses to the spot market. This was Bidco's failure.
2. **Cake buy-back, or a discount on fish/poultry/dairy feed**, for growers (the Agventure hook). An integrated feed mill makes this natural.
3. **Aggregation through lead farmers and cooperatives** with weigh-and-pay on the spot (mobile money), as Farm Africa does. Avoid long payment lags.
4. **Recover input credit at the point of delivery, but keep credit modest.** Hybrid seed only (the highest-ROI input), not full packages, to limit the default exposure that drives side-selling.
5. **Geographic diversification** across bimodal western Kenya and the unimodal Rift and Kajiado zones to reduce weather risk, as Kamida does ([VC4A](https://vc4a.com/ventures/kamida-enterprises-limited/?lang=en)).
6. **Ride the public programmes.** Use county and AFA seed distribution and LBDA drives as the free "seed" component and add the offtake and price commitment. Do not duplicate the subsidy.

---

## 5. Government policy

- **Edible Oil Crops Promotion Project (AFA).** Runs 1 Jul 2023 to 30 Jun 2028 in 24 counties. Targets 200,000 acres (about 81,000 ha) and lifting local supply to 50% by 2028 ([Milling MEA](https://millingmea.com/kenya-accelerates-edible-oil-crops-farming-to-cut-imports-led-by-afa/)). The budget is KES 981m, and MPs have questioned its effectiveness and the decision to import 500 t of sunflower seed from Zambia rather than buy from Trans Nzoia ([Eastleigh Voice](https://eastleighvoice.co.ke/oil%20crop%20farming/99064/mps-raise-concerns-over-effectiveness-of-sh981-million-edible-oil-crop-promotion-project)). Kenya Seed distributed 70 t of seed for multiplication in Uasin Gishu and Trans Nzoia, with a further 30 t at ADC ([Star, Mar 2024](https://www.the-star.co.ke/news/infographics/2024-03-27-state-turns-to-local-production-to-cut-sh160bn-edible-oil-import-cost)).
  - **[ESTIMATE]** Even if fully achieved, 81,000 ha × 1 t/ha gives about 81 kt of seed, or about 25–30 kt of oil. That is about 5% of demand, not 50%. The target is aspirational.
- **March 2026 relaunch.** CS Kagwe launched an initiative at the Thika Kilimo Biashara Expo to fast-track sunflower and soy through high-yield varieties, seed multiplication and support for farmer groups and processing ([Capital FM](https://capitalfm.africa/govt-eyes-local-edible-oil-supply-through-sunflower-soybean-farming/); [Star](https://www.the-star.co.ke/counties/central/2026-03-14-kenya-launches-sunflower-drive-to-cut-sh145bn-edible-oil-import)). The goal is to halve edible-oil imports over 2026–2030 ([Milling MEA](https://millingmea.com/?p=2039516)).
  - The Star quotes seed at about KES 310/kg and a seeding rate of 20–30 kg/acre. **[CONFLICT/AMBIGUITY]** That rate fits soybean; hybrid sunflower is usually sown at about 2–3 kg/acre [ESTIMATE].
- **County programmes.** Nakuru gave out 45 t of sunflower seed to about 11,900 farmers, expecting about 20,000 acres ([KNA](https://www.kenyanews.go.ke/?p=138895)), and is seeding 3,900 more farmers ([Nakuru County](https://nakuru.go.ke/over-3900-farmers-in-nakuru-set-to-receive-sunflower-seeds/)). LBDA has a sunflower drive in Kisumu ([Milling MEA](https://millingmea.com/lbda-expands-sunflower-farming-drive-to-boost-farmer-incomes-in-kisumu/)). Kakamega promotes sunflower. Busia and Siaya are reviving cotton (17 t of seed in Busia, Aug 2026, [KNA](https://www.kenyanews.go.ke/busia-farmers-receive-17-tons-of-cotton-seed/)).
- **Trade policy on oil.** The 10% duty on crude palm oil has applied since 1 Jul 2024 under EAC Gazette No. 18. Processors are lobbying to scrap it ([People Daily](https://peopledaily.digital/news/agency-calls-for-removal-of-10pc-tax-on-crude-palm-oil)). The proposed 25% duty on raw and refined oils was dropped with the Finance Bill 2024. One MPOB item claims a 25% one-year duty on refined oils; it is unverified **[CONFLICT]**.
- **GMOs (status, Oct 2026).**
  - Cabinet lifted the GMO ban on 3 Oct 2022. The ELC dismissed the LSK petition on 12 Oct 2023, and the High Court dismissed further petitions on 7 Nov 2024.
  - **On 7 Mar 2025 the Court of Appeal (Kiage, Korir, Ngugi JJA) issued conservatory orders halting importation and open cultivation of GMOs pending the Kenya Peasants League appeal** ([Capital FM](https://capitalfm.africa/coa-halts-gmo-importation-pending-appeal/); [Citizen Digital](https://citizen.digital/article/blow-to-govt-as-court-of-appeal-bars-importation-of-gmos-n358801); [DLA Piper 2025](https://www.dlapiperafrica.com/en/kenya/insights/2025/gmo-adoption-in-kenya-navigating-legal-challenges-and-embracing-change)).
  - **No merits judgment was found as of Oct 2026.** In Jul 2026 feed millers described GMO imports as still suspended ([The Star](https://www.the-star.co.ke/news/2026-07-17-feed-industry-calls-for-reforms-to-make-animal-food-affordable)).
  - **Implication.** Kenyan feed millers cannot legally import GM soybean meal (Americas). That props up demand and prices for non-GM regional soy and oilseed cake, which favours a local crusher. **Two-sided risk:** a ruling for the government would let US$400/t GM soymeal in at about KES 67–72/kg landed, capping cake values. Model a scenario with about a 30% fall in the cake price premium [ESTIMATE].
- **Feed-raw-material duty waivers are ad hoc.** For example, 500,000+ t were waived duty-free in an earlier year ([Food Business Africa](https://www.foodbusinessmea.com/?p=1850132), [DATED]), and the government planned to gazette 360,000 t of duty-free yellow maize in Sep 2026 ([prior notes](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_agribusiness_manufacturing.md)). Waivers on soybean meal would directly compete with the plant's cake.

---

## 6. Storage, aggregation, logistics and post-harvest losses

- **Trunk haulage.** KES 4–9 per t-km, base 6.5 (derived in the table in §0). Shippers Council: US$5–8 per TEU-km in Kenya vs US$1–2 in Asia ([FreshPlaza](https://www.freshplaza.com/north-america/article/9714714/high-logistics-costs-hinder-africa-s-perishable-exports/), undated). Kenya Railways averaged KES 2,439/t per haul in Q1 2021 ([Business Daily](https://www.businessdailyafrica.com/bd/news/counties/sgr-cargo-revenue-decline-after-cut-in-freight-charges-3826184), [DATED]), and a 2026 tariff book exists ([KRC](https://krc.co.ke/wp-content/uploads/2026/06/Kenya-Railways-Tariff-Book.pdf); rates not extracted). The Kisumu MGR line is a possible option for Tanzanian or Ugandan lake and rail routes [ESTIMATE].
- **County cess and duplicative levies** on produce in transit remain "excessive" ([CAK/World Bank via AllAfrica, Nov 2025](https://allafrica.com/stories/202511270035.html)). Budget KES 300–1,000/t [ESTIMATE].
- **Indicative distances to Kisumu** [ESTIMATE, road km]: Busia/Bungoma 100–150; Homa Bay/Migori 100–180; Nakuru 190; Narok/Kajiado 300–450; Lira 450; Singida via Mwanza and Sirari 750–850; Lusaka about 2,300.
- **Storage.** NCPB rates were cut to KES 3 per 50 kg bag per month (KES 60/t/month) in 2020. WRS-certified storage costs KES 48 per 90 kg bag in month 1, then KES 9 per bag ([Business Daily](https://www.businessdailyafrica.com/bd/news/boost-for-cereal-farmers-as-drying-costs-slashed-2452566); [Logistics Business Africa](https://www.logisticsbusinessafrica.co.za/warehouse-receipt-system-in-kenya-open-doors-to-maize-farmers/), [DATED]). NCPB must lease 25% of its capacity to the private sector under the WRS. It earned KES 359.7m from leasing in 2024 ([Milling MEA](https://millingmea.com/?p=2032467)). **[ESTIMATE]** Own silos or warehouses at the plant cost KES 8,000–15,000 per t of capacity (capex workstream). Leased NCPB depots in Kisumu, Bungoma and Busia can act as aggregation hubs.
- **Post-harvest losses.** No Kenya-specific oilseed figures were found (APHLIS covers cereals). Malawi farm-level losses for soy and groundnut average 5–12% of harvest when they occur ([AgEcon](https://ageconsearch.umn.edu/record/313565/files/ajar12237.pdf)). French harvest-stage losses average about 2% for sunflower and 6% for soybean ([OCL](https://www.ocl-journal.org/articles/ocl/full_html/2015/03/ocl150012-s/T3.html)). KIPPRA blames post-harvest losses in part for the 2023 dip in sunflower volume. **[ESTIMATE]** Assume 5–10% farm-level loss, which affects farmer economics, plus 1–3% intake shrink and 0.5%/month storage loss at the plant.
- **Bird damage** is a major agronomic loss for sunflower in Kenya. It favours block planting and synchronised hybrids [ESTIMATE, agronomic knowledge; not sourced here].

---

## 7. Seasonality and working capital

### 7.1 Harvest calendar [ESTIMATE unless cited; agronomic norms, not confirmed by search]

| Source | Plant | Harvest / main buying window | Share of annual crop |
|---|---|---|---|
| Kenya West/Nyanza (bimodal) sunflower and soy | Mar–Apr (long rains); Sep–Oct (short rains) | **Jul–Sep**; Jan–Feb | about 60/40 |
| Kenya Rift and Kajiado sunflower; canola | Mar–May | **Aug–Oct** (canola Aug–Sep) | mostly single |
| Uganda (Lango, East) sunflower and soy | Mar–Apr; Aug–Sep | **Jul–Aug**; Dec–Jan | about 55/45 |
| Tanzania central (Singida, Dodoma; unimodal) | Dec–Feb | **May–Aug** | single (planting window, [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC10873336)) |
| Zambia/Malawi soy | Nov–Dec | Apr–Jun | single |

About **70% of the year's seed is bought June–October**, with a smaller window in Dec–Feb. Prices bottom at harvest and rise 50–90% into the lean season. The Homa Bay middleman spread is about KES 20 to KES 37/kg ([Nation 2026](https://nation.africa/kenya/business/seeds-of-gold/homa-bay-farmers-ditch-groundnuts-for-soya-beans-as-demand-rises-5549966)). This rewards a plant that can **carry stock** but punishes one that buys hand-to-mouth.

### 7.2 Working capital for the 20 kt/yr plant [ESTIMATE]

- **Peak seed inventory.** About 10,000 t (low 7,000, high 12,000) at end-October. At KES 57,000/t that is about **KES 570m (USD 4.4m)**, range KES 400–860m.
- **Average seed inventory.** About 5,000–6,000 t, roughly KES 285–340m. At 14.4% the carry costs about KES 41–49m/yr, or **about KES 2,300/t of seed processed** (range 1,500–3,500).
- **Storage.** About KES 120/t/month for 4 months on average, about KES 500/t. Shrink of about 0.5%/month over 4 months is about 2%, or about KES 1,100/t.
- **Outgrower input pre-finance.** Base year 4 has 8,000 t from outgrowers. At 0.9 t/ha delivered and 30% side-selling, that needs about 12,700 ha (31,000 acres) under contract. At a seed-only input of about KES 1,500–3,000/acre this is KES 45–95m outstanding Mar–Aug. A full package (seed, fertiliser, extension) at about KES 6,000–10,000/acre would be KES 190–310m. Expect 5–15% loss on credit.
- **Total seasonal working-capital peak** (seed stock + input credit + receivables − payables): about **KES 650–950m (USD 5–7m)** at steady state. Financing options [ESTIMATE]: WRS-backed inventory finance, DFI working-capital lines (AgDevCo, Norfund, IFC), and pre-sale of cake to the feed-mill side.
- **The feed mill helps smooth this.** It can draw down cake inventory evenly through the year and switch to imported sunflower meal (about KES 50/kg landed) when seed runs short.

---

## 8. Delivered cost build-up (KES per tonne of seed at a Kisumu/Busia plant gate) [ESTIMATE]

| Component | KE outgrower (L/B/H) | KE spot via aggregators | Uganda (Lira/Soroti) | Tanzania (Singida via Sirari) | Soy (KE/UG) | Canola (Rift) |
|---|---|---|---|---|---|---|
| Farmgate | 45,000 / 52,000 / 65,000 | 33,000 / 47,000 / 60,000 | 22,000 / 32,000 / 41,000 | 27,000 / 35,000 / 47,000 | 45,000 / 62,000 / 85,000 | 55,000 / 60,000 / 65,000 |
| Aggregation, bagging, trader margin | 2,000 / 3,000 / 4,500 | 3,000 / 4,000 / 5,500 | 4,000 / 5,000 / 7,000 | 4,000 / 5,000 / 7,000 | 3,000 / 4,500 / 6,000 | 1,000 / 1,500 / 2,000 |
| Haulage (feeder + trunk) | 1,500 / 2,500 / 4,000 | 2,000 / 2,500 / 4,000 | 2,500 / 3,500 / 5,000 | 4,000 / 5,500 / 8,000 | 2,000 / 3,000 / 5,000 | 2,000 / 3,000 / 4,000 |
| Border, phyto, AFA/KEBS, agent, cess | 300 / 500 / 1,000 | 300 / 500 / 1,000 | 800 / 1,500 / 2,500 | 1,000 / 2,000 / 3,500 | 500 / 1,500 / 2,500 | 300 / 500 / 1,000 |
| Quality shrink and rejects (moisture, FM, aflatoxin) | 700 / 1,300 / 2,000 | 1,200 / 1,500 / 1,500 | 1,000 / 1,500 / 2,500 | 1,500 / 2,500 / 4,000 | 1,000 / 1,500 / 2,500 | 500 / 800 / 1,000 |
| Programme cost (extension, credit loss, field staff) | 1,500 / 3,000 / 5,000 | – | – | – | 0 / 2,000 / 4,000 | – |
| **Delivered** | **51,000 / 62,300 / 81,500** | **39,500 / 55,500 / 72,000** | **30,300 / 43,500 / 58,000** | **37,500 / 50,000 / 69,500** | **51,500 / 74,500 / 105,000** | **58,800 / 65,800 / 73,000** |

Rounded model inputs for Uganda: 38,000 / 47,000 / 61,500 KES/t. I lifted the low and base above the build-up because a Ugandan farmgate of KES 22 is an export unit value, not a price that wins volume against Mukwano.

**Programme cost logic.** One field officer per 500 farmers at about KES 60k/month costs about KES 720k/yr. Those farmers deliver about 400 t, so the officer costs about KES 1,800/t. Credit losses of about 10% on a KES 6,000/acre package at 0.4 t/acre add about KES 1,500/t.

**Sanity check: maximum affordable seed price** [ESTIMATE; the oil-price and crush-margin workstreams should replace these inputs]

| | Sunflower | Soybean | Canola |
|---|---|---|---|
| Oil yield and value | 30% at KES 175/kg = 52,500 | 12% at KES 175/kg = 21,000 | 33% at KES 185/kg = 61,050 |
| Cake yield and value | 67% at KES 35/kg = 23,450 | 84% at KES 65/kg = 54,600 | 64% at KES 40/kg = 25,600 |
| Product value per t of seed | 75,950 | 75,600 | 86,650 |
| Crushing cost | about 6,500 | about 7,000 (extrusion) | about 6,500 |
| **Break-even seed price** | **about KES 69,000/t** | **about KES 68,600/t** | **about KES 80,000/t** |

Assumptions behind these values:
- Crude oil at KES 175/kg assumes a sunflower or soy premium of about 5–15% over landed CPO at KES 150–166/kg.
- Cake values sit at a discount to landed Black Sea sunflower meal (KES 48–52/kg) and to non-GM soy meal.

Against the base blended delivered cost of about KES 57,000/t, **sunflower leaves a gross crush margin of about KES 12,000/t (16%)**.
- At a 25% oil yield, or a 20% fall in the CPO price, the margin falls to about KES 2–5k/t.
- **Soy is marginal to negative at KES 70+/kg** unless its cake earns a non-GM premium. It is better routed whole into the feed mill as extruded full-fat soy.
- **Canola is the most attractive per tonne but the least available.**

---

## 9. Feedstock strategy: sourcing mix by year (reference 20 kt/yr plant)

**Sizing judgement.** Domestic sunflower output is about 10–30 kt/yr and incumbents (Bidco, Kapa, Kamida, small pressers) are already short of seed. **A crusher above about 20 kt/yr of seed is not supportable before year 5.** The exception is building a contracted base of more than 20,000 ha, roughly 25% of the national EOCPP target. Recommended approach:
- Start at **8–10 kt** in year 1 (one 30–40 t/day line).
- Add a second line when contracted area exceeds about 10,000 ha.
- Size the **feed mill** independently of the crusher: about 20–40 kt/yr of feed. It can buy external protein (imported sunflower meal, regional soy, fishmeal or BSF) whenever the crusher's cake is insufficient.

| Source (% of seed; tonnes) | Y1 (8 kt) | Y2 (13 kt) | Y3 (17 kt) | Y4 (20 kt) | Y5 (20 kt) | Delivered base, KES/t |
|---|---|---|---|---|---|---|
| Kenyan contracted outgrowers (sunflower, mainly West/Nyanza + Rift) | 10% / 800 | 20% / 2,600 | 30% / 5,100 | 40% / 8,000 | 45% / 9,000 | 62,300 |
| Kenyan spot via aggregators/cooperatives | 20% / 1,600 | 20% / 2,600 | 15% / 2,550 | 15% / 3,000 | 15% / 3,000 | 55,500 |
| Uganda sunflower + soy (licensed aggregators) | 35% / 2,800 | 30% / 3,900 | 30% / 5,100 | 25% / 5,000 | 25% / 5,000 | 47,000 |
| Tanzania sunflower (swing) | 30% / 2,400 | 25% / 3,250 | 15% / 2,550 | 10% / 2,000 | 5% / 1,000 | 50,000 |
| Canola / soy specialty (Rift canola, Homa Bay soy) | 5% / 400 | 5% / 650 | 10% / 1,700 | 10% / 2,000 | 10% / 2,000 | about 70,000 |
| **Blended delivered cost (base)** | **about 52,300** | **about 53,700** | **about 55,600** | **about 57,000** | **about 57,600** | |
| Contracted area needed (at 0.9 t/ha, 30% leakage) | about 1,300 ha | about 4,100 ha | about 8,100 ha | about 12,700 ha | about 14,300 ha | |
| Implied contracted smallholders (0.5–1 ha each) | 1.3–2.6k | 4–8k | 8–16k | 13–25k | 14–29k | |

**Blended delivered cost by year** [ESTIMATE]: low about KES 45,000/t, base about KES 57,000/t, high about KES 72,000/t (USD 347 / 439 / 555).

Two drivers move the blend:
- As the mix shifts toward costlier but more secure outgrower seed, the base cost rises about 10% from Y1 to Y5.
- That rise should be offset by better oil yield from hybrids (+2–4 points), which is worth about KES 3,500–7,000/t.

---

## 10. Binding supply risks (ranked)

1. **Absolute volume.** Kenyan oilseed output is too small, and incumbents are already short. P(year-1 throughput less than 60% of plan) is about 40% [ESTIMATE]. *Mitigants:* modular lines, start small, a feed mill that can run on bought-in protein.
2. **Competition for seed from Tanzanian crushers and Tanzanian policy.** Kenyan seed currently flows south at Loitokitok. Tanzania is building crush capacity (the US$130m Arusha plant) and steering seed to domestic processing. *Mitigant:* do not underwrite more than 25% from Tanzania; site near Uganda.
3. **Outgrower leakage and crop switching** (the Bidco precedent). *Mitigants:* floating price linked to import parity, cake/feed buy-back, weigh-and-pay, seed-only credit.
4. **Weather.** Fully rain-fed; the 2026 drought hit dairy and maize ([prior notes](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_agribusiness_manufacturing.md)). *Mitigant:* source from bimodal and unimodal zones in three countries.
5. **Aflatoxin and quality** against the 10 ppb fish-feed standard. This is especially acute for Tanzanian cake and seed and any groundnut. *Mitigants:* lot testing, moisture control, dehulling, binders; reject non-compliant lots into dairy or poultry feed lines with higher tolerance [ESTIMATE].
6. **Regional export restrictions** (Zambia and Malawi history; Zambia's new China outlet; Uganda unlikely). Keep these out of the base case.
7. **GMO ruling (two-sided).** A Court of Appeal ruling for the government would open GM soymeal imports at about KES 67–72/kg and cap cake values. Continued suspension sustains the non-GM premium.
8. **Oil price and duty policy.** Scrapping the 10% CPO duty or a 20% fall in palm prices would cut the sunflower break-even seed price by about KES 7–10k/t, wiping out most of the margin at base seed cost. That is a supply risk because the plant could no longer outbid rivals.
9. **Working capital.** A KES 650–950m seasonal peak at 14.4% interest. A stock-out forces lean-season buying at +50–90%.

---

## 11. Gaps and uncertainties

- **No authoritative 2024–2026 crop statistics.** KNBS Economic Survey tables, AFA Nuts and Oil Crops Directorate data and FAOSTAT conflict by up to 10x (soy: 2 kt vs 17 kt; sunflower: 3.6 kt vs 6 kt vs about 9.5 kt for Nakuru alone). **Action:** buy or request the AFA NOCD data and county agriculture reports; run a field survey before financial close.
- **Prices.** There is no 2026 bulk price series for Kenyan sunflower cake, soybean meal or crude sunflower oil. FAOSTAT-derived aggregator prices (Selina Wamucii, Tridge) are noisy, some are clearly wrong (Zambia US$1.74–2.62/kg), and their KES/USD conversions differ from 129.8. **Action:** obtain quotes from AKEFEMA members, Bidco/Kapa procurement and Kisumu feed millers.
- **Tanzania export rules.** No 2025–26 export ban was found, but there was no access to TRA or Ministry notices. The "TZS 40–70/kg" quote is clearly erroneous. The 3 Mt production claim is implausible.
- **Uganda volumes.** Informal trade dominates, so official Kenya import statistics understate flows. No 2025 Uganda sunflower production figure was found.
- **Side-selling rates.** No quantified EAC oilseed evidence was found. The 15/30/50% range is a literature-informed estimate.
- **Trucking rates.** There is no 2025–26 per-t-km survey. Rates are derived from 2022 container prices and an undated Mombasa–Kampala rate.
- **Harvest calendars** are agronomic norms, not confirmed by 2026 sources.
- **GMO case.** The status of the Court of Appeal merits hearing (expected late 2025) is unknown. Verify on Kenya Law before close.
- **Oil and cake yields.** These come from literature and vendor sources. Kenyan hybrid oil content was not measured. **Action:** lab-test 20–30 seed lots from target counties (NIR or Soxhlet).
- **Castor, and the extra-EAC CET status on oilcakes in 2026**, were not verified.
- **Search-result extraction.** Most pages could not be fetched, so some figures rest on search-engine summaries of paywalled or unreachable pages (notably the Nation Kajiado and Homa Bay pieces, CPM and KNA). Their exact wording and dates should be confirmed.
