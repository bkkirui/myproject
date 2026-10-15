# G1 economics v2: Borut, Bomet (2,270 poultry, 70 livestock, 23 acres, 12 t lorry)

Prepared 2026-10-15. Model: `G1-model.xlsx` (live formulas; v1 kept as `G1-model-v1.xlsx`; recalculated in LibreOffice, 0 errors). Inputs are tagged **SOURCED**, **BENCHMARK**, **ASSUMED** or **OWNER-REPORTED**. Of 284 input rows, 8 are SOURCED, 40 BENCHMARK, 19 OWNER-REPORTED and 217 ASSUMED (about 50 of those are zero placeholders for unused egg parameters on non-chicken species). This is a benchmark screen, not a forecast and not advice. No farm accounts exist.

## 1. Answer first

**On benchmark prices the farm loses money, and the lorry makes it much worse.** Base OMBM is **-KES 1.53M** (-32% of revenue); without the lorry it is -0.58M. The B12 outcome is **no viable option** for owner-operation as designed (ranking B). If a lawyer confirms lease and sale are executable (ranking A), the top option is **sale as a conditional exit**, with lease second. Only the stacked High case (every input favourable at once) makes owner-operation pass. I did not tune any assumption to change this.

## 2. What changed vs v1, and why

| Item | v1 | v2 | Effect |
|---|---|---|---|
| Poultry | ~1,000, split guessed | **2,270**: 4 x 500 chicken breeds, 100 ducks, 50 geese, 20 turkeys, 100 guinea fowl | Revenue up; labour need up |
| Correction | | The brief said 2,770; 2,000 + 270 = **2,270**. INTAKE.md now says 2,270. No 2,770 figure is in the model | |
| Land | 12 acres guessed, rates 6k | 23 acres (owner), rent and rates **nil** | Land is opportunity cost only (L = KES 11.5M at assumed 500k/acre) |
| Labour | 18k + 11.5k + 10.5k | 3 x 22,000 (owner), +7.5% statutory +NITA +casuals | 868k vs 533k |
| Vet | per-head drugs only | + weekly visit fee (52 x 3,000, ASSUMED) | +156k |
| Structures | 800k | 2.0M (owner), 10-year life | Depreciation 200k |
| Lorry | none | cost-of-ownership sheet | -949k a year |
| Stores | none | 6 months feed and drugs on hand (owner) | Cash sheet: no feed purchases for months 1-6 |
| Owner | distance unknown | >300 km: 16 h per visit, 8k cash per visit | 556 h/yr, 10.7 h/week |
| Chick cost | 170 | 120 (sourced band 90-140) | Slightly favourable |

The four chicken breeds carry **identical** parameters: I found no breed-specific price, laying or growth data. Bird age and stage are unstated, so I assumed 40% of each flock is laying hens. The Mix table below tests that.

## 3. Base / low / high

| KES | Low | **Base** | High | v1 base |
|---|---|---|---|---|
| Revenue | 3.25M | **4.85M** | 7.00M | 2.78M |
| Gross margin | -1.76M | **0.82M** | 3.59M | 0.53M |
| Hired labour | 0.91M | **0.87M** | 0.87M | 0.53M |
| Weekly vet fees | 0.21M | **0.16M** | 0.10M | |
| Lorry net cost (with depreciation) | 1.38M | **0.95M** | 0.69M | |
| **OMBM** | -4.68M | **-1.53M** | +1.59M | -0.23M |
| OMBM without lorry | -3.30M | **-0.58M** | +2.28M | |
| Cash margin after controls, stipend, owner travel | -4.56M | **-1.35M** | +1.76M | |

Purchased feed is 58% of base revenue. Low stacks every adverse input, so it bounds the answer and does not predict it.

## 4. Per-enterprise margins (base, KES per year)

| Enterprise | Revenue | Gross margin | Margin/task hour |
|---|---|---|---|
| Cattle (4 cows in milk assumed) | 445k | 108k | 84 |
| Sheep | 228k | 119k | 218 |
| Goats | 62k | 40k | 219 |
| Sasso, Kuroiler, Rainbow, Kebro (each) | 897k | 86k | 118 (all four) |
| Ducks / geese / turkeys / guinea fowl | 176k / 123k / 89k / 144k | 46k / 66k / 36k / 60k | 526 (all four) |

