# Technical and operations research: oilseed crushing, oil refining and extruded aquafeed (Kenya)

*Prepared 19 Oct 2026 for the Oilseed crushing + feed mill business plan. Author role: process engineer. FX: KES 130/USD (CBK ~129.8). Where I give no source, the figure is labelled **[ESTIMATE]** with my reasoning. **[DATED]** means the source is from before 2025. **[CONFLICT]** marks disagreement between sources. Almost all equipment prices found online are marketplace listings (Alibaba, IndiaMART, made-in-china) and not quotes. Treat them as order-of-magnitude only. Prices and market sizes are consistent with the companion file `research/market_demand.md`. Where this file uses its prices (crude oil, cake, SBM, feed), I say so.*

---

## 0. Key assumptions for the model

| # | Parameter | Low | Base | High | Unit | Source / basis |
|---|---|---|---|---|---|---|
| **Crushing** | | | | | | |
| 1 | Sunflower seed oil content (as received, ~8% moisture) | 36 | 40 | 44 | % | Oil-type sunflower 38–50% ([SA Grain/ARC, 2020](https://sagrainmag.co.za/2020/09/07/quality-hybrids-yield-high-oil-content/) [DATED]); hybrids 35–45% (Pakistani trial, search snippet). Smallholder seed in Kenya is mixed and often open-pollinated, so the base is set low [ESTIMATE] |
| 2 | Residual oil in full-press expeller cake | 12 | 10 | 7 | % of cake | 8–12% typical for commercial expellers ([US patent 10550352](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10550352) / [10647077](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10647077)); 6–7% vendor claim for sunflower ([oilexpeller.com](https://www.oilexpeller.com/?p=1702)) |
| 3 | Crude oil yield, full press (filtered) | 27 | 31 | 34 | % of seed | Mass balance in §5 [ESTIMATE]. Dehulled seed gave 31–35% vs ~19.7% undehulled in small Tanzanian presses ([COSTECH, 2015](https://repository.costech.or.tz/items/ebaa08d7-561a-4733-b9f8-91b212a43a4f) [DATED]) |
| 4 | Cake yield, full press, no dehulling | 66 | 64 | 61 | % of seed | Mass balance [ESTIMATE] |
| 5 | Cake crude protein, non-dehulled / dehulled | 26 / 33 | 30 / 36 | 33 / 40 | % as fed | Feedipedia: non-dehulled meal 29–33% DM, dehulled 35–39% DM ([Feedipedia](https://www.feedipedia.org/Node/732); [node 12806](https://feedipedia.org/node/12806)). Expeller cake is diluted by its 8–12% residual oil [ESTIMATE] |
| 6 | Oil yield, prepress + solvent (residual in meal 0.5–1.5%) | 36 | 38 | 40 | % of seed | Mass balance [ESTIMATE]; prepress cake leaves press at ~15–20% oil before extraction (patent and study snippets above) |
| 7 | Minimum efficient scale, solvent extraction | 75 | 150 | 200 | t seed/day | >200 tpd ([Univ. Missouri EM0602](https://extension.missouri.edu/media/wysiwyg/Extensiondata/Pub/pdf/energymgmt/em0602.pdf) [DATED]); >75 tpd and mechanical <100 tpd ([AMPC Montana](https://www.ampc.montana.edu/documents/briefings/briefing86.pdf) [DATED]); a 200 tpd solvent plant in Ethiopia ([MIGA ESIA, 2021](https://www.miga.org/sites/default/files/2021-05/ESIA-07-05-2021-V2%20Final.pdf) [DATED]) |
| 8 | Operating days per year (crushing) | 270 | 300 | 330 | d | [ESTIMATE]: 24 h/day, with downtime for seed shortage and maintenance |
| 9 | Crushing utilisation Y1 / Y2 / Y3+ | 35/55/70 | 50/70/85 | 65/85/90 | % | [ESTIMATE]: seed supply is the binding constraint (see §5, §6) |
| 10 | Electricity, full-press crushing (cleaning to filtering) | 40 | 60 | 120 | kWh/t seed | Small expellers 112–124 Wh/kg ([PJSIR 1993](https://pjsir.org/multidisciplinary-archive/Volume%2036%201993/Issue%205/Article%2012%20Vol%2036%20Issue%205%201993%20pp%20210-212.pdf) [DATED]); industrial prepress 28.4 kWh/t + 153 kg steam/t ([Desmet via GCIRC 2011](https://www.gcirc.org/fileadmin/documents/Proceedings/IRCPrague2011vol2/Oilmill_Refining_Process/1101-1104.pdf) [DATED]); base [ESTIMATE] for modern 20–25 tpd presses |
| 11 | Steam, seed conditioning | 0.10 | 0.15 | 0.25 | t steam/t seed | Desmet 153 kg/t prepress (above) |
| **Refining** | | | | | | |
| 12 | Refining loss, crude → RBD (incl. dewaxing) | 3.5 | 5 | 8 | % of crude | Caustic refining loss 7.1% for sunflower at 12 °Bé (lab study, [Periodica Polytechnica](https://pp.bme.hu/ch/article/download/2650/1755) [DATED]); physical refining has lower neutral-oil loss ([PMC8394065](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8394065/)); base [ESTIMATE] for crude at 1–2% FFA |
| 13 | Bleaching earth | 0.8 | 1.5 | 2.5 | % of oil | [ESTIMATE]: no sourced sunflower figure was found |
| 14 | Refinery utilities | 20 / 0.2 | 30 / 0.3 | 45 / 0.45 | kWh / t steam per t oil | [ESTIMATE] |
| **Aquafeed** | | | | | | |
| 15 | Extrusion line nameplate, Phase 1 | 2 | 3 | 4 | t/h | Design choice; see §3 |
| 16 | Effective throughput / nameplate | 70 | 85 | 90 | % | [ESTIMATE]: die changes, start-ups, fines |
| 17 | Extruder run hours per year, Phase 1 | 3,500 | 4,500 | 6,000 | h | [ESTIMATE]: 2 shifts, ramping to 3 |
| 18 | Grow-out feed crude protein | 28 | 30 | 32 | % | Request spec; matches SamakGro Low-Pro/High-Pro finisher range (market_demand.md) |
| 19 | Sunflower cake inclusion (grow-out) | 10 | 20 | 25 | % | 15% best in Ugandan trial ([LRRD 2012](https://lrrd.org/lrrd24/5/aany24084.htm) [DATED]); 30% SBM-protein replacement neutral ([Egypt study](https://journals.ekb.eg/article_104795.html)); fibre and expansion limit it ([EJABF 2023](https://ejabf.journals.ekb.eg/article_317853.html) [DATED]) |
| 20 | Soybean meal inclusion | 20 | 30 | 35 | % | Formulation §3.3 [ESTIMATE] |
| 21 | Fishmeal / omena inclusion | 0 | 7 | 12 | % | Fishmeal-free tilapia diets viable ([Brazil, Ciência Animal Brasileira](https://new.scielo.br/j/cab/a/GtnVBGQBQLdBFThsBZ7xyBm/?lang=en)); base keeps 7% for palatability [ESTIMATE] |
| 22 | Raw-material cost per t of grow-out feed | 65,000 | 75,000 | 90,000 | KES/t | §3.3, using market_demand.md ingredient prices [ESTIMATE] |
| 23 | Feed process shrink (moisture + fines not recycled) | 1.5 | 2.5 | 4 | % | [ESTIMATE] |
| 24 | Electricity, extruded aquafeed | 70 | 90 | 130 | kWh/t feed | [ESTIMATE]: fine grinding + extruder + dryer fans. Muyang claims 12% energy saving per t from improved shearing ([Engormix](https://en.engormix.com/feed-machinery/extrusion/energy-efficiency-improving-pellet_a34811/)) |
| 25 | Thermal energy, aquafeed (preconditioner steam + dryer) | 0.8 | 1.1 | 1.5 | GJ fuel-equiv/t feed | Dryer 3,000–4,500 kJ/kg water evaporated ([All About Feed](https://allaboutfeed.net/animal-feed/feed-processing/the-economics-of-feed-drying)); ~0.17–0.2 t water removed/t feed [ESTIMATE] |
| **Utilities and labour** | | | | | | |
| 26 | Grid electricity, all-in energy cost (CI1/CI2, ex-VAT) | 16 | 20 | 25 | KES/kWh | Base CI1 energy charge ~15.29 and CI2 ~14.02 KES/kWh for 2025/26 ([EPRA 2023 schedule](https://www.epra.go.ke/wp-content/uploads/2023/01/ABRIDGED-KPLC-TARIFF-2023.pdf) [DATED]), plus pass-throughs ~3.87 KES/kWh (fuel 3.14, forex 0.72, WRA 0.014; Jun 2026, [People Daily](https://peopledaily.digital/business/explainer-how-epras-new-electricity-bill-will-affect-households-and-businesses/amp)), plus levies [ESTIMATE] |
| 27 | Demand charge | 700 | 1,100 | 1,100 | KES/kVA/month | CI2 700, CI1 1,100 (EPRA 2023 schedule [DATED]) |
| 28 | Biomass fuel (wood/briquettes, as-fired ~13–15 MJ/kg) | 5 | 8 | 14 | KES/kg | [ESTIMATE]: no 2026 price found. Sunflower husk HHV ~17.8 MJ/kg ([Univ. Córdoba](https://helvia.uco.es/handle/10396/17436)) |
| 29 | Steam cost, biomass boiler | 2,000 | 2,800 | 4,000 | KES/t steam | [ESTIMATE] = 3.7 GJ fuel/t steam at 75% efficiency × fuel price, plus O&M |
| 30 | Operator wage (gross) | 24,000 | 35,000 | 45,000 | KES/month | 2026 statutory minimum in the five cities: machine attendant 20,455, machine operator 24,359, artisan Grade II 33,087 ([Kenyans.co.ke](https://www.kenyans.co.ke/news/124803-fke-announces-implementation-new-minimum-wages-workers)); market premium [ESTIMATE] |
| 31 | Employer on-costs (NSSF, housing levy, NITA, overtime, medical) | 8 | 15 | 20 | % of gross | [ESTIMATE] |
| 32 | Headcount, Phase 1 | 55 | 70 | 90 | FTE | §4.3 [ESTIMATE] |
| 33 | Maintenance | 2.5 | 3.5 | 5 | % of equipment capex/yr | [ESTIMATE]; plus press wear parts ~KES 100–200/t seed (abrasive sunflower hulls) |
| 34 | Packaging: feed (25 kg PP bag with liner) | 1.5 | 2.0 | 2.8 | KES/kg feed | [ESTIMATE] |
| 35 | Packaging: oil, 20 L jerrican / 1 L PET | 6 / 15 | 8 / 20 | 10 / 28 | KES/L | [ESTIMATE] |
| **Capex (installed, Kenya)** | | | | | | |
| 36 | Phase 1 capex (50 tpd crush, 20 t/d refinery, 3 t/h extrusion, 5 kt silos), excl. working capital | 6.5 | 9.5 | 14 | USD m | Bottom-up §4.1 [ESTIMATE], cross-checked to the benchmarks in §4.2 |
| 37 | Phase 1 working capital (seed season stock, ingredients, receivables) | 2.0 | 3.0 | 4.5 | USD m | [ESTIMATE]: 3–4 months of seed at KES 55–65/kg |
| 38 | Phase 2 incremental capex (to 150 tpd prepress + solvent, 60 t/d refinery, +6 t/h extrusion, +15 kt silos) | 15 | 22 | 32 | USD m | §4.1 [ESTIMATE]; Mainland Dodoma USD 28m for 30–35 kt/yr seed incl. silos and feed line ([Milling MEA](https://millingmea.com/chinese-agribusiness-giant-mainland-group-to-launch-new-sunflower-oil-plant-in-tanzania/)) |
| 39 | Complete aquafeed mill capex per t of annual capacity | 150 | 250 | 400 | USD/t·yr | De Heus Njeru USD 25m/100 kt (2025, [Ecofin](https://www.ecofinagency.com/news-industry/0509-48437-de-heus-invests-25-million-in-ugandan-fish-feed-industry)); Yalelo–Famsun USD 6m/25 kt ([The Fish Site](https://thefishsite.com/articles/new-25000-tpa-fish-feed-mill-to-support-zambias-growing-aquaculture-industry) [DATED 2015]) |
| 40 | Seed storage capex (galvanised silos with aeration) | 80 | 120 | 160 | USD/t stored | [ESTIMATE] |
| 41 | Industrial building (steel portal frame, slab) | 25,000 | 32,000 | 40,000 | KES/m² | [ESTIMATE] |
| 42 | Build time from FID to commissioning, Phase 1 | 12 | 15 | 20 | months | [ESTIMATE]: Chinese lead times 15–60 days ex-works per listings, plus shipping, civil works and permits |
| **Quality** | | | | | | |
| 43 | Aflatoxin design limit, finished fish feed | 5 | 10 | 20 | µg/kg (ppb) | KS 2289-1 limit not retrieved. EU 20 ppb feed materials / 5 ppb some compound feeds ([EU, FAOLEX](https://faolex.fao.org/docs/pdf/eur40481.pdf)); FDA 20 ppb general ([Missouri Dept Agric.](https://agriculture.mo.gov/plants/feed/aflatoxin.php)). Base 10 ppb as an internal release limit [ESTIMATE] |

---

## 1. Oil extraction technology

### 1.1 Options

| Route | Residual oil in cake/meal | Oil recovery (of oil in seed) | Typical scale | Capex intensity | Fit for this project |
|---|---|---|---|---|---|
| Cold pressing (<60 °C) | 12–18% [ESTIMATE] | ~65–75% | 0.5–25 t/d (Bavarian decentral plants averaged 5.2 t/d; [TFZ Bayern](https://www.tfz.bayern.de/mam/cms08/en/dateien/productionofvegetableoilsindecentralplants_biomasswuerzburg1998_wi.pdf) [DATED]) | Lowest | Niche "virgin" oil only. Leaves too much oil in the cake |
| **Full-press hot expeller** (cook/condition 100–120 °C, 1–2 press stages) | **7–12%** (patents, vendor above) | **~75–82%** | 5–150 t/d; mechanical dominates below ~100 t/d ([AMPC](https://www.ampc.montana.edu/documents/briefings/briefing86.pdf)) | Low | **Phase 1** |
| Prepress + hexane solvent extraction | 0.5–1.5% in meal | ~96–98% | >75–200 t/d ([Missouri](https://extension.missouri.edu/media/wysiwyg/Extensiondata/Pub/pdf/energymgmt/em0602.pdf); [AMPC](https://www.ampc.montana.edu/documents/briefings/briefing86.pdf)); one patent squeezes ~2/3 of sunflower oil mechanically and extracts the rest | High, with hazardous-area zoning, a desolventiser-toaster and hexane storage | **Phase 2**, only if ≥120–150 t/d of seed is secured |
| Extrusion-expelling (dry extruder + press), mainly soy | ~6–8% [ESTIMATE] | — | 1–10 t/h | Low–medium | Option for **non-GM soybean**: makes 42–44% CP expeller soy meal for fish feed and avoids the imported-SBM/GMO problem. Directly extruded full-fat soy was the most cost-effective in a Ugandan tilapia study ([Makerere](https://makir.mak.ac.ug/handle/10570/5900)) |

**Note on sources.** A 500 tpd US solvent plant built in 2014 shut in 2016 ([PHX listing](https://www.phxequip.com/Multimedia/documents/plants/solvent-extraction-plant-500-tpd-2318.pdf)). The listing gives no reason, but it is a reminder that solvent plants fail when seed supply fails. Ukrainian vendors sell 300 tpd sunflower extraction sets ([Inventure](https://inventure.com.ua/en/investments/new-vegetable-oil-extraction-equipment-set-with-a-processing-capacity-of-up-to-300-tonnes-of-seeds-per-day)).

### 1.2 Is solvent extraction worth it? [ESTIMATE, using market_demand.md prices]

- Extra oil: going from 31% to 38% yields ~70 kg more oil per t of seed. At ~KES 190/kg crude, that is **+KES 13,300/t seed**. Cake mass falls by 70 kg at ~KES 40/kg, **–KES 2,800**. The gross gain is **~KES 10,500/t seed**.
- Extra opex: hexane loss 1–1.5 kg/t (~KES 250), steam ~0.3 t (~KES 850), power ~15 kWh (~KES 300), labour and maintenance (~KES 850). Total **~KES 2,250/t**, so the net gain is **~KES 8,000–8,500/t seed (~USD 63)**.
- At 45,000 t/yr (150 tpd), the gain is ~KES 370m (USD 2.8m) a year against roughly USD 4–6m of Chinese/Indian solvent plant and safety infrastructure. **Payback is about 1.5–2 years.** At 15,000 t/yr (50 tpd) it is ~USD 0.95m a year against ~USD 3m, with poor economies of scale and serious hexane-safety risk for a first-time operator. **That does not justify it in Phase 1.**
- Integration offsets part of the gain. Residual oil in the ~20–30% of cake used in the company's own fish feed is not lost: it replaces coating oil and dietary energy (tilapia feeds carry 5–8% lipid). The penalty from full pressing is therefore smaller in an integrated plant.
- **Judgement:** full press in Phase 1. Add prepress + solvent in Phase 2 only once ≥40,000 t/yr of seed is under contract or on long-run import.

### 1.3 Seed preparation and filtration (Phase 1 line)
Intake and weighing → pre-cleaner (scalper, aspirator, magnet; removes ~1.5–3% impurities) → **optional dehuller and hull separator** (Phase 2; removes ~8–12% of seed weight as hulls, raises cake CP to ~34–38% and cuts fibre, and the hulls fuel the boiler) → cooker/conditioner (steam-jacketed stack, 100–115 °C, moisture 5–6%) → 2–3 screw presses of 20–25 t/d each (for example the Goyum MK-V-C class, 20 t/24 h, 40 HP ([oilexpeller.com](https://www.oilexpeller.com/?p=5487)), or Chinese 6YL/ZX series) → screening tank (foots go back to the press) → **plate-and-frame or vertical pressure-leaf filter** (with filter aid) → 5–10 µm polishing bag filter → crude oil tanks. Crude specification for sale to refiners: moisture and volatiles ≤0.2%, insoluble impurities ≤0.05–0.1%, FFA ≤2% [ESTIMATE; to agree contractually]. KEBS failed imported oil on "insoluble impurities" and vitamin A in 2023 ([Food Business MEA](https://www.foodbusinessmea.com/kebs-declares-government-imported-cooking-oil-unfit-for-consumption-unveiling-web-of-controversy/)), so filtration quality matters.

### 1.4 Refining: crude vs refined, and is it worth it at small scale?

**Process.** Degumming (water or acid; phosphoric acid 0.05–0.1%) → neutralising (caustic, batch or semi-continuous) or, for physical refining, deep acid degumming to <10 mg/kg phosphorus ([PMC8394065](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8394065/)) → bleaching (activated earth, 0.8–2.5%) → **dewaxing/winterisation** (essential for clear sunflower oil in bottles; chill to 5–8 °C, then filter) [ESTIMATE, standard practice] → deodorising (230–250 °C, high vacuum; a thermal-oil heater is needed) → vitamin A (and D) fortification → filling. Tocopherol losses average 30% (chemical) and 36% (physical) ([Trakya Univ.](https://dspace.trakya.edu.tr/items/059efa67-ab2a-4747-b7cc-a601cc14d9d4/full)).

**Chemical vs physical.** Physical refining has lower neutral-oil loss and recovers FFA as a by-product, but it needs well-degummed, low-phosphorus oil ([PMC8394065](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8394065/)). Caustic refining of sunflower lost ~7.1% in one study ([BME](https://pp.bme.hu/ch/article/download/2650/1755)). **Recommendation [ESTIMATE]:** use a semi-continuous chemical line with winterisation for Phase 1, because it tolerates variable smallholder crude. Move to continuous physical refining in Phase 2.

**Equipment prices (listings, not quotes).** Semi-continuous physical refinery for 10–50 t/d from USD 30k (Xinxiang Hongyang); a 30 tpd soybean press plus refining "turnkey" line at USD 65–68k FOB (Henan Fangchuangjie) ([made-in-china](https://m.made-in-china.com/hot-china-products/Refining_Process.html)); a complete sunflower refinery at USD 160k (Anyang Best, capacity not stated). Tanzania: a refinery "valued at TZS 1.5bn" (~USD 0.55–0.6m) for ~30 t ([The Exchange](https://theexchange.africa/?p=49868), undated). The listings are bare equipment. **My installed Phase 1 estimate for a 20 t/d oil refinery with winterisation, tank farm (500 t crude + 300 t refined), fortification dosing and a 20 L/5 L/1 L filling line is USD 0.6–1.2m (base 0.9m)** for Chinese mid-tier equipment, or USD 1.5–2.5m European (Desmet, Alfa Laval, Andritz) [ESTIMATE].

**Economics per t of crude [ESTIMATE, using market_demand.md prices].** Crude sold to refiners fetches ~KES 180–195k/t (5–12% below import parity, with buyer power held by Bidco, Pwani and Kapa). Refined bulk sells ex-works at ~KES 264k/t. The refining cost is about:
- loss of 5% × 190k = KES 9.5k
- chemicals and bleaching earth ~KES 1.5k
- energy ~KES 1.5k
- labour and maintenance ~KES 2k
- fortificant ~KES 0.3k
- depreciation ~KES 2.5k

That totals **~KES 17–18k/t**, leaving a net margin of **~KES 55k/t before packaging and distribution**, or ~KES 45k/t if sold in 20 L jerricans to institutions and wholesalers. On ~4,400 t/yr that is **~KES 200m/yr (~USD 1.5m) on ~USD 0.9m of capex**.

**Regulatory push towards refining.** Vegetable fats and oils sold for food must be fortified with vitamin A ([FAOLEX Kenya](https://faolex.fao.org/docs/pdf/ken115324.pdf); Bidco and Kapa comply by adding premix, [ATNi 2025](https://accesstonutrition.org/app/uploads/2025/07/20250701_ATNi_EAMA_Kenya_Micronutrients_v2.pdf)). Unfortified, unrefined oil therefore cannot be legally retailed as cooking oil, except arguably as a niche "virgin" product that still needs fortification.

**Judgement: refine in Phase 1.** The main risk is commercial, not technical: building distribution against an oligopoly. A crude-only fallback depends on refiners' willingness to buy, and Bidco reportedly sources only ~5 kt of local seed (market_demand.md).

**Small-scale reference.** AFA's Lamu common-user facility crushes 5 t of seed and refines 500 L of oil per day ([Milling MEA](https://millingmea.com/kenya-commissions-edible-oil-facility-in-lamu-county/)). It shows that micro-refining exists, but at uneconomic scale for a commercial investor.

---

## 2. Feedstock (engineering view)

- **[CONFLICT] Kenyan sunflower output** is about 80,000 t according to a Ministry official (KNA, e.g. [?p=179463](https://www.kenyanews.go.ke/?p=179463); exact page attribution not confirmed), but ~6,000 t on FAOSTAT-based data ([Selina Wamucii](https://www.selinawamucii.com/insights/prices/kenya/sunflower-seeds)). Nakuru alone claims ~9,500 t from >9,000 ha in one report and 3,000 t in another (KNA pages, e.g. [?p=141371](https://www.kenyanews.go.ke/?p=141371); attribution not confirmed). The Edible Oil Crops Promotion Project (Jul 2023–Jun 2028) targets Bungoma, Busia, Kakamega, Nakuru, Uasin Gishu, Trans Nzoia and others, aiming to expand oil crops from 60,000 to 250,000 ha ([KNA](https://www.kenyanews.go.ke/government-rolls-out-sunflower-project-to-boost-local-production-of-edible-oils/)).
- **Implication:** a 50 tpd plant needs 15,000 t/yr, which is 20–100% of reported national output. Phase 1 must source on four legs:
  1. outgrower contracts in Busia, Bungoma and Kakamega
  2. Tanzanian sunflower seed (cross-border trade is already active in Kajiado, [Nation](https://nation.africa/kenya/business/seeds-of-gold/the-cross-border-sunflower-trade-transforming-kajiado-s-economy--5530502))
  3. non-GM soybean from Uganda/Zambia/Malawi
  4. cottonseed from western Kenya and Uganda
- **Multi-seed line.** The plant should be able to crush sunflower, soy (via an extruder-expeller) and cottonseed (after delinting; gossypol limits fish-feed inclusion to ~5–8% [ESTIMATE]).
- **Seasonality.** Western Kenya has two rain seasons, so seed arrives in 2 peaks. Storage must hold **3–4 months of throughput (4,000–5,000 t in Phase 1)** [ESTIMATE].
- **Seed cost.** In Tanzanian small processors, raw material was 61% of total cost ([Dodoma study](https://ageconsearch.umn.edu/record/343092/files/COST%20EFFICIENCY%20OF%20SMALL%20SCALE%20SUNFLOWER%20PROCESSORS%20IN%20TANZANIA_035446.pdf) [DATED]). In this project seed is ~70–80% of crushing cash cost [ESTIMATE].

---

## 3. Extruded floating fish-feed line

### 3.1 Twin-screw vs single-screw

| Criterion | Single-screw (e.g. Andritz, Famsun SJPS, Chinese generic) | Twin-screw (e.g. Famsun MY series, Wenger TX, Clextral, Bühler) |
|---|---|---|
| Starch needed for reliable float | ≥20–25% [ESTIMATE] | ~10–15% [ESTIMATE] |
| Tolerance of fibre, fat and fines (sunflower cake at 20%+) | Moderate | High |
| Small pellets (0.8–2 mm fry/fingerling) | Difficult | Good |
| Capex for the same t/h | 1.0× | ~1.4–2.0× [ESTIMATE] |
| Wear-part cost | Lower | Higher |
| Capacity range | Andritz single-screw 2–12 and 10–20 t/h ([Andritz](https://andritz.com/products-en/tiac/feed-biofuel/extruders-aqua-feed)) | Famsun MY120 7.5 t/h at Yalelo, Zambia ([The Fish Site](https://thefishsite.com/articles/new-25000-tpa-fish-feed-mill-to-support-zambias-growing-aquaculture-industry) [DATED]) |

**Recommendation: twin-screw**, at ~3 t/h in Phase 1 and ~6 t/h in Phase 2. The base formula relies on high-fibre sunflower cake and only ~15% starch, and fingerling sizes are where the margin is highest (KES 160–250/kg vs 110–150/kg for grow-out, market_demand.md). Chinese industry context: by 2013 there were already >300 Chinese aquafeed extrusion lines above 5 t/h, moving towards 10 t/h ([All About Feed](https://allaboutfeed.net/animal-feed/feed-additives/growing-trend-of-asian-extruded-aquatic-feeds) [DATED]).

### 3.2 Process train and pellet sizes
Ingredient intake (bag tipping and bulk) → pre-grinding (hammer mill) → batching scales and mixer → **fine grinding / pulveriser to <250 µm (≥95% through 425 µm)**, which is critical for floating and water stability → mixer → preconditioner (steam + water to 22–28% moisture, 90–95 °C) → extruder and die (for example 2, 3, 4 and 6 mm) → pneumatic conveying → multi-pass belt dryer to ≤10% moisture → drum coater (1–4% oil; vacuum coating is not needed for tilapia) → counter-flow cooler → screener (fines recycled, ~3–5%) → 25 kg bagging [ESTIMATE, standard design]. Dryer exhaust heat recovery saves 20–100 kWh thermal per t ([Petfood Industry](https://www.petfoodindustry.com/articles/2499-target-sustainable-petfood-processing)).

Pellet sizes and CP [ESTIMATE; align with KS 2289-1 stage definitions]:
- powder/crumble 0.3–1 mm at 40–45% CP (fry)
- 1.5–2 mm at 35–38% (fingerling)
- 3 mm at 30–32% (grower; SamakGro sells 3 mm grower)
- 4–6 mm at 28–30% (finisher; SamakGro 4 mm finisher)

### 3.3 Base grow-out formulation (~30% CP floating) [ESTIMATE; to be optimised by a nutritionist with least-cost software]

| Ingredient | Inclusion % | CP contribution (pp) | Price used (KES/kg) | KES per kg feed |
|---|---|---|---|---|
| Sunflower cake (own, expeller, ~30% CP, ~10% oil) | 20 | 6.0 | 40 (transfer price) | 8.0 |
| Soybean meal / own expeller soy cake (~45% CP, non-GM) | 30 | 13.5 | 95 | 28.5 |
| Omena / fishmeal (~58% CP) | 7 | 4.1 | 160 | 11.2 |
| Cottonseed cake (decorticated, ~38% CP) | 5 | 1.9 | 38 | 1.9 |
| Maize (or maize germ) | 18 | 1.4 | 50 | 9.0 |
| Wheat pollard | 13 | 2.1 | 32 | 4.2 |
| Wheat bran | 2.5 | 0.4 | 25 | 0.6 |
| Own crude sunflower oil (in mash + coating) | 2 | — | 190 | 3.8 |
| Premix, DCP, salt, lysine, methionine, binder, mould inhibitor, toxin binder | 2.5 | 0.3 | 250 | 6.3 |
| **Total** | **100** | **~29.7% CP** | | **~73.5** |

- Calculated nutrients [ESTIMATE]: lipid ~6.7%, crude fibre ~8.4%, starch ~15% (twin-screw needed).
- **Fibre is the binding constraint.** Feedipedia puts non-dehulled cake at 20%+ fibre. Ugandan trials used up to 15% sunflower cake ([LRRD](https://lrrd.org/lrrd24/5/aany24084.htm) [DATED]). Wheat bran above ~10% and SBM above ~20% retarded growth in Ogunji & Wirth (2001), as cited in search snippets (URL not confirmed) [DATED]. Up to 25% of fishmeal protein can be replaced by SBM without growth loss at 30% CP ([NIOF Egypt](https://niof-eg.com/wp-content/uploads/2022/07/USE-OF-SOYBEAN-MEAL-AND-OR-CORN-GLUTEN-MEAL-AS.pdf)). Fully fishmeal-free soy diets gave lower cost per kg of fish in Brazil ([Ciência Animal Brasileira](https://new.scielo.br/j/cab/a/GtnVBGQBQLdBFThsBZ7xyBm/?lang=en)). Dehulling (Phase 2) would allow 25–30% sunflower meal.
- **Raw-material cost ≈ KES 73.5/kg.** With 2.5% shrink it is ~KES 75/kg. Conversion cost is ~KES 12–18/kg (§4.3), so the **cash cost is ~KES 88–93/kg** against a KES 110–150/kg ex-mill price (market_demand.md).
- **Omena risk.** Fishmeal is often aflatoxin-contaminated and omena supply is tight (2024 statement by a Kiambu poultry cooperative, seen in search snippets; page not confirmed [DATED]). FAO has flagged feed–food competition over *Rastrineobola argentea* ([FAO](https://fao.org/docrep/pdf/010/a1444e/a1444e16.pdf) [DATED]). Design a 0–3% fishmeal variant using soy, insect (BSF) meal or blood meal [ESTIMATE].

### 3.4 Cake balance: aquafeed absorbs only a fraction of the cake
At 20% inclusion, 10,000 t of feed uses ~2,050 t of sunflower cake. Phase 1 crushing makes ~9,600 t, so **~75–80% of the cake must be sold to dairy/poultry feed millers** (~KES 40/kg, Rift Valley and Central dairy belt). Nationally, feed millers run at 50–60% of capacity (market_demand.md), so a separate dairy/poultry mash line adds little. **Crushing soy instead of part of the sunflower would let the company's own cake replace the 30% SBM share**, which is the most valuable integration lever.

---

## 4. Capex and opex

### 4.1 Bottom-up capex [ESTIMATE; Chinese mid-tier equipment (Famsun/Muyang for extrusion, Henan/Zhengzhou or Indian for oil) unless stated]

| Item | Phase 1 (USD m) | Phase 2 increment (USD m) | Notes |
|---|---|---|---|
| Land 6–10 acres (purchase) or lease/SEZ plot | 0.6 | 0.3 | Kisumu peri-urban ~KES 5–15m/acre [ESTIMATE; no 2025–26 industrial data found]; Athi River averaged KES 21.3m/acre at end-2025 ([HassConsult via AllAfrica](https://allafrica.com/stories/202601270545.html)); a 36-acre Athi River industrial plot listed at KES 30m/acre (May 2026, [listing](https://kenyapropertycentre.com/for-sale/land/industrial-land/machakos/athi-river/63388-prime-36-acre-industrial-property)) |
| Civil works and buildings (~4,500 m² P1; +6,000 m² P2) | 1.2 | 2.5 | KES 25–40k/m² [ESTIMATE] |
| Seed silos and receiving/pre-cleaning (5 kt P1; +15 kt P2) | 0.5 | 1.8 | USD 80–160/t stored [ESTIMATE]; Mainland Dodoma included 4 silos totalling 30 kt ([Milling MEA](https://millingmea.com/chinese-agribusiness-giant-mainland-group-to-launch-new-sunflower-oil-plant-in-tanzania/)) |
| Crushing: 50 tpd full press (P1); to 150 tpd prepress + dehulling + flaking (P2) | 0.8 | 2.0 | Equipment ~USD 10–16k per tpd installed for Chinese/Indian presses [ESTIMATE]; Indian 8 tpd expeller at INR 0.3m (~USD 3.5k) bare ([IndiaMART](https://m.indiamart.com/impcat/oil-extraction-machine.html)) |
| Solvent extraction 150–200 tpd with desolventiser-toaster, hexane farm and safety zone | — | 4.5 | European ~2× [ESTIMATE] |
| Refinery and packing: 20 t/d semi-continuous (P1); 60 t/d continuous physical (P2) | 0.9 | 2.5 | §1.4 |
| Extrusion: 3 t/h twin-screw full line (P1); +6 t/h (P2) | 1.9 | 3.5 | §4.2 |
| Utilities: biomass boiler (3–4 t/h P1; +10 t/h P2), thermal-oil heater, 1.6 MVA transformer and 1 MVA standby genset, borehole and water treatment, ETP, fire system | 1.1 | 2.0 | [ESTIMATE] |
| QC laboratory | 0.15 | 0.1 | §7 |
| Vehicles and forklifts | 0.3 | 0.3 | |
| Engineering, freight, duties (IDF/RDL ~4.5–5.5% of customs value; verify against the Finance Act 2026), permits, pre-operating | 0.75 | 1.0 | [ESTIMATE] |
| Contingency (15% P1, ~10% P2) | 1.2 | 1.8 | |
| **Total capex** | **~9.4** | **~22** | Low/high: P1 6.5–14; P2 15–32 |
| Working capital | ~3.0 | +5–7 | Seed inventory is the big item: 4 months × 3,750 t × KES 60k ≈ KES 0.9bn at Phase 2 |

**Chinese vs European, rule of thumb [ESTIMATE]:**
- European extrusion (Andritz, Bühler, Wenger, Clextral): ~2.5–4× Chinese generic and ~1.5–2.5× Famsun/Muyang for the same t/h.
- A 3 t/h line: ~USD 0.25–0.5m Chinese generic, ~USD 1.2–1.8m Famsun/Muyang turnkey, ~USD 3–5m European (all ex-works plus erection).
- Base case: Famsun/Muyang-class, for spares, service and references (Famsun supplied Yalelo).

### 4.2 Benchmarks (external)

| Plant | Scope | Investment | Implied intensity | Source |
|---|---|---|---|---|
| De Heus, Njeru (Uganda), opened 2 Sep 2025 | Aquafeed, up to 100 kt/yr | USD 25m (€22m per another source) [CONFLICT] | ~USD 250/t·yr | [De Heus](https://www.deheus.com/articles/news/de-heus-opens-state-of-the-art-fish-geed-factory-in-uganda-supporting-aquaculture-growth-in-east-africa); [Ecofin](https://www.ecofinagency.com/news-industry/0509-48437-de-heus-invests-25-million-in-ugandan-fish-feed-industry); [AllAfrica](https://allafrica.com/stories/202509040050.html) |
| Yalelo–Famsun, Zambia (2015–16) | Turnkey aquafeed mill, 25 kt/yr expandable to 50 kt, MY120 twin-screw 7.5 t/h | USD 6m | ~USD 240/t·yr [DATED] | [The Fish Site](https://thefishsite.com/articles/new-25000-tpa-fish-feed-mill-to-support-zambias-growing-aquaculture-industry) |
| Victory Farms, Doho (Homa Bay) | Extruded fish-feed mill (part of a KES 2.2bn project incl. KES 390m hatchery and ponds) | KES 1.3bn (~USD 10m) | Capacity not disclosed | [The Standard](https://www.standardmedia.co.ke/business/nyanza/article/2001549421/new-bid-to-improve-fish-production-in-homa-bay); [Streamline](https://streamlinefeed.co.ke/news/victory-farms-invests-kes-4-5-billion-tech-slash-homa-bay-fish-prices) |
| SamakGro, Naivasha (Maxim Agri / Victory Farms / Gatsby Africa) | Feed mill sourcing up to 35 kt of ingredients/yr; AgDevCo mezzanine (amount undisclosed) | n/a | — | [The Fish Site](https://thefishsite.com/es/articles/african-aquaculture-leaders-join-forces-to-build-feed-mill-maxim-agri-victory-farms-gatsby-africa) [DATED 2022] |
| Tunga Nutrition (Skretting/Unga), Nairobi | Aquafeed 24 → 45 kt/yr (was ~10 kt in 2022) [CONFLICT on baseline] | Not disclosed | — | [WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi); [FeedNavigator 2022](https://WWW.FEEDNAVIGATOR.COM/Article/2022/02/01/nutreco-forms-animal-and-fish-feed-joint-ventures-in-kenya-and-uganda) |
| Unga Farm Care, Nairobi | 5,000 t/yr extruded fish feed | n/a | — | [Seaboard Overseas](https://www.seaboardoverseas.com/unga-farm-care-ea-limited-opens-5000-mt-per-year-extruded-fish-feed-plant-nairobi/) [DATED] |
| Kisumu Fisheries Centre of Excellence (public), Kabonyo | Includes a fish-feed mill, training and research | USD 19.3m total | Public competitor or partner | [Food Business MEA](https://www.foodbusinessmea.com/?p=2133722) (date unclear) |
| Mainland Group, Dodoma (Tanzania) | Sunflower crushing 30–35 kt seed/yr, 30 kt silos, cake-to-feed line | USD 28m | ~USD 800–930/t seed·yr, or ~USD 250–280k per tpd (full scope) | [Milling MEA](https://millingmea.com/chinese-agribusiness-giant-mainland-group-to-launch-new-sunflower-oil-plant-in-tanzania/); [TanzaniaInvest](https://tanzaniainvest.com/?p=26552) |
| Homa Bay County investor call | Oil mill 85 kt/yr (palm/sunflower) + 15,000 ha nucleus farm | USD 27.5m (estimate) | Includes the farm | [KenInvest](https://opportunities.invest.go.ke/opportunities/opportunity/edible-oil-production-1) |
| AFA Lamu common facility | 5 t/d crush, 500 L/d refine | n/a | — | [Milling MEA](https://millingmea.com/kenya-commissions-edible-oil-facility-in-lamu-county/) |
| Agventure (canola, Timau) | Canola crushing and seed; AgDevCo USD 9.5m mezzanine (Nov 2024) | Capacity not disclosed | — | [AgDevCo PR](https://www.agdevco.com/site/assets/files/2133/agventure_press_release_nov_2024.pdf) [DATED] |
| Kenyan edible-oil industry | 13 processors invested ~KES 100bn over 5 years (KAM, as reported) | — | Mostly palm refining | [KenInvest](https://opportunities.invest.go.ke/opportunities/opportunity/edible-oil-production-1) |
| Small Chinese/Indian lines (listings) | 2 t/h floating line USD 78k "sample" ([Alibaba](https://www.alibaba.com/product-detail/_1600909115028.html)); IITA: 120–150 kg/h line USD 18k, 4–5 t/h line USD 85k ex-shipping ([IITA PROPAS](https://propas.iita.org/en/solutions/formulation-and-pelleting-of-low-cost-feeds/109/export/)); Indian 1 t/h full line INR 9.39m (~USD 110k) ([IndiaMART](https://m.indiamart.com/proddetail/sinking-and-floating-fish-feed-processing-line-17906853762.html)) | — | Bare equipment, not comparable | |

**Read-across.** The Phase 1 feed line (3 t/h, ~10–12 kt/yr) at ~USD 3m all-in (equipment 1.9m plus its share of buildings, utilities and contingency) is ~USD 250–300/t·yr, in line with De Heus and Yalelo. The lean crushing and refining side is ~USD 430/t seed·yr, about half of Mainland's full-scope intensity. That gap reflects lean scope (no solvent plant, smaller silos, Chinese presses) but **is the main capex risk, so the high case is +50%**. I found no capex figures for Menengai, Sigma Feeds or Unga's oil and feed lines (gap).

### 4.3 Opex

**Energy.**
- Tariff: EPRA's 2026–29 retail tariff application was withdrawn in June 2026, so base tariffs are unchanged ([Kenya Times](https://thekenyatimes.com/latest-kenya-times-news/epra-gives-way-forward-after-withdrawal-of-new-electricity-tariff/)). Monthly fuel and forex pass-throughs continue (~KES 3.87/kWh in Jun 2026, [People Daily](https://peopledaily.digital/business/explainer-how-epras-new-electricity-bill-will-affect-households-and-businesses/amp); new April 2026 charges, [Capital FM](https://capitalfm.africa/electricity-bills-set-to-rise-as-epra-introduces-new-april-2026-charges/)).
- **[CONFLICT]** Nation reports industrial (>15,000 kWh/month) power at KES 13.44/kWh for FY to Jun 2026 ([Nation](https://beta.nation.co.ke/kenya/business/companies/kenya-power-takes-biggest-sales-fall-from-industrial-users-5282278)), apparently excluding pass-throughs. AfroTools gives ~KES 15/kWh for industrial use ([AfroTools](https://afrotools.com/tools/electricity-tariff/kenya/), unofficial).
- **Risk:** Kenya Power warned that county wayleave charges could force a >30% rise ([Serrari](https://serrarigroup.com/kenya-power-warns-of-30-increase-in-electricity-prices-amid-mounting-wayleave-charges-and-debt-crisis/)).
- Base **KES 20/kWh all-in**, plus the demand charge.

| Phase 1 energy (base year at full rate) | Quantity | Cost (KES m/yr) |
|---|---|---|
| Electricity: crushing 15,000 t × 60 kWh + refining 4,650 t × 30 + feed 10,000 t × 90 + general 0.2 GWh | ~2.2 GWh | ~44 |
| Demand charge ~900 kVA × KES 1,100 × 12 | | ~12 |
| Steam: crushing 2,250 t + refinery ~1,400 t + feed ~3,500 t = ~7,150 t | ~26 TJ fuel, ≈ 1,900 t wood/briquettes | ~15–20 (at KES 8/kg) |
| Standby diesel (outages; assume 3–5% of hours) | | ~5–8 [ESTIMATE] |
| **Total** | | **~76–84 (~USD 0.6m)** |

- Per tonne [ESTIMATE]: **crushing ~KES 1,600–2,000/t seed; extruded feed ~KES 2,800–3,300/t**.
- Furnace oil instead of biomass would cost ~KES 70m+/yr in fuel, so a biomass boiler is clearly better.
- **Hull self-sufficiency in Phase 2.** Hulls fall out at ~10% of seed with partial dehulling (4,500 t/yr at 45 kt) [ESTIMATE]. At ~15 MJ/kg as-fired that is ~65 TJ, which roughly covers the ~45–60 TJ thermal demand of Phase 2. A French crushing plant added a dehuller and hull boiler for "energetic independence" ([OCL 2012](https://www.ocl-journal.org/articles/ocl/pdf/2012/06/ocl2012196p332.pdf) [DATED]). Husk ash is alkali-rich and causes fouling, slagging and corrosion, so specify a boiler designed for agri-residues ([LAPSE 2023](https://psecommunity.org/wp-content/plugins/wpor/includes/file/2302/LAPSE-2023.8652-1v1.pdf) [DATED]).

**Labour (Phase 1, ~70 FTE) [ESTIMATE].**
- Management, 6: GM KES 600k, plant manager 350k, finance 250k, procurement/outgrower 200k, sales 200k, QA manager 200k per month.
- Lab, 4 at KES 80k.
- Operators, 41 at KES 35–40k: crushing 3 shifts × 4; refinery/packing 17; extrusion 2 shifts × 6.
- Maintenance, 6 at KES 70k, including a DOSHS-certified boiler operator and electricians.
- Stores, logistics and drivers, 8 at KES 35k.
- Gross ~KES 4.4m/month; ~KES 61m/yr including 15% on-costs (**~USD 0.47m**).
- Field extension officers for outgrowers (6–10 at KES 50k): ~KES 5–6m/yr.
- Statutory floors: machine operator KES 24,359 and machine attendant KES 20,455 (five cities, 1 May 2026, [Kenyans.co.ke](https://www.kenyans.co.ke/news/124803-fke-announces-implementation-new-minimum-wages-workers)). **[CONFLICT]** WageIndicator lists 21,749 and 18,263 for Nairobi/Mombasa/Kisumu ([WageIndicator](https://wageindicator.org/en-ke/ai/work-in-kenya/minimum-wage/2182-cities-nairobi-mombasa-and-kisumu/)). The 2026 minimum-wage rise was 12% ([Nation](https://nation.africa/kenya/news/the-12pc-minimum-wage-bombshell--5519274)).

**Other opex [ESTIMATE].**
- Maintenance: 3.5% of equipment capex (~KES 25m/yr in Phase 1) plus press wear parts KES 150/t seed.
- Packaging: feed KES 2.0/kg; oil KES 8/L in 20 L, KES 20/L in 1 L PET; cake bags KES 0.7/kg.
- Refining chemicals: KES 1.5k/t oil.
- Lab running costs and external accredited tests: KES 6–10m/yr.
- Insurance: 0.5% of asset value.
- Security and outsourced cleaning: KES 6m/yr.

**Unit conversion cost (excluding raw material and depreciation), base:**
- **crushing ~KES 4,500–6,000/t seed**
- **refining ~KES 7,000–9,000/t oil (excluding packaging)**
- **extruded aquafeed ~KES 12,000–18,000/t**

---

## 5. Recommended phased configuration and mass balance

### 5.1 Phases
- **Phase 0 (6–9 months, ~USD 0.3–0.5m) [ESTIMATE].** Seed-aggregation pilot with outgrowers in Busia and Bungoma, plus import-seed contracts. Toll-crush or rent capacity. Feed formulation trials, for example toll-extrusion at an existing mill or KMFRI Sangoro/Kegati trials. This tests the binding constraint (seed) before committing ~USD 12m.
- **Phase 1 (build 12–18 months; Year 1–3).** 50 tpd multi-seed full-press crushing, 20 t/d semi-continuous refinery with winterisation and fortification, packing (20 L, 5 L, 1 L), 3 t/h twin-screw extrusion line (~10–12 kt/yr feed), 5 kt silos, 3–4 t/h biomass boiler, QC lab. **Capex ~USD 9.5m (6.5–14) + WC ~USD 3m.**
- **Phase 2 (Year 3–5; gated).** Proceed only if three conditions hold: (a) ≥40 kt/yr of seed is contracted or reliably importable, (b) feed sales reach ≥8 kt/yr at a ≥20% gross margin, (c) the Phase 1 refinery runs at >70%. Scope: crushing to 150 tpd with dehulling, prepress and a 150–200 tpd solvent plant; continuous physical refinery to 60 t/d; a second 6 t/h extrusion line (total ~35–40 kt/yr); +15 kt silos; hull-fired 10 t/h boiler. **Incremental capex ~USD 22m (15–32) + WC ~USD 5–7m.**

### 5.2 Phase 1 mass balance (base, full rate: 50 tpd × 300 d, 100% sunflower)

```
Sunflower seed in .................................. 15,000 t (40% oil, 8% moisture)
 ├─ cleaning impurities (2%) ........................    300 t  -> boiler fuel / waste
 ├─ conditioning moisture loss (2%) .................    300 t  -> vapour
 ├─ filtered crude oil (31%) ........................  4,650 t  (~5,080 m3)
 │    ├─ to aquafeed (2% of feed) ...................    205 t
 │    └─ to refinery ................................  4,445 t
 │         ├─ refined fortified oil (95%) ...........  4,220 t  (~4,610 m3)
 │         └─ gums, soapstock, FFA, waxes (5%) ......    225 t  -> soap makers / acid oil
 ├─ expeller cake (64%; ~10% oil, ~30% CP) ..........  9,600 t
 │    ├─ to aquafeed (20% of mash) ..................  2,050 t
 │    └─ sold to dairy/poultry feed millers .........  7,550 t
 └─ foots / handling (1%, mostly recycled) ..........    150 t

Aquafeed: mash in 10,250 t -> finished floating feed 10,000 t (2.5% shrink)
 Inputs: own sunflower cake 2,050 | SBM or own soy cake 3,075 | omena/fishmeal 718 |
         cottonseed cake 513 | maize 1,845 | wheat pollard 1,333 | wheat bran 256 |
         own crude oil 205 | premix/minerals/amino acids/binder 256
 Extruder: 3 t/h nameplate × 85% × ~4,000 h ≈ 10,200 t/yr (2 shifts, 5–6 days)
```

**Variant with soy (recommended mix: 10,000 t sunflower + 5,000 t non-GM soy) [ESTIMATE]:**
- Soy via extruder-expeller gives ~12–13% oil (~630 t) and ~80–82% cake at ~42–44% CP (~4,050 t). That covers all 3,075 t of SBM demand, with ~1,000 t surplus for poultry feed.
- Sunflower gives 3,100 t oil and 6,400 t cake.
- Total crude oil ~3,730 t. Lower oil revenue, but it removes ~KES 290m/yr of SBM purchases and the GMO-import exposure.

### 5.3 Phase 2 mass balance (base, 45,000 t/yr seed, prepress + solvent, partial dehulling)
- Oil 38%: 17,100 t
- Meal (~1% oil, ~35% CP): 47%, 21,150 t
- Hulls: 10%, 4,500 t, to the boiler
- Impurities, moisture and other losses: 5%, 2,250 t

Aquafeed at ~30 kt/yr would use ~7,500 t of meal (25% inclusion), so ~13,600 t is sold.

---

## 6. Site selection

Approximate road distances from Kisumu [ESTIMATE, map-based]: Bondo/Siaya ~60–70 km, Homa Bay ~130 km, Busia ~115 km, Bungoma ~110 km, Eldoret ~160 km, Nakuru ~190 km, Nairobi ~345 km, Mombasa ~820 km.

Cage geography (2019 frame survey [DATED]): Siaya 81% of 3,696 cages, Homa Bay 479, Busia 120, Kisumu 85. By 2025 there were ~7,000 cages (market_demand.md).

| Criterion (weight) | Kisumu peri-urban | Homa Bay / Siaya | Busia | Bungoma / Eldoret | Nakuru / Naivasha SEZ | Athi River / Mombasa |
|---|---|---|---|---|---|---|
| Feedstock access (25%) | 4: Busia/Bungoma/Kakamega seed + Uganda soy, 110–140 km | 2 | 4: border with Uganda (soy, maize, cottonseed, sunflower) | 5: sunflower belt, Trans Nzoia/Uasin Gishu maize and soy, Kenya Seed sunflower factory in Kitale (KNA search results, specific page not confirmed) | 3: Nakuru sunflower and canola region | 2: imported seed only |
| Distance to cage customers (20%) | 5 | 5 | 4 | 3 | 2 | 1 |
| Market for surplus cake: dairy/poultry belt (10%) | 3 | 2 | 2 | 4 | 5 | 4 |
| Power quality and tariff (10%) | 4 | 2 | 3 | 4 | 5: geothermal, SEZ | 4 |
| Water (5%) | 5: lake and boreholes | 4 | 3 | 3 | 3 | 2 |
| Land cost and availability (10%) | 3 | 4 | 4 | 4 | 3 | 2: ~KES 21–30m/acre Athi River |
| Logistics and import access (10%) | 4: Kisumu port, MGR, Uganda | 2 | 4 | 3 | 5: SGR ICD | 5 |
| SEZ/EPZ availability (5%) | 2: none confirmed | 1 | 2 | 2: "AEZ Eldoret" proposed ([UNCTAD 2022](https://unctad.org/system/files/non-official-document/aldc_2022_pdsd_pdw_ken_ppt_16-18_mar_francis_gitau_eng.pdf) [DATED]) | 5: Naivasha SEZ, 1,000 acres ([Capital FM](https://capitalfm.africa/inside-kenyas-sez-strategy-are-dongo-kundu-naivasha-and-tatu-city-delivering/)) | 5: Dongo Kundu, 3,000 acres; Athi River EPZ |
| Skills and labour (5%) | 4 | 2 | 3 | 4 | 4 | 5 |
| **Weighted score** | **3.95** | 2.85 | 3.50 | 3.80 | 3.55 | 2.80 |

Scores are my judgement [ESTIMATE].

**SEZ context.** Kenya has ≥36 gazetted SEZs in 14 counties (or "over 25", depending on period). Realised SEZ investment was ~USD 961m with 4,392 jobs against 26,000 projected ([Capital FM, Jul 2026](https://capitalfm.africa/inside-kenyas-sez-strategy-are-dongo-kundu-naivasha-and-tatu-city-delivering/)). SEZ incentives are capped at 10 years (macro notes). A private single-enterprise SEZ licence may be possible; verify with SEZA.

**Recommendation.**
- Locate in **peri-urban Kisumu** (e.g. the Kisumu–Busia road, Kibos/Mamboleo, or near the port), with **seed-buying and pre-cleaning depots at Busia and Bungoma**.
- **Bungoma/Eldoret is a close second.** Crushing does not reduce transported mass much (oil + cake ≈ 95% of seed), so the choice is driven by where the feed and cake go: fish feed to the lake, cake to the Rift dairy belt. Kisumu sits between the two.
- Avoid Homa Bay/Siaya for the processing plant: weak power and roads, and it would head-to-head with Victory Farms' Doho mill. Use a depot there instead.
- Avoid Athi River/Mombasa: it contradicts the local-oilseed thesis and puts the plant on the palm refiners' home turf.
- **Water demand** is ~30–50 m³/day in Phase 1 (boiler make-up, refinery, preconditioner, domestic) [ESTIMATE]. **Power** needs are ~1.1–1.3 MW connected load in Phase 1, needing a 1.6 MVA transformer on an 11 kV supply (CI2) and a ~1 MVA standby genset. An extruder trip mid-run blocks the die, so standby power is a process requirement, not a luxury.

---

## 7. Quality, standards and permits

| Area | Requirement | Source / status |
|---|---|---|
| Fish feed | **KS 2289-1:2016, Compounded tilapia feeds, Part 1: complete feeds** (starter, grower, finisher, brooder). The aflatoxin clause was not retrieved | [WTO TBT notification](https://members.wto.org/crnattachments/2016/TBT/KEN/16_4795_00_e.pdf) [DATED]; the page could not be fetched (DNS) |
| Fish-feed oversight | Fisheries Management and Development (Safety and Quality) regulations cover import/export of fish feed, accredited labs, permits and licences (Gazette Supplement No. 149 of 2024). Small feed makers are poorly monitored | [UNEP LEAP](https://leap.unep.org/en/countries/ke/national-legislation/fisheries-management-and-development-safety-and-quality); [Chuka Univ.](https://repository.chuka.ac.ke/handle/123456789/16476) |
| Aflatoxin | Kenyan food limits: 10 ppb maize, 15 ppb peanut butter ([Rödl](https://roedl.com/insights/life-sciences-law/kenya-aflatoxin-food-cancer-contamination-legal)). Cereals found at up to 500 ppb ([Kenyans.co.ke/KALRO](https://www.kenyans.co.ke/news/123956-kalro-kebs-warn-dangerous-aflatoxin-levels-cereals-sold-kenyan-markets)). Fish feeds in Nyeri contaminated ([Toxins 2018](https://pmc.ncbi.nlm.nih.gov/articles/PMC6251936/table/tbl2) [DATED]). Feed benchmarks: EU 20/5 ppb, FDA 20 ppb | **Design for ≤10 ppb finished feed [ESTIMATE].** Test every lot of maize, cake, groundnut and fishmeal with rapid tests (ELISA or lateral flow) and confirm monthly by HPLC at an accredited lab. Use toxin binder in the premix |
| Edible oil fortification | Vegetable fats and oils must be fortified with vitamin A per KS 326-2 (as cited in the regulation). KEBS has threatened non-renewal of licences for non-fortifiers | [FAOLEX](https://faolex.fao.org/docs/pdf/ken115324.pdf); [The Star 2019](https://www.the-star.co.ke/business/2019-08-27-kebs-cs-munya-differ-on-edible-oil-release/) [DATED] |
| Edible oil product standard | Codex CXS 210 (named vegetable oils) applies where no Kenyan specification exists. A specific KS/EAS sunflower-oil standard number (possibly EAS 299) **was not verified** | FAOLEX (Codex fallback) |
| Product certification | KEBS Standardization Mark (permit to use the S-mark) for each product: refined oil, fish feed, and cake if bagged and sold as feed [ESTIMATE; verify scope] | — |
| Crop regulator | AFA (Nuts and Oil Crops Directorate) registration of the oilseed processor and buyer [ESTIMATE; verify under the Crops Act 2013] | — |
| Environment and safety | NEMA EIA licence (refinery effluent, boiler emissions; solvent plant in Phase 2 needs a full study); DOSHS workplace registration and statutory boiler and pressure-vessel examinations; county fire certificate; Water Resources Authority borehole permit; hexane hazardous-area classification in Phase 2 | [ESTIMATE; standard Kenyan permits] |
| Voluntary or customer-driven | FSSC 22000 / ISO 22000 for supermarket oil listings; HACCP; halal certification for oil; ASC Feed Standard if supplying ASC-certified farms | [ESTIMATE] |
| **QC lab (USD 0.15m)** | Moisture analyser, NIR (protein, fat, fibre, moisture), Kjeldahl or Dumas, Soxhlet, fibre, FFA/PV titration, Lovibond colour, aflatoxin rapid reader, water stability and floatability tests, pellet durability tester, microbiology basics | [ESTIMATE] |

---

## 8. Gaps and uncertainties

1. **Seed availability is the overriding unknown.** National sunflower output is 6 kt (FAOSTAT) vs 80 kt (Ministry) [CONFLICT]. Phase 1 alone needs 15 kt/yr. No county-level verified tonnage for 2025–26 was found, nor the status of Tanzanian seed export policy.
2. **No reliable turnkey capex quotes.** All equipment prices are marketplace listings (USD 30k–160k for "refineries", USD 10k–78k for "extrusion lines"). Real comparators are full-scope (Mainland USD 28m, De Heus USD 25m). The capex base is a bottom-up [ESTIMATE] with ±40% accuracy. **Action:** obtain 3 written quotes each for oil (e.g. Henan/Zhengzhou, Goyum/Indian, Farmet/Desmet) and extrusion (Famsun, Muyang-class, Andritz/Bühler) with defined scope, CIF Mombasa.
3. **Electricity cost.** I found no 2026 official CI1/CI2 schedule. The base of KES 20/kWh is derived from the 2023 schedule plus 2026 pass-throughs. The Nation figure of KES 13.44 conflicts. A >30% rise is a stated Kenya Power risk. Grid reliability in western Kenya was not quantified.
4. **KS 2289-1 contents** (aflatoxin, fibre, moisture and pellet specifications) were not retrieved. The KEBS edible-oil standard number was not verified. It is unclear whether KEBS certification of fish feed is mandatory.
5. **Victory Farms Doho mill capacity** is undisclosed. If it sells surplus feed (SamakGro already retails), it is a direct low-cost competitor in exactly the target geography. Tunga's 45 kt expansion and De Heus's 100 kt Njeru plant add regional capacity. The merchant aquafeed market may be only 20–40 kt (market_demand.md), so even 10 kt/yr is a 25–50% share target.
6. **Process yields** (oil content of Kenyan seed, residual oil, refining loss) come from international or older literature [DATED]. Run a pilot pressing of 20–50 t of local seed through a toll crusher, with lab analysis, before FID.
7. **Formulation.** Sunflower-cake inclusion above ~15–20% in extruded tilapia feed under East African conditions is not well documented. Fibre (~8%) is high. Needs feeding trials (e.g. KMFRI) and a nutritionist.
8. **Biomass fuel price and supply.** No 2026 Kenyan firewood or briquette price was found (KES 5–14/kg assumed). Hull fuel only becomes available with dehulling (Phase 2).
9. **Land prices** for industrial land in Kisumu, Bungoma and Eldoret: no 2025–26 data. Whether any SEZ near Kisumu exists or is planned was not established.
10. **Fiscal items to verify:** IDF/RDL rates, VAT on machinery and feed inputs, duty remission on imported seed/SBM/premix, and current SEZ CIT rates (Finance Act 2026).
11. **No Kenyan comparables found** for Menengai, Sigma Feeds or Pwani crushing capex, or for Agventure plant capacity.
12. **GMO court outcome** (judgment scheduled for Apr 2026) was not found. It determines whether imported GM SBM undercuts own soy cake.
