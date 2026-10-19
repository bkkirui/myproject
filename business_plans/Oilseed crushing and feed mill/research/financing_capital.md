# Financing and capital structure: oilseed crushing + aquafeed mill (Kenya)

Research date: 19 Oct 2026. Workstream: project finance, cost of capital, financing plan by phase, valuation and exit.

**Read this first: evidence base and its limits.**
- **Searches.** Only **one** web search was possible this session (on Agventure/AgDevCo). After that the shared web-search budget for the workflow was used up. The only direct fetch tried (the AgDevCo PDF) failed with a DNS error.
- **Where the figures come from.** Most sourced figures here are carried over from earlier cited notes, chiefly the screening-study research notes and the sibling files `feedstock_supply.md`, `market_demand.md` and `technical_operations.md`. Their URLs are given inline, but **they were not re-verified this session**.
- **Labels used:**
  - **[PK-UNVERIFIED]** is the analyst's prior knowledge of how an institution or market works. No source was retrieved this session, so check it before relying on it. No numbers are presented as sourced under this label.
  - **[ESTIMATE]** is the analyst's own figure, with the reasoning given.
  - **[DATED]** means the source is older than 2025.
  - **[CONFLICT]** means sources disagree.
- **What this means for the model.** Term-sheet numbers below are **structuring assumptions for the model**, not quotes. The Phase 0 action list (§9) says how to replace them with indicative terms.

Inputs from sibling files used throughout:
- **Phase 1:** capex USD 9.5m (6.5–14) and working capital USD 3.0m (2–4.5). Scope is a 50 tpd full-press crush, 20 t/d refinery, 3 t/h extrusion and 5 kt silos ([technical_operations.md](technical_operations.md)).
- **Phase 2:** incremental capex USD 22m (15–32) and working capital +5–7m. Scope is 150 tpd prepress plus solvent extraction ([technical_operations.md](technical_operations.md)).
- **Steady-state seasonal working-capital peak:** KES 650–950m (USD 5–7m) ([feedstock_supply.md](feedstock_supply.md)).
- **Seed supply:** a crusher above ~20 kt/yr of seed "is not supportable before year 5" ([feedstock_supply.md](feedstock_supply.md)).

---

## 0. Key assumptions for the model