Poultry is 85% of revenue (eggs 1.75M, live birds 2.37M) but earns only 552k, a 13% margin. A hen slot earns about 243 a year, a grower slot about 125. These are tag-ASSUMED yields at BENCHMARK prices (egg 15 KES farm gate, bird 750); small changes swing them widely.

## 5. Is KES 22,000 x 3 affordable?

| | Low | Base | High |
|---|---|---|---|
| FTE required | 3.30 | 2.72 | 2.32 |
| Utilisation of 3 staff | 110% | 91% | 77% |
| Labour as % of revenue | 28% | 18% | 12% |
| Gross margin / (labour + fixed costs) | -0.60x | 0.35x | 1.80x |

**Scale justifies three staff** (about 757 birds each plus livestock, driven by my 0.4 h per 100 birds per day assumption, to be measured). **The margin does not pay for them**: base labour is 106% of gross margin, and gross margin covers only 35% of labour plus fixed costs. Pay at which B12 value reaches zero is negative: wage cuts alone cannot close the gap. All-in cost is KES 23.7k per person per month, 2.4 times the stockman minimum (9,236). One worker is a relative: contract, task card and time log must be the same as for the others.

**Egg-meat mix (four chicken breeds, base gross margin):**

| Hens in flock | 0% | 20% | **40%** | 60% | 80% | 100% |
|---|---|---|---|---|---|---|
| Chicken margin, KES | 250k | 298k | **345k** | 392k | 439k | 486k |
| Egg trays per day | 0 | 5.3 | 10.6 | 15.9 | 21.3 | 26.6 |
| Growers sold per week | 68 | 54 | 41 | 27 | 14 | 0 |

More hens help only modestly (about +47k per 20 points) and need a buyer for up to 27 trays a day. In the Low case more hens makes it worse (feed). **No mix closes the gap**; the implied structure is a laying core of 30-50% with a steady weekly grower sale, once buyers are confirmed.

## 6. The lorry

| KES per year (base) | |
|---|---|
| Depreciation (4.5M value ASSUMED, 25% residual, 10 years) | 338k |
| Insurance 4%, fixed maintenance 2%, NTSA inspection, licences and tracker | 305k |
| **Standing cost, even if parked** | **642k** |
| Own-farm running: 4,000 km (fuel 197k, tyres and repairs 56k), 52 ad hoc driver days 78k | 331k |
| Credit for transport it replaces | -24k |
| **Net cost** (low 1.38M, high 0.69M) | **949k** (cash only: 612k) |

It accounts for **62% of the base OMBM loss**. A 12 t lorry is oversized for eggs, birds and small stock. **Hire income is zero in every headline case** because I found no source for demand or rates. To cover itself at an *illustrative* 25,000 gross per hire day (13,000 net after fuel, driver and tyres), it needs **73 hire days a year** (47 on cash costs only), about 29% of a working year, with a driver, owner >300 km away and fuel-theft risk. Evidence points only: local cargo minimum Sh225/km (Business Daily 2023); a 13 t tangerine load Sh110,000 per trip (Nation, undated). **Selling it improves the owner-operator value by KES 1.21M a year** (base; proceeds about 4.28M at the 2% declared return). Keep it only on written hire quotes and a named customer. If kept: GPS tracker, logbook, fuel receipts and a licensed driver, as it is the easiest asset to bleed.

## 7. Capital and working capital

| KES (base) | |
|---|---|
| Land 23 acres (opportunity cost) | 11.5M (53%) |
| Structures | 2.0M |
| Animals (poultry 1.23M, cattle 0.60M, sheep 0.30M, goats 0.07M) | 2.20M |
| Lorry | 4.50M |
| Feed and drug stores on hand | 1.58M |
| **Total** | **21.8M** (excluding land 10.3M; excluding land and lorry 5.8M) |

**KES 2m cannot be total capital**: animals alone are 2.2M, and land is far more. I treat it as structures only; please confirm. OMBM is -15% of capital excluding land.

**Cash (18 months, owner-operator, opening cash assumed 0):** months 1-6 run on stores and generate about +150k a month, reaching +0.9M. From month 7 feed and drug purchases (about 263k a month) resume and the base flow turns to **-113k a month (-1.35M a year)**, falling to -0.45M by month 18 and still declining. Low case: peak funding need **4.8M**. High: none. Treat the first six months as the owner's own inventory running down, not profit. Restocking six months of stores costs about 1.6M.

## 8. Revised B12 (convention: real terms; no land rent or rates; land earns lease rent or sale return plus g x L; stress on cash basis)

| Option, annual value KES | Low | **Base** | High |
|---|---|---|---|
| Self-run, PLAN generic | -7.18M | -3.72M | -0.24M |
| Owner-operator, lorry kept | -6.15M | **-2.38M** | +1.20M |
| Owner-operator, lorry sold | -4.46M | -1.16M | +2.11M |
| Lease (23 acres x 8,000, plus stock and lorry proceeds) | 0.10M | 0.27M | 0.53M |
| Sale (net of 5%, 2% real) | 0.32M | 0.38M | 0.47M |

- **Stress limit** is -10% of K = **-1.06M**. Owner-operator base worst case is -2.36M: **fails**. High passes (+0.36M). On the stricter v1 basis (depreciation not added back) base is -2.90M, also a fail.
- **Ranking A** (lease and sale available): sale first in Low and Base, owner-operator without lorry first in High. Lease beats sale only if real land growth exceeds about **2.0% a year** (base flip point).
- **Ranking B** (`title_ok` = 0; title deed, freehold status and any Land Control Board consent not seen): **no viable option; do not proceed as designed** in Low and Base. Only High returns "proceed".
- **Outcome: no viable option as an owner-operator; conditional exit (sale or lease) if title permits.** Sale and lease values scale with land at an **unsourced 500k/acre** (range 350-700k): get a valuer.
- The controls are affordable (3.9% of revenue, under the 7% cap) but fail the one-third-of-OMBM test while OMBM is negative.

## 9. Break-even (base)

| Lever, alone | Needed | Now |
|---|---|---|
| OMBM for B12 value = 0 | 0.85M | -1.53M |
| Egg farm-gate price | 36 KES (1,082 per tray) | 15 (450) |
| Live-bird price | 1,556 | 761 |
| Purchased feed price cut | 84% | 0 |
| Poultry scale (margin per bird constant) | 5.3 times | 1 |
| Revenue at constant ratios | 3.9 times | 1 |

No single lever is credible. **Stacked, cumulative owner-operator value:**

| Step | Value, KES |
|---|---|
| Start | -2.38M |
| + sell the lorry | -1.16M |
| + feed 20% cheaper (own fodder on 23 acres, bulk buying) | -0.60M |
| + two staff plus extra casuals for the hours gap | -0.41M |
| + egg and bird prices both 10% higher | -0.01M |
| + drop supervisor stipend, halve owner visits | +0.13M |

Even all five together only reach roughly break-even (about 130k, with no margin for the stress limit). Egg +3 KES and bird +150 together still leave -1.59M with the lorry kept. Feed price moves value by about 282k per 10%.

## 10. Ambiguities to resolve

- Is KES 2m structures only (my reading) or total capital? Lorry value, year and make; is 12 t GVW or payload?
- Poultry age and stage per house, and which birds lay. Hen share drives the mix.
- Water pans "about 8m litres": 8 million litres or 8 m3? Strong water security is accepted but not valued.
- Title deed copy; who counted animals; vaccines given; vault cash and key-holders; lorry licences and driver.
- Is the weekly vet fee already inside my per-head drug costs? Possible partial double count.
- Which worker is the relative, and what the role is.

## 11. First 8 weeks of data (`Collect_8wk` sheet, 19 items)

| Week | Collect | Replaces |
|---|---|---|
| 1 | Independent count by breed and age; title copy and search; lorry file (logbook, price, insurance, driver, tracker); vault count and key log | counts, hen share, title, lorry inputs, opening cash |
| 2 | Acreage by use; pan volumes; staff contracts and time use | acres, forage, hours |
| 4 | Feed receipts, three quotes, physical store count against the 6-month claim; staff time log | feed price, labour hours per 100 birds |
| 6 | Vet invoice and fee; three written 12 t hire quotes and named customers; lease and sale indications | vet fee, hire days and rate, rent, land value |
| daily, to 8 | Eggs by breed, feed bags, deaths; every sale with price and buyer; milk | eggs/hen, hen feed, prices, mortality |
| 8 | Owner hours and trip costs; rerun model | owner time |