| # | Parameter | Low | Base | High | Unit | Source / basis |
|---|---|---|---|---|---|---|
| 1 | KES/USD spot at model start | 129.4 | 129.8 | 130.0 | KES/USD | 129.81 on 15 Oct 2026 ([Kenya Times](https://thekenyatimes.com/business/kenyan-shilling-holds-firm-as-forex-reserves-drop-by-221million/)) |
| 2 | KES depreciation vs USD, 2027–2035 | 2.0 | 4.0 | 7.0 | %/yr | [ESTIMATE]: inflation differential (KES CPI 6.8% vs US ~2.5–3%) plus election-year stress in 2027. See prior notes ([macro](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_macro_investment_climate.md)) |
| 3 | CBR (reference rate for KES loans) | 8.25 | 8.75 | 10.0 | % | Held at 8.75% on 7 Oct 2026 ([CBK](https://www.centralbank.go.ke/2026/10/07/mpc-retains-the-cbr-at-8-75-percent-3/)) |
| 4 | Average bank lending rate (market) | 14.0 | 14.4 | 15.5 | % | 14.4% in Sep 2026 ([Capital FM](https://capitalfm.africa/private-sector-credit-growth-accelerates-to-10-6pc-in-september/)) |
| 5 | Senior KES term loan, all-in rate (greenfield borrower) | 14.0 | 15.5 | 17.5 | % nominal | [ESTIMATE]: market average 14.4% plus 1–3 pp greenfield and single-asset premium. Risk-based pricing is CBR + margin [PK-UNVERIFIED] |
| 6 | Senior term tenor / grace | 5 / 12 | 7 / 18 | 8 / 24 | yrs / months | [ESTIMATE]: typical Kenyan bank project/asset loan. Grace covers 12–20 months of construction plus ramp-up |
| 7 | USD base rate (SOFR, 2027–30 average) | 3.25 | 4.0 | 5.0 | % | [ESTIMATE]: the US 10-year was 5.24% on 9 Oct 2026 and the Fed was hiking ([ETF Trends](https://www.etftrends.com/fixed-income-content-hub/treasury-yields-snapshot-october-9-2026/)). SOFR itself was not retrieved |
| 8 | DFI senior USD margin over SOFR | 4.5 | 6.0 | 7.5 | pp | [ESTIMATE]: Kenya USD sovereign yields of 8.5–9.9% (2034–39) ([People Daily](https://peopledaily.digital/business/cbk-kenya-eurobond-yields-rise-as-bond-market-faces-fresh-pressure)) plus a corporate/greenfield spread. All-in ≈ 9.5–11% USD |
| 9 | Mezzanine (AgDevCo-type), all-in USD cost | 11 | 13 | 16 | % USD | [ESTIMATE]: AgDevCo uses mezzanine in Kenyan oilseed and aquaculture deals (§2) but terms are undisclosed. Assumes cash coupon plus a royalty or equity kicker |
| 10 | Mezzanine tenor / grace | 6 / 24 | 8 / 36 | 10 / 48 | yrs / months | [ESTIMATE] |
| 11 | Seasonal working-capital line rate | 13.0 | 14.5 | 16.0 | % KES | [ESTIMATE]: market rate ±. Secured on stock and receivables |
| 12 | WC borrowing base, stock (collateral-managed or WRS) | 50 | 65 | 75 | % of stock value | [ESTIMATE] / [PK-UNVERIFIED] typical inventory-finance advance rates |
| 13 | Upfront / arrangement fees (all debt) | 1.0 | 1.5 | 2.5 | % of facility | [ESTIMATE]; DFIs also charge DD and legal costs, often USD 75–200k |
| 14 | Min. DSCR covenant (lock-up) / default | 1.20 / 1.05 | 1.30 / 1.10 | 1.40 / 1.20 | x | [ESTIMATE]: standard project-finance range |
| 15 | Max net debt / EBITDA (after year 3) | 2.5 | 3.0 | 3.5 | x | [ESTIMATE] |
| 16 | Debt-service reserve account (DSRA) | 3 | 6 | 6 | months of debt service | [ESTIMATE] |
| 17 | Phase 1 long-term funding need (capex + pre-op + fees + IDC + DSRA + permanent WC) | 9.5 | 12.4 | 18.0 | USD m | Built in §6 from sibling capex (6.5 / 9.5 / 14) |
| 18 | Phase 1 equity share (incl. grants) | 40 | 50 | 60 | % of long-term funding | [ESTIMATE]: greenfield, first-time operator, no offtake history. Lenders/DFIs will not go above ~50–60% debt |
| 19 | Cost-overrun standby equity | 10 | 15 | 20 | % of capex | [ESTIMATE]: standard lender requirement |
| 20 | Phase 2 funding need | 22 | 30 | 41 | USD m | Sibling capex 15 / 22 / 32 + WC 5–7 + fees, IDC and DSRA |
| 21 | Phase 2 debt share | 45 | 55 | 60 | % | [ESTIMATE]: with an operating record and DFI senior debt |
| 22 | Grants / TA realistically obtainable | 0 | 0.3 | 1.0 | USD m | [ESTIMATE]: AECF/IFAD/foundation programmes (§4). **Do not let the base case depend on grants** |
| 23 | Founder equity hurdle, Phase 1 (survival-weighted) | 30 | 35 | 40 | % KES IRR | Screening report hurdle for greenfield ([macro notes §2](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_macro_investment_climate.md)) |
| 24 | Equity return expected by PE/DFI fund investor (Phase 2) | 18 | 22 | 25 | % USD gross IRR | [PK-UNVERIFIED]: typical African PE target. ≈ 23–30% KES-equivalent at a 4% drift |
| 25 | WACC, Phase 1 (nominal KES, post-tax) | 19 | 23 | 27 | % | §5 calculation [ESTIMATE] |
| 26 | WACC, steady state after Phase 2 (nominal KES, post-tax) | 14 | 16.5 | 19 | % | §5 calculation [ESTIMATE] |
| 27 | Exit EV/EBITDA (trade sale, year 7–10) | 4.0 | 5.0 | 7.0 | x | [ESTIMATE]. Anchors: KPC IPO 8.1x ([african-markets](https://www.african-markets.com/en/stock-markets/nse/kenya-pipeline-company-ipo-subscribed-at-105-7-listing-on-the-nairobi-securities-exchange-scheduled-for-march-10)); US LMM PE 5.5–6.4x ([Capitalpad](https://capitalpad.com/lower-middle-market-ebitda-multiples/)). See §8 |
| 28 | Corporate income tax | 30 | 30 | 30 | % | ([Chambers 2026](https://practiceguides.chambers.com/practice-guides/corporate-tax-2026/kenya)) |
| 29 | Tax-loss carry-forward limit | 5 | 5 | 5 | years | Finance Act 2025 ([KPMG](https://kpmg.com/us/en/taxnewsflash/news/2025/07/kenya-tax-changes-finance-act-2025.html)) |
| 30 | Interest deductibility cap | 30 | 30 | none | % of EBITDA | [PK-UNVERIFIED]: interest-restriction rule from Finance Act 2021. Verify |
| 31 | WHT on interest paid to non-resident lenders | 0 | 15 | 15 | % | [PK-UNVERIFIED]: DFI loans usually require gross-up. Some DFIs may be exempt by treaty or agreement. Verify |
| 32 | Outgrower input credit loss rate | 5 | 10 | 15 | % of credit | [ESTIMATE] from [feedstock_supply.md](feedstock_supply.md) |

---

## 1. Cost of capital: KES and USD

**Market anchors, Oct 2026 (sourced in prior notes):**

| Instrument | Yield / rate | Source |
|---|---|---|
| CBR | 8.75% (held 7 Oct 2026) | [CBK](https://www.centralbank.go.ke/2026/10/07/mpc-retains-the-cbr-at-8-75-percent-3/) |
| 91 / 182 / 364-day T-bill | 8.75 / 8.86 / 9.04% (15 Oct 2026) | [Serrari](https://serrarigroup.com/kenya-91-day-treasury-bill-draws-ksh-49-8bn-in-bids/) |
| Tax-free infrastructure bonds (Aug 2026 reopening) | 11.75–12.74% coupons | [Serrari](https://serrarigroup.com/cbk-opens-ksh150bn-tax-free-infrastructure-bond-sale/) |
| Average commercial-bank lending rate | 14.4% (Sep 2026); NPL ratio 13.9% | [Capital FM](https://capitalfm.africa/private-sector-credit-growth-accelerates-to-10-6pc-in-september/); [Business.co.ke](https://business.co.ke/private-sector-credit-growth-hits-10-6-as-npls-fall-to-13-9/) |
| Kenya USD Eurobonds | 6.26% (2027) to 9.89% (2039) on 16 Oct 2026 | [People Daily](https://peopledaily.digital/business/cbk-kenya-eurobond-yields-rise-as-bond-market-faces-fresh-pressure) |
| US 10-year Treasury | 5.24% (9 Oct 2026) | [ETF Trends](https://www.etftrends.com/fixed-income-content-hub/treasury-yields-snapshot-october-9-2026/) |
| Inflation | 6.8% y/y (Sep 2026) | [KNBS](https://www.knbs.or.ke/wp-content/uploads/2026/09/Kenya-Consumer-Price-Indices-and-Inflation-Rates-September-2026.pdf) |

**Debt pricing for this project [ESTIMATE]:**
- **KES senior, Kenyan bank, greenfield single-asset borrower: 14–17.5%, base 15.5%.**
  - The market average of 14.4% includes prime corporates.
  - A new SPV with no trading history pays 1–3 pp more, and usually gives a founder guarantee as well.
  - Real cost is about 8.7% (15.5% less 6.8% CPI). That is expensive debt in real terms.
- **USD senior from a DFI: about 9.5–11% all-in** (SOFR ~4% + 5.5–7%).
  - In KES terms that is (1.10 × 1.04) − 1 ≈ **14.4% at a 4% depreciation path, roughly the same as KES bank debt**.
  - USD debt also carries the depreciation tail: a 2015- or 2023-style 20–25% KES move [PK-UNVERIFIED for the magnitude] would add about 20% to the KES value of principal.
- **Partial natural hedge (judgement).**
  - Oil revenue is priced off import parity: CPO about USD 1,430/t landed, crude sunflower oil about USD 1,610/t ([market_demand.md](market_demand.md)). Cake is priced off soybean-meal and sunflower-meal parity.
  - Seed is also bought at prices that follow oil and cake parity, especially with the floating, import-parity-linked contract recommended in [feedstock_supply.md](feedstock_supply.md).
  - The crush **margin** is therefore largely USD-indexed: a weaker KES raises KES revenue and KES seed cost together.
  - Implication: **USD debt can be up to ~40–50% of total debt** without a large structural mismatch. KES-denominated working-capital debt is still the right match for seasonal stock financing.
- **Local-currency DFI lending** [PK-UNVERIFIED]. Several DFIs (FMO, AgDevCo, BII) can lend in KES, typically by hedging through TCX (The Currency Exchange Fund) or by on-lending through Kenyan banks. Pricing is usually close to the KES government curve plus a credit margin, i.e. around 13–16%. It removes FX risk at little or no saving over bank KES debt, but the tenors are longer (7–10 years). **Ask every DFI approached for a KES option.**

**Equity cost:**
- **Founder hurdle.** The screening report sets 35–40% expected KES IRR survival-weighted for greenfield, or ~45–50% conditional on survival, and 25–30% for established businesses.
- **Why the hurdle is that high.** Passive alternatives are a 12–12.7% tax-free infrastructure bond and NSE expected returns of about 13–15% ([macro notes §2](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_macro_investment_climate.md)).
- **Outside equity** [PK-UNVERIFIED]:
  - African PE funds typically target 20–25% gross USD IRR, about 3x money.
  - DFIs investing directly accept roughly 12–18% USD on equity-like instruments when development impact is high.
  - AgDevCo-type impact investors accept lower risk-adjusted returns on mezzanine in exchange for smallholder impact.
- **Judgement.**
  - Outside equity at Phase 2 (USD ~22% target) costs **less** than the founder's KES greenfield hurdle. Once the plant is de-risked, selling a minority to a fund at a step-up valuation is accretive.
  - Selling equity in Phase 1, before an operating record, is dilutive at a punitive valuation.

---

## 2. Who finances agro-processing in Kenya (2025–2026)

### 2.1 DFIs and specialist agri investors

| Institution | Instruments / ticket | Kenya agri / oilseed / aqua evidence | Fit for this project | Status / notes |
|---|---|---|---|---|
| **AgDevCo** (UK-backed specialist agri investor) | Senior debt, **mezzanine** and equity; typical ticket ~USD 2–20m [PK-UNVERIFIED] | **Agventure (Kenyan canola crusher, "Pure Mountain"): USD 9.5m mezzanine loan** to expand canola oil and seed processing and raise outgrower purchases ([AgDevCo PR, Nov 2024](https://www.agdevco.com/site/assets/files/2133/agventure_press_release_nov_2024.pdf) [DATED]; [Africa PE News](https://www.africaprivateequitynews.com/p/kenyas-agventure-raises-95m-from); [Food Business MEA](https://www.foodbusinessmea.com/agventure-secures-us9-5m-investment-from-agdevco-to-expand-canola-oil-and-seed-processing/)). **Victory Farms: USD 4m (2021) plus a USD 15m follow-on mezzanine (2026)** ([WeAreAquaculture](https://weareaquaculture.com/news/finance/tilapia-producer-victory-group-secures-15m-follow-on-investment-from-agdevco)). Raised USD 85m from BII, Swedfund and Norfund ([Food Business MEA](https://www.foodbusinessmea.com/agdevco-raises-us85m-from-bii-swedfund-and-norfund-to-support-african-agribusiness/), date not confirmed) | **Best single fit for Phase 1**: it has done both an oilseed crusher and an aquaculture deal in Kenya, offers mezzanine, and runs a smallholder TA unit [PK-UNVERIFIED] | Loan terms are **not disclosed** in any result found. [CONFLICT]: Agrifocus reports the Agventure deal on 9 Apr 2026 ([Agrifocus](https://agrifocusafrica.com/2026/04/09/agdevco-invests-9-5-million-in-kenyas-agventure-to-advance-regenerative-agriculture/)) against the Nov 2024 press release, so it is either late re-reporting or a second tranche. Note: the prior notes cited foodbusinessmea `?p=2133850` for Agventure, but per the search title that URL is the AgDevCo USD 85m fundraise article |
| **BII** (UK) | Debt and equity, direct (usually ≥USD 10m) or via funds/banks [PK-UNVERIFIED] | Invested £1.07bn in Africa in 2025, with ≥25% of new investment going to frontier markets under the 2026–31 strategy ([Engineering News](https://www.engineeringnews.co.za/article/1bn-plus-invested-in-african-businesses-last-year-bii-2026-06-25)). BII–ILX USD 15m MSME/agribusiness loan to an East African FI, Mar 2026, with up to USD 500m of co-financing planned ([BII](https://www.bii.co.uk/en/news-insight/news/british-international-investment-and-ilx-complete-first-joint-investment/)). Agribusiness programme with FMO ([BII](https://www.bii.co.uk/en/news-insight/news/bii-and-fmo-join-forces-with-the-uk-government-to-boost-finance-for-agribusinesses/) [DATED 2024]) | Phase 1: **indirect** (BII-funded bank lines, AgDevCo). Phase 2: direct if the ticket is ≥USD 10m | Active |
| **IFC** | Loans/equity, minimum direct ticket about USD 5m (unverified); risk-sharing with banks | Risk-sharing: 4G Capital uses **IFC first-loss guarantees with Equity Bank and KCB** ([BusinessTech Africa](https://www.businesstechafrica.co.za/article/african-smes-are-finding-another-way-to-borrow-money)). IFC–FCDO agribusiness programme (DRC, 2026) ([IFC](https://www.ifc.org/en/pressroom/2026/united-kingdom-and-ifc-partner-to-expand-agribusiness-and-accelerate-job-creation-)). Kenya pipeline: Airtel, OrPower, Atlas ([Boardlot](https://www.boardlot.co.ke/p/beyond-the-headlines-how-the-ifc)) | Phase 2 senior/A-loan; Phase 1 only through bank risk-sharing | Active |
| **Proparco** (France) | Senior loans, ~USD 10m+ [PK-UNVERIFIED] | **Kenya Nut Company: USD 18.7m loan** ([Africa PE News](https://www.africaprivateequitynews.com/p/proparco-backs-kenya-nut-company-with-18-7m-loan); date not confirmed) | Phase 2 | Active in Kenyan agro-processing |
| **Norfund** (Norway) | Equity, mezzanine and loans; agribusiness is a core sector in East Africa [PK-UNVERIFIED] | Investor in AgDevCo (above) | Phase 2 equity or debt; Phase 1 indirectly via AgDevCo | No 2026 Kenya-specific deal retrieved |
| **FMO** (Netherlands) | Loans and equity, including local currency [PK-UNVERIFIED] | Committed to ARAF II, Jul 2026 ([Finta](https://finta.ai/blog/development-finance-institutions-backing-private-funds)) | Phase 2; KES option | No Kenya agro deal retrieved |
| **AfDB** | Lines of credit to banks; direct only for large deals | **USD 10m trade-finance line to Family Bank** for Kenyan SMEs, Oct 2026 ([fundsforNGOs](https://news.fundsforngos.org/2026/10/14/afdb-family-bank-10-million-trade-finance-line-kenya-smes-foreign-currency/)) | Indirect: FX trade finance for imported equipment and premix | Active |
| **US DFC** | Loans, portfolio guarantees (ex-USAID DCA) | 83% of USAID programmes were ended by Mar 2025 ([Pharmaceutical Technology](https://www.pharmaceutical-technology.com/?p=361037)) | **Do not plan on** USAID/DCA-type guarantees. DFC's 2026 Africa posture is unknown | **Gap**: not researched |
| **AATIF** (Africa Agriculture and Trade Investment Fund) | USD senior/mezz loans to agri corporates and FIs, ~USD 5–30m [PK-UNVERIFIED] | None retrieved | Phase 2 alternative | Unverified |
| **Triodos** (investment funds) | Mainly fund/FI investments [PK-UNVERIFIED] | None retrieved | Low fit | Unverified |

### 2.2 PE and impact funds (equity, mostly Phase 2)
- **Catalyst Principal Partners Fund II** (USD 155m) and **Novastar East Africa Fund I** (USD 80m) are local/regional funds ([Zoom Investors](https://zoominvestors.com/blog/private-equity-east-africa); secondary). Catalyst does mid-market control and significant-minority deals; Novastar leans to consumer and tech.
- **Helios IV** (USD 1.25bn target) is too large for this deal.
- **Phatisa** (food/agri PE across Africa), **Kuramo** and **Inside Capital** (smaller East African growth equity) are plausible names [PK-UNVERIFIED]. No 2025–26 fund sizes or Kenyan agro deals were retrieved.
- **Equity is scarce.** Kenyan startups raised ~USD 86m in Q3 2026, >92% of it debt ([Business Today](https://businesstoday.co.ke/african-ventures-raise-us-674million-in-q3/)). That suggests equity is scarce and expensive, which argues for **founder-funded Phase 1 equity and outside equity only after commissioning**.

### 2.3 Kenyan banks
- **Big five:** KCB, Equity, Stanbic, NCBA, Co-op.
- **Credit conditions:** private-sector credit grew 10.6% y/y in Sep 2026 and new lending hit a record KES 99.4bn that month, so banks are lending again. The NPL ratio is 13.9% ([Business Daily](https://www.businessdailyafrica.com/bd/markets/market-news/september-loans-signal-strong-private-sector-credit-growth-5629568); [Business.co.ke](https://business.co.ke/private-sector-credit-growth-hits-10-6-as-npls-fall-to-13-9/)).
- **Typical greenfield terms** [ESTIMATE / PK-UNVERIFIED]:
  - KES term loans of 5–7 years with 6–18 months grace.
  - Collateral cover of 125–150% (land title plus debenture over plant), a personal guarantee from the promoter, and an insurance assignment.
  - DSCR ≥1.25–1.3x.
  - A USD option at roughly SOFR + 5–7% for borrowers with USD-linked revenue.
- **Outgrower input finance with banks.** Bidco's sunflower and soy contract farming used **Equity Bank input loans** ([Business Daily](https://www.businessdailyafrica.com/bd/news/counties/bidco-set-to-buy-sh120m-sunflower-seeds-from-farmers-in-meru-2301152) [DATED]). This tripartite model (bank, farmer, processor) is the template for outgrower credit, and keeps it off the crusher's balance sheet except for any first-loss given.
- **Election-year caution.** Election years historically slow credit and capex decisions ([macro notes §4](../../../research_notes/Profitable%20business%20opportunities%202026/kenya_macro_investment_climate.md)). An FID in mid-2027 sits right in the Aug 2027 election window.

---

## 3. Blended finance and guarantees
- **IFC risk-sharing / first-loss with Kenyan banks** is in active use with Equity and KCB ([BusinessTech Africa](https://www.businesstechafrica.co.za/article/african-smes-are-finding-another-way-to-borrow-money)). Ask the lead bank whether an existing IFC or BII risk-sharing facility can cover the term loan. That can cut collateral requirements more than the rate.
- **Africa Guarantee Fund (AGF)** [PK-UNVERIFIED]: partial credit guarantees, typically ~50% (up to ~75%), on SME loans made by partner banks, for a guarantee fee of ~1–2% p.a. A Phase 1 senior loan of USD 4–5m is at the upper end of AGF's SME focus. Confirm its current Kenyan partner banks.
- **Kenya Credit Guarantee Scheme** (GoK, MSME-focused) [PK-UNVERIFIED]: ticket sizes are too small for this project.
- **USAID DCA / DFC guarantees.** USAID is largely dismantled (83% of programmes ended, Mar 2025) ([Pharmaceutical Technology](https://www.pharmaceutical-technology.com/?p=361037)). **Model with no US guarantee.** Treat DFC as upside, pending research.
- **Blended capital via AgDevCo.** AgDevCo's UK/Nordic-funded capital ([BII, Swedfund, Norfund](https://www.foodbusinessmea.com/agdevco-raises-us85m-from-bii-swedfund-and-norfund-to-support-african-agribusiness/)) is itself semi-concessional, patient mezzanine. In practice it is the most realistic "blended" layer for Phase 1.

## 4. Grants and technical assistance (budget conservatively)
- **AECF (Africa Enterprise Challenge Fund)** [PK-UNVERIFIED]: Nairobi-based. Competitive grants and repayable grants for agribusiness and renewables, typically ~USD 0.1–1.5m with matching required. It runs on calls, so timing is uncertain.
- **IFAD** [PK-UNVERIFIED]: operates through government programmes in Kenya. The Aquaculture Business Development Programme (ABDP) and cereal/oilseed value-chain projects are relevant. Its benefits flow to farmers (inputs, extension, cage clusters) rather than as cash to the processor. Use it to co-fund the outgrower programme. Check ABDP's 2026 status.
- **Mastercard Foundation (Young Africa Works Kenya)** [PK-UNVERIFIED]: funds partners for youth employment in agri value chains, and could fit outgrower or aqua-farmer programmes.
- **NGO aggregation partners.** Farm Africa runs soy aggregation centres with interest-free loans for ~6,000 Homa Bay farmers ([Standard, Jul 2026](https://www.standardmedia.co.ke/counties/article/2001553574/relief-to-6000-farmers-as-soya-bean-production-intensifies)), a ready-made partner for seed supply.
- **County and national programmes.** County sunflower drives exist (Kakamega, LBDA in Kisumu; see [feedstock_supply.md](feedstock_supply.md)). There is also the national edible oil crops push (EOCPP) and a KenInvest edible-oil opportunity listing for Homa Bay ([KenInvest](https://opportunities.invest.go.ke/opportunities/opportunity/edible-oil-production-1)).
- **Model treatment:** base USD 0.3m of grants, used only to co-fund the outgrower programme and ESIA/feasibility work. Grants never fund core capex in the base case.

---

## 5. Recommended capital structure and WACC

**Principles (judgement):**
1. **Size debt to DSCR at ramp-up, not to capex.**
   - Seed supply is the binding constraint. Phase 1 needs 15 kt/yr, which is 20–100% of reported national sunflower output, so utilisation in years 1–2 is likely only 40–60% [ESTIMATE].
   - Senior debt must therefore be serviceable from ramp-up EBITDA.
2. **Match currency to cash flow.**
   - Seasonal working capital is in KES.
   - Long-term debt is at most ~50% USD, because the margin is import-parity-linked.
   - If a DFI offers KES at a cost comparable to USD plus expected depreciation, prefer KES.
3. **Patient mezzanine instead of more senior debt** in Phase 1. A 3-year grace covers ramp-up.
4. **Outside equity at Phase 2**, priced on operating EBITDA. Use the founder's balance sheet for Phase 0–1.

**Illustrative WACC [ESTIMATE].** Nominal KES, post-tax. Debt is tax-deductible at 30%, subject to the interest-cap check.

| Layer | Phase 1 weight | Pre-tax cost (KES-equivalent) | Post-tax | Steady state (post-Phase 2) weight | Pre-tax | Post-tax |
|---|---|---|---|---|---|---|
| Equity | 50% | 35% (founder greenfield hurdle) | 35% | 40% | 25% (blended founder + fund) | 25% |
| Senior (KES bank / DFI) | 36% | 15.5% | 10.9% | 45% | 14.0% (DFI, longer tenor) | 9.8% |
| Mezzanine (USD 13% + 4% FX drift) | 14% | 17.5% | 12.3% | 5% | 17.5% | 12.3% |
| Seasonal WC (outside WACC; carried as an operating cost of funds) | — | 14.5% | 10.2% | — | 13.5% | 9.5% |
| **WACC** | | | **≈ 23%** | | | **≈ 15–16.5%** |

- **Use 23% (19–27%) to discount Phase 1 project cash flows.** If project IRR is below ~23% nominal KES, the founder's 35% equity hurdle can only be met through leverage at ramp risk.
- The steady-state WACC of ~16.5% is the right rate for a terminal-value cross-check.

---

## 6. Phased financing plan with term-sheet assumptions

### Phase 0: development (Q4 2026 to ~Q3 2027, 9–12 months). About USD 0.6–1.0m.

| Use | USD m | Source |
|---|---|---|
| Outgrower pilot (2,000–3,000 ha, seed-only credit), weigh-and-pay, agronomists | 0.25–0.4 | Founder equity; grant co-funding (AECF/foundation) if won |
| Feasibility, FEED/engineering, ESIA (NEMA), land option, permits | 0.2–0.35 | Founder equity |
| Offtake work: crude-oil LOIs with Bidco/Menengai/Kapa; cake and feed LOIs with Tunga/SamakGro/De Heus ([market_demand.md](market_demand.md)); DFI and bank DD costs | 0.1–0.25 | Founder equity |

- **Why start now.** DFI processes (screening, IC, DD, legal) take **6–12 months** [PK-UNVERIFIED]. Open AgDevCo and two banks in Phase 0 so that debt is committed at FID.
- **FID gates (conditions precedent):**
  - ≥8–10 kt/yr of seed under contract or with a credible import route.
  - Signed LOIs for ≥50% of crude oil or cake.
  - ESIA licence.
  - Committed debt.
- **FID timing.** Prefer FID after the Aug 2027 election result is settled (Q4 2027). The cost is about one quarter of delay.

### Phase 1: 50 tpd crush + refinery + 3 t/h extrusion. FID ~Q4 2027, COD ~Q1–Q2 2029.

**Uses (USD m)**

| Item | Low | Base | High | Basis |
|---|---|---|---|---|
| Installed capex incl. contingency | 6.5 | 9.5 | 14.0 | [technical_operations.md](technical_operations.md) |
| Pre-operating costs, outgrower scale-up, training | 0.4 | 0.6 | 0.9 | [ESTIMATE] |
| Financing fees, lender DD and legal | 0.15 | 0.25 | 0.4 | Row 13 |
| Interest during construction (IDC) | 0.3 | 0.55 | 0.9 | [ESTIMATE]: 50% average drawdown over 15 months at 15.5% (senior) and 13% (mezz) |
| DSRA (6 months) | 0.25 | 0.45 | 0.7 | Row 16 |
| Permanent working capital (equity / term funded) | 0.8 | 1.0 | 1.5 | [ESTIMATE]: the non-seasonal core of the USD 2–4.5m need |
| **Total long-term funding** | **8.4** | **12.4** | **18.4** | |
| Seasonal WC revolver limit (separate) | 1.5 | 2.0 | 3.0 | KES 195–390m |
| Cost-overrun standby equity (committed, undrawn in base) | 1.0 | 1.4 | 2.1 | 15% of capex |

**Sources, base case**

| Instrument | USD m | % of long-term | Currency | Rate (base; range) | Tenor / grace | Repayment | Security / key covenants | Likely providers |
|---|---|---|---|---|---|---|---|---|
| Founder ordinary equity (incl. Phase 0 spend and land) | 4.4 | 35% | KES/USD | Hurdle 35% (30–40%) | Permanent | — | Plus a **standby equity letter** for cost overruns of ~USD 1.4m | Founder |
| Co-investor / strategic equity | 1.5 | 12% | KES/USD | — | Permanent | — | Shareholders' agreement. Ideally a strategic partner: a large cage-fish farmer (aquafeed offtake), a feed miller (cake offtake), or a family office or angel syndicate | Strategic / family office |
| Grants / TA | 0.3 | 3% | USD | 0% | — | — | Milestone-based | AECF, foundations, IFAD-programme co-funding [PK-UNVERIFIED] |
| **Mezzanine loan** | 1.7 | 14% | USD (ask for a KES option) | **13% all-in** (11–16%): e.g. ~9–10% cash + royalty or kicker [ESTIMATE] | **8 yrs, 3-yr grace** (interest may be capitalised in years 1–2) | 5 years of sculpted amortisation | Subordinated; second charge; information rights; E&S action plan (IFC PS / DFI standards) | **AgDevCo** (precedents: Agventure, Victory Farms) |
| **Senior term loan** | 4.5 (≈ KES 585m) | 36% | **KES** (or ≤50% USD) | **15.5%** = CBR 8.75 + ~6.75 margin, floating (14–17.5%); USD option SOFR + 6% ≈ 10% | **7 yrs incl. 18-month grace** (interest-only during construction and ramp-up) | 22 quarterly instalments (or sculpted to DSCR 1.4x) | First legal charge over land and buildings; debenture over plant; insurance assignment; DSRA 6 months; DSCR ≥1.30x (lock-up), ≥1.10x (default); net debt/EBITDA ≤3.0x from year 3; gearing ≤60%; founder guarantee likely; ideally partly guaranteed (IFC risk-sharing / AGF) | KCB, Equity, Stanbic, NCBA, Co-op (one lead, possibly a club of two) |
| **Total long-term** | **12.4** | 100% | | | | | Debt 50% / equity + grants 50% | |
| **Seasonal WC revolver** | 2.0 limit (KES 260m) | — | KES | **14.5%** (13–16%) | 12 months, renewable | Revolving; clean-down 30 days/yr [ESTIMATE] | Borrowing base: 65% of seed and oil stock under collateral management or WRS receipts; 75% of eligible receivables <90 days | Same bank, or a separate bank with a collateral manager |
| Equipment supplier credit (optional) | 0.5–1.5 | — | USD/CNY | ~0–8% (embedded in price) | 12–24 months deferred | Milestones | L/C or bank guarantee | Chinese/Indian OEMs; ECA cover only for larger tickets [PK-UNVERIFIED] |

**Debt-service check (illustrative, [ESTIMATE]; the model will supersede).**
- **Senior.** KES 585m at 15.5%. Annual principal after grace is ≈ KES 106m, plus ≈ KES 90m of interest falling over time, so year-1 amortising debt service ≈ **KES 196m (USD 1.5m)**.
- **Mezzanine, from year 4.** USD 0.34m principal plus ~0.2m interest per year.
- **Peak combined debt service ≈ USD 2.0m/yr**, around operating years 3–4.
- **What EBITDA that needs.** At DSCR 1.3x, CFADS must be ≥ USD 2.6m, i.e. EBITDA ≈ USD 3.0m+ after tax and maintenance capex.
- **Steady-state EBITDA from sibling files** [ESTIMATE]:
  - Crush margin ~KES 31k/t × 15 kt = KES 465m.
  - Less processing (~KES 8k/t), giving ≈ KES 345m.
  - Plus refining margin ≈ KES 200m and feed contribution ≈ KES 150–190m.
  - Less fixed overheads ≈ KES 300m.
  - That gives **≈ KES 400m (USD ~3.1m) at full utilisation**.
- **Conclusion: the base senior quantum (USD 4.5m) is the maximum the plant can carry**, and only if utilisation reaches ≥75% by year 3.
  - If the model shows a slower seed ramp, cut senior debt to USD 3–3.5m and replace it with equity or longer-grace mezzanine.
  - Do not stretch senior debt to cover capex overruns.

### Phase 2: to 150 tpd prepress + solvent, 60 t/d refinery, +6 t/h extrusion. ~Year 4–6 after COD (≈ 2032–33).
**Trigger:** ≥40 kt/yr of seed contracted or on long-run import ([technical_operations.md](technical_operations.md)), plus 2 years of audited EBITDA.

| Instrument | USD m (base) | Currency | Rate | Tenor / grace | Notes / providers |
|---|---|---|---|---|---|
| Retained cash flow (years 2–5 after debt service) | 4–6 | KES | — | — | [ESTIMATE] |
| New equity (minority, 25–40%) at a step-up valuation | 8 | USD | Fund target ~22% USD IRR | — | Catalyst, Phatisa, Norfund/BII direct or via funds, AgDevCo equity, or a strategic (e.g. a feed multinational) [PK-UNVERIFIED for appetite] |
| DFI senior A-loan (refinances Phase 1 senior) | 14 | USD and/or KES (via TCX) | SOFR + 5–6% (≈ 9–10% USD) or ~13–14% KES | **8–10 yrs, 2-yr grace** | IFC, Proparco (Kenya Nut USD 18.7m precedent), FMO, AATIF; possibly a B-loan with Kenyan banks |
| Mezzanine (rolled over or upsized) | 2–3 | USD | 12–14% | 7–8 yrs | AgDevCo follow-on (Victory Farms precedent: USD 4m to 15m) |
| Seasonal WC (structured inventory finance) | 6–7 limit (KES 0.8–0.9bn) | KES | 13–14% | 1 yr, renewable | Collateral-managed / WRS. Possible DFI-funded bank line (AfDB/BII lines to Kenyan banks) |
| **Total Phase 2 funding** | **≈ 30 (22–41)** | | | | Post-Phase 2 target: debt ≈ 50–55% of capital, net debt/EBITDA ≤ 2.5x |

### Exit (year 7–10 from FID): trade sale or secondary at 4–7x EBITDA (§8).

---

## 7. Working-capital finance for seasonal seed and price hedging

**Size of the need.**
- Seed arrives in two peaks in western Kenya. Storage must hold **3–4 months of throughput (4,000–5,000 t in Phase 1)** ([technical_operations.md](technical_operations.md)).
- Steady-state peak working capital is **KES 650–950m (USD 5–7m)**, made up of seed stock plus input credit plus receivables less payables. Outgrower input credit alone is KES 45–95m (seed only) to KES 190–310m (full package) from Mar–Aug ([feedstock_supply.md](feedstock_supply.md)).
- Phase 1 is USD 2–4.5m.

**Instruments.**
1. **Inventory or borrowing-base revolver with a collateral manager.**
   - Most practical [PK-UNVERIFIED]: the bank advances 60–70% against stock held in a warehouse controlled by a collateral manager (field-warehousing or tripartite agreement).
   - Cost: the loan rate (~14.5%) plus a collateral-management fee of ~0.5–1.5% of stock value a year [ESTIMATE].
2. **Warehouse Receipt System (WRS).**
   - Kenya's WRS Council operates under the Warehouse Receipt System Act 2019 [PK-UNVERIFIED for the Act's year and details].
   - NCPB must lease 25% of its capacity to the private sector under WRS, and earned KES 359.7m from leasing in 2024 ([Milling MEA](https://millingmea.com/?p=2032467)).
   - WRS-certified storage cost KES 48 per 90 kg bag in month 1 (~KES 533/t), then ~KES 100/t per month ([Logistics Business Africa](https://www.logisticsbusinessafrica.co.za/warehouse-receipt-system-in-kenya-open-doors-to-maize-farmers/) [DATED]).
   - **Gap:** it was not confirmed whether sunflower or soybean are gazetted WRS commodities (the system is maize- and cereal-centric).
   - Uses: (a) let aggregators and farmer groups finance their own seed on receipts, so the crusher buys later and holds less stock; (b) pledge the crusher's own stock in certified NCPB depots (Kisumu, Bungoma, Busia) as aggregation hubs ([feedstock_supply.md](feedstock_supply.md)).
3. **Tripartite outgrower input finance.**
   - The bank lends to farmers, the processor guarantees offtake and deducts repayments at weigh-and-pay, and the processor gives an optional 10–20% first-loss [ESTIMATE].
   - Precedent: Bidco with Equity Bank ([Business Daily](https://www.businessdailyafrica.com/bd/news/counties/bidco-set-to-buy-sh120m-sunflower-seeds-from-farmers-in-meru-2301152) [DATED]).
   - **Failure mode to avoid:** a fixed farmgate price below spot. Bidco's outgrowers switched crops ([Business Daily](https://www.businessdailyafrica.com/bd/markets/bidco-taps-farmers-to-cover-edible-oil-supply-shortfall-1970404) [DATED]).
4. **Customer prepayments and supplier credit.**
   - Feed customers rarely prepay. Oil distributors may pay cash-on-delivery.
   - Imported premix, fishmeal and SBM can be bought on 30–60 day supplier terms or with bank L/Cs. Note the AfDB USD 10m trade-finance line to Family Bank ([fundsforNGOs](https://news.fundsforngos.org/2026/10/14/afdb-family-bank-10-million-trade-finance-line-kenya-smes-foreign-currency/)).
   - Pwani Oil's 2022 shutdown "for lack of dollars" ([The Star](https://www.the-star.co.ke/news/2022-06-06-pwani-oil-shuts-plant-blames-lack-of-dollars) [DATED]) shows why **USD liquidity lines** matter for any imported input.

**Commodity price hedging.**
- **There is no liquid sunflower-seed or sunflower-oil futures market usable from Kenya** [PK-UNVERIFIED].
- **Proxy hedges.** Exchange-traded proxies exist: Bursa Malaysia CPO futures (prices quoted in [Bernama](https://www.bernama.com/lite/news.php?id=2544958)), CBOT soybean oil and soybean meal ([Barchart](https://www.barchart.com/futures/quotes/ZMV26)), and soybean-meal benchmarks ([cbonds/World Bank](https://cbonds.fr/indexes/154082/)). They carry significant basis risk. Sunflower oil traded at a USD 100–150/t premium to palm in Sep 2026 and moved the opposite way that month ([market_demand.md](market_demand.md)).
- **Margin accounts.** A small processor would need a broker account and USD margin, which Kenyan banks may not support [PK-UNVERIFIED].
- **Recommended operational hedges** [judgement]:
  - (a) A **floating seed price** set as a floor plus a share of oil/cake import parity, announced before planting ([feedstock_supply.md](feedstock_supply.md)). This passes most price risk back through the crush spread.
  - (b) Keep stock turns short and cap unhedged stock at 3–4 months.
  - (c) Pre-sell 30–50% of crude oil or cake monthly to refiners and feed millers at parity-linked formulas.
  - (d) If a DFI senior loan is in USD, use **KES/USD forwards** from banks for the next 6–12 months of debt service. Forward premium ≈ the interest differential, ~4.5–5.5%/yr [ESTIMATE].
- **Policy risks (not hedgeable):**
  - Removal of the 10% CPO duty, which would cut oil parity by ~9% ([feedstock_supply.md](feedstock_supply.md)).
  - Lifting of the GMO import injunction, which would cut SBM-linked cake prices by 20–30% [ESTIMATE] ([market_demand.md](market_demand.md)).
  - The model should carry both as discrete downside scenarios.

---

## 8. Comparable transactions, failures, valuation and exit

**Comparable financings (East Africa)**

| Company | Deal | Amount | Investor / instrument | Date | Source |
|---|---|---|---|---|---|
| Agventure (Kenya, canola crush + seed) | Expansion of oil and seed processing; more outgrower purchasing | USD 9.5m | AgDevCo mezzanine | Nov 2024 [DATED]; re-reported Apr 2026 [CONFLICT] | [Africa PE News](https://www.africaprivateequitynews.com/p/kenyas-agventure-raises-95m-from); [Agrifocus](https://agrifocusafrica.com/2026/04/09/agdevco-invests-9-5-million-in-kenyas-agventure-to-advance-regenerative-agriculture/) |
| Victory Farms (Kenya, tilapia + in-house feed) | Series B | USD 35m | Equity (investors not retrieved) | 2023 [DATED] | [The Fish Site](https://thefishsite.com/es/articles/victory-farms-raises-35-million-to-fuel-east-african-tilapia-expansion) |
| Victory Farms | Follow-on (reported as KES 1.9bn) | USD 15m | AgDevCo mezzanine (after USD 4m in 2021) | 2026 | [WeAreAquaculture](https://weareaquaculture.com/news/finance/tilapia-producer-victory-group-secures-15m-follow-on-investment-from-agdevco); [Business Daily](https://www.businessdailyafrica.com/bd/corporate/companies/victory-farms-raises-sh1-9bn-to-scale-tilapia-output-5417840) |
| Victory Farms Doho feed mill (Homa Bay) | Extruded feed mill within a KES 2.2bn project | KES 1.3bn (~USD 10m) | Internal / group | 2025–26 | [The Standard](https://www.standardmedia.co.ke/business/nyanza/article/2001549421/new-bid-to-improve-fish-production-in-homa-bay) |
| Kenya Nut Company | Expansion | USD 18.7m | Proparco loan | Date not confirmed | [Africa PE News](https://www.africaprivateequitynews.com/p/proparco-backs-kenya-nut-company-with-18-7m-loan) |
| De Heus, Njeru (Uganda) | 100 kt aquafeed plant | USD 25m [CONFLICT: €22m] | Corporate | Sep 2025 | [Ecofin](https://www.ecofinagency.com/news-industry/0509-48437-de-heus-invests-25-million-in-ugandan-fish-feed-industry) |
| Mainland Group, Dodoma (Tanzania) | 30–35 kt sunflower crush + silos + feed line | USD 28m | Corporate (Chinese) | ~2025–26 | [Milling MEA](https://millingmea.com/chinese-agribusiness-giant-mainland-group-to-launch-new-sunflower-oil-plant-in-tanzania/) |
| Tunga Nutrition (Skretting/Nutreco + Unga JV) | Aquafeed capacity 24 to 45 kt | Not disclosed | Corporate JV | ~Feb 2026 | [WeAreAquaculture](https://weareaquaculture.com/news/feed/skretting-opens-new-aquafeed-plant-in-nairobi) |
| AgDevCo (fund level) | Capital raise | USD 85m | BII, Swedfund, Norfund | Date not confirmed | [Food Business MEA](https://www.foodbusinessmea.com/agdevco-raises-us85m-from-bii-swedfund-and-norfund-to-support-african-agribusiness/) |

**Read-across.**
- The realistic DFI ticket for a Kenyan oilseed or aqua processor at this stage is **USD 5–15m, mostly mezzanine or debt from AgDevCo**.
- Larger senior DFIs (Proparco, IFC) come in at **USD 15–20m+** once the business is established. That matches the proposed Phase 1/Phase 2 split.
- Strategic competitors invest **USD 25–28m** per regional plant from their own balance sheets, which is the scale Phase 2 must compete against.

**Failures and stress cases (lessons for structuring).**
- **Pwani Oil shut its plant in 2022 for lack of dollars** ([The Star](https://www.the-star.co.ke/news/2022-06-06-pwani-oil-shuts-plant-blames-lack-of-dollars) [DATED]).
  - Lesson: keep FX-denominated inputs small and hold committed USD trade lines.
  - A local-seed crusher is structurally less exposed than a CPO refiner.
- **Bidco's outgrower programme underdelivered.** Farmers switched to maize, wheat and beans when the fixed seed prices were uncompetitive, and Bidco still gets only ~5 kt of its >10 kt local seed need ([Business Daily](https://www.businessdailyafrica.com/bd/markets/bidco-taps-farmers-to-cover-edible-oil-supply-shortfall-1970404) [DATED]; [KNA](https://www.kenyanews.go.ke/?p=23808)).
  - Lesson: lenders will rightly treat **seed supply as the key credit risk**. Use floating-price contracts and size debt to a conservative ramp.
- **A 500 tpd US solvent plant built in 2014 shut in 2016** ([PHX listing](https://www.phxequip.com/Multimedia/documents/plants/solvent-extraction-plant-500-tpd-2318.pdf) [DATED]). The reason is not stated; the sibling file infers seed supply.
  - Lesson: do not debt-finance solvent capacity before seed is contracted.
- **No documented 2024–26 East African oilseed-processor insolvency was retrievable this session** (gap). Small Tanzanian and Ugandan sunflower pressers are widely reported to run at low utilisation [PK-UNVERIFIED].

**Valuation benchmarks and exit routes.**
- **Sourced anchors:**
  - KPC IPO at **≈ 8.1x EV/EBITDA** (Mar 2026). This is regulated infrastructure, an upper bound ([african-markets](https://www.african-markets.com/en/stock-markets/nse/kenya-pipeline-company-ipo-subscribed-at-105-7-listing-on-the-nairobi-securities-exchange-scheduled-for-march-10); [Rio Times](https://www.riotimesonline.com/kenya-pipeline-ipo-state-buyers-2026/)).
  - US lower-middle-market PE deals: **5.5–5.6x** (USD 1–10m EV) and **6.4x** (USD 10–25m) in H1 2025 ([Capitalpad](https://capitalpad.com/lower-middle-market-ebitda-multiples/)).
  - NASI dividend yield of 5.8% after a ~29–32% 2026 rally ([Cytonn Q3 2026](https://cytonn.com/uploads/downloads/cytonn-q32026-markets-review-vf.pdf)).
- **Unsourced context** [PK-UNVERIFIED]: global listed oilseed processors (ADM, Bunge) have typically traded at ~6–9x EV/EBITDA. NSE-listed food manufacturers (e.g. Unga Group) have traded at low single-digit earnings multiples with thin liquidity.
- **No Kenyan or East African agro-processor M&A multiple was found** (gap).
- **Exit multiple, base 5.0x (range 4–7x) EBITDA [ESTIMATE].** The reasoning:
  - Start from a US LMM baseline of ~5.5–6.4x.
  - Apply a country, illiquidity and commodity-cyclicality discount of 15–30%.
  - Add a strategic premium if a multinational wants local non-GM protein and EAC-origin oil.
  - Underwrite at ≤ the entry multiple of any Phase 2 equity.
- **Exit routes, ranked by likelihood [judgement]:**
  1. **Trade sale to a feed or aquafeed strategic** (Nutreco/Skretting via Tunga with Unga, De Heus, or Victory Farms/SamakGro) seeking a local non-GM protein supply. This is strongest if the GMO import ban persists.
  2. **Trade sale to an edible-oil refiner** (Bidco, Kapa, Pwani, Menengai) wanting EAC-origin soft oil. EAC-grown seed should enable duty-free intra-EAC exports, unlike oil refined from imported CPO, which pays 25% ([market_demand.md](market_demand.md)).
  3. **Regional agri-trader** (ETG, Olam/ofi, Cargill, Mainland Group) [PK-UNVERIFIED for appetite].
  4. **PE secondary or buy-out of the founder** by a Phase 2 fund or another fund (Catalyst, Phatisa).
  5. **NSE listing.** Unlikely below ~USD 50m EV given the IPO market's dependence on state-linked buyers ([Rio Times](https://www.riotimesonline.com/kenya-pipeline-ipo-state-buyers-2026/)).
- **Illustrative exit value** [ESTIMATE]: post-Phase 2 steady-state EBITDA of USD 8–10m × 5.0x ≈ **USD 40–50m EV**.

---

## 9. Recommendations and next actions

1. **Phase 1 structure (base USD 12.4m long-term plus a USD 2m WC line):**
   - 47% founder and strategic equity, plus 3% grants.
   - 14% AgDevCo-type USD mezzanine (8 years, 3-year grace).
   - 36% KES senior bank loan (7 years, 18-month grace, ~15.5%), ideally with IFC or AGF risk-sharing.
   - A separate KES borrowing-base revolver under collateral management.
   - Plus ~USD 1.4m of committed standby equity.
2. **Phase 2 (≈ USD 30m):**
   - Bring in outside equity (~USD 8m, a 25–40% minority) at a step-up valuation.
   - Refinance Phase 1 senior debt into a **DFI 8–10 year A-loan** (USD or TCX-hedged KES).
   - Scale structured inventory finance to KES 0.8–0.9bn.
3. **Phase 0 actions to convert assumptions into indicative terms (next 90 days):**
   - (a) Approach AgDevCo with a teaser and request indicative mezzanine terms, a KES option and smallholder TA.
   - (b) Get indicative KES term and WC terms from at least two of KCB, Equity, Stanbic, NCBA and Co-op, and ask specifically about IFC/BII/AGF risk-sharing cover.
   - (c) Get collateral-manager quotes and confirm the WRS eligibility of sunflower and soy with the WRS Council.
   - (d) Check AECF's open calls and the status of the IFAD aquaculture programme.
   - (e) Get tax advice on the interest-restriction cap, WHT gross-up on foreign loans, the 5-year loss limit, and investment deductions or SEZ status (SEZ incentives capped at 10 years ([US State Dept ICS 2026](https://www.state.gov/reports/2026-investment-climate-statements/kenya))).
4. **Do not:**
   - Debt-finance the solvent plant before ≥40 kt of seed is secured.
   - Take USD senior debt above ~50% of total debt.
   - Sell Phase 1 equity to a fund pre-revenue.
   - Rely on US (USAID/DFC) guarantees.

---

## 10. Gaps and uncertainties

1. **Research coverage was severely limited.** Only one web search was possible (budget exhausted), and the single direct fetch failed with DNS. Every figure tagged [PK-UNVERIFIED] or [ESTIMATE] needs checking, especially:
   - AgDevCo, AATIF, Africa Guarantee Fund, AECF and IFAD terms and current programmes.
   - DFC's 2026 status.
   - Phatisa, Kuramo and Inside Capital fund sizes and appetite.
   - TCX KES pricing.
   - Kenyan tax rules on interest deductibility and WHT.
2. **No disclosed loan terms** (rate, tenor, grace, covenants) for any Kenyan agri DFI deal, Agventure and Victory Farms included. Every term-sheet number above is a structuring assumption.
3. **SOFR level** in Oct 2026 was not retrieved. Base 4.0% is inferred from a 5.24% 10-year and a hiking Fed.
4. **No Kenyan or East African agro-processor EV/EBITDA multiples** and no documented oilseed-processor insolvency from 2024–26. The exit multiple relies on US benchmarks with a country discount.
5. **WRS eligibility of oilseeds** and the availability of collateral managers in western Kenya are unconfirmed.
6. **Victory Farms Series B investors**, and whether its 2026 USD 15m is the same as the "KES 1.9bn" raise, are not confirmed. **Agventure deal date** conflicts (Nov 2024 vs Apr 2026), and the prior-notes URL for Agventure (`foodbusinessmea ?p=2133850`) appears to point to the AgDevCo fundraise article instead.
7. **The debt-capacity check depends on unvalidated EBITDA** (≈ USD 3.1m at full Phase 1 utilisation, from sibling-file arithmetic). If the seed ramp is slower, senior debt falls to USD 3–3.5m and equity rises to ~60%.
8. **KES path.** No 2027 KES/USD forecast was found. The 4% drift is inferred, and the election tail (Aug 2027) is not quantified.
9. **Policy shocks that cannot be hedged:** CPO duty removal, the outcome of the GMO import injunction, and ad hoc duty waivers on maize and soy. Their effect on lender appetite is not quantified.