**Week-8 rule:** annualised OMBM with the lorry should be at least about KES 0.85M to continue, or about 0.58M without it. If measured OMBM is near or below zero, sell the lorry first, then cut feed cost and consider two staff plus casuals; if still short at week 16 and title is clear, compare lease and sale with a valuer. Set a cumulative loss limit at sign-off; base burn after stores run out is about 113k a month.

## Sources (accessed 2026-10-15; search summaries only, pages could not be fetched in this session, so none is verified against the original)

- Day-old chicks KES 90-140; Kenbro ~115, Kenchic broiler ~105: https://www.beyondforest.org/post/day-old-chicks-prices-in-kenya-2025-update-kenchic-kienyeji-broiler-prices-near-nairobi (2025 update). BENCHMARK.
- Mature kienyeji KES 900-1,500 retail; dressed 600-1,200: https://www.beyondforest.org/post/kienyeji-chicken-prices-in-kenya-2026-cost-per-kg-breeds-farming-guide-and-profitability (2026). BENCHMARK; no Sasso/Kuroiler/Rainbow/Kebro price found.
- Eggs: farm gate ~400 per tray; retail 504-720 (Nation, ~Jul 2026): https://nation.africa/kenya/business/egg-prices-rise-as-milk-maize-shortages-persist-5583908 ; indigenous 540-750: https://www.businessdailyafrica.com/bd/markets/commodities/eggs-prices-ease-but-cost-of-feeds-big-headache-to-farmers-4814490 . BENCHMARK.
- Feed: layers mash 3,900-4,000 (late 2025, as v1); Sh4,500 and chick mash 4,940 in Feb 2023: https://www.the-star.co.ke/news/star-farmer/2023-02-03-costly-animal-feed-pushes-egg-prices-to-record-high . No 2026 bag price found. BENCHMARK.
- Duck, goose, turkey, guinea fowl (undated asking, breeder and ornamental prices): https://jiji.co.ke/74-turkeys/local ; https://www.standardmedia.co.ke/farmkenya/article/2001342677/how-to-rear-domestic-guinea-fowls ; https://nation.africa/kenya/business/seeds-of-gold/beyond-the-beauty-of-ornamental-birds-lies-a-lucrative-business-1213296 ; https://mwananchi.co.tz/kenya/business/seeds-of-gold/you-can-t-afford-guinea-fowls-why-not-hatch-their-eggs-234496 . BENCHMARK/ASSUMED after haircut.
- Land: no Bomet price found. Low-authority blog: https://graduatefarmer.co.ke/2025/05/14/how-to-get-rich-through-farming-in-kenya-a-2025-guide-to-avocado-and-coffee-profits/ (150k remote to 800k+; lease 10-30k per acre). ASSUMED 500k/acre.
- Diesel Nairobi 217.86 per litre, 15 Sep-14 Oct 2026 (EPRA via https://www.kenyans.co.ke/news/127048-epra-retains-fuel-prices-september-october-cycle ). BENCHMARK; Borut uplift assumed.
- NTSA inspection, heavy commercial over 5 t, Sh4,600 (date unclear): https://www.kenyanews.go.ke/?p=1101 ; draft 3,500: https://www.kenyans.co.ke/news/77117-ntsa-unveils-proposed-vehicle-inspection-fees-new-rules-take-effect-list . BENCHMARK.
- Truck fuel use 3-7 km/L: https://www.carimports.co.ke/reviews/2019-isuzu-forward-review-prices-specs/ . Driver pay 22,469-61,097 per month: https://wageindicator.org/en-ke/work-in-kenya/jobs-and-salaries/kenya-heavy-truck-and-lorry-drivers . Freight Sh225/km: https://www.businessdailyafrica.com/bd/corporate/shipping-logistics/truckers-to-downsize-hike-charges-on-taxes-4283514 . Lorry price, insurance premium and hire rates: **none found; ASSUMED.**
- Unchanged from v1: FX, minimum wages, NSSF, milk, small-stock prices (see `G1-economics.md` sources).
