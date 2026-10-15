# Change log

## Part 1: v2 → v3 (round-2 reviews)
Codes: R2-L livestock, R2-A agronomy, R2-G governance, R2-E economics (MAJOR items). "PLAN" = PLAN.md; "A"/"B" = appendices. Cheap MINORs are listed at the end.

| Item | Where / how addressed |
|---|---|
| R2-L1 poultry thresholds | A2 retiered: broiler amber 0.2%/day or 2x trailing mean, red 0.5%/day or doubling or absolute count; week-1 rule; small-flock "N birds or %, whichever is smaller"; layer 0.05/0.1; poultry red = lockdown, vet call, notifiable-suspect response. Marked vet-calibrated |
| R2-L2 sudden-death trigger | A1 two-step triage (unopened carcass, in-situ photo, vet phone triage in 2 h; escalation criteria); "unexplained" until post-mortem; KPI uses vet-confirmed cause; live call test in G2 tabletop |
| R2-L3 unprotected interval | PLAN section 2 Day-7 safety pack as G0 exit criterion; vet-led health review in baseline audit; interim lead in section 3 |
| R2-A1 this-season memo | PLAN section 9 rewritten: irreversible acts decided once in a week 1–2 memo, agronomist review, capped input spend, feed-first, independent receipt reconciliation. The v2 wording was inverted and is replaced |
| R2-A2 timeline vs peaks | PLAN section 3: interim lead runs G2; G2b for tests needing the manager; manager start in a trough with retention through peaks; G3 not started inside a peak unless interim lead runs it |
| R2-A3 drought | A2 leading triggers (rainfall/pasture shortfall with staged response; feed-days red at 90 projected, not 60 current); A5 irrigation demand and lead time; PLAN G1 item 7 crop/forage insurance decision |
| R2-A4 cross-enterprise paths | A4 feed-flow, litter and medicated-feed rule with medicines register and no-sale flag link; owned by WP4, vet and agronomist co-sign |
| R2-A5 G1 inputs / Farm Model | PLAN section 4 input tags and conditional pass (15% margin of safety, re-confirmation triggers); section 8 rows for Farm Model, ration, water; model owner and version log (A6). Regional defaults first, overwritten at G1 |
| R2-G1 representative capture | B2 caps, dual approval, bank notifications, vetting, fidelity cover, non-relation, quarterly cross-check |
| R2-G2 whitelist/vendor hole | B3 vendor creation is T3, per-payee caps, exception-report batch, reconciliation by a non-preparer, change logs to owner, bank daily limit |
| R2-G3 paper vs integrity | PLAN section 7: paper for recording only; transmission via unit-lead capture to entity-owned store; completeness on raw submissions. B7 |
| R2-G4 emergency envelope | B5 aggregate cap, non-payee approver, logged notice at declaration, bank payment, 72-h review. Combined with R2-L4 act-first rule (A1) |
| R2-G5 fraud response | B8 one-page protocol; failed spot-count starts it; PLAN kill triggers reference it |
| R2-E1 decision sheet | PLAN "Decision sheet": approve G0+G1 only, capped spend, outcomes, stop points, dates, five actions. Change log, species and threshold detail moved to separate files. Body is about 2,100 words including tables (the extra is mostly tables) |
| R2-E2 time budget | PLAN section 5: one table by phase, honest year-1 total (~400–450 h, ~8 h/week) and A3 (~260 h/yr). T1 sized from 24 months of purchase lines plus supply agreements, target T2 queue 30–45 min/week; 30-min clock replaced; kill trigger defined against the phase total, emergency days excluded |
| R2-E3 overhead cap | B10 line-by-line definition, management cost reported separately, three scale bands with caps, non-waivable core, expected-loss test per optional control |
| R2-E4 timeline | PLAN section 3 dated critical path, earliest-possible durations, interim lead, G2b, manager start in a trough, earliest A3 Q3 2028 (plan Q1 2029) |
| R2-E5 G1 hurdle | PLAN section 4: base margin must beat best alternative plus risk premium (default 3–5% of invested capital); default recommendation is the best alternative if it fails; stress limit signed |

**Rejected or modified:**
- R2-E1 asked for body under about 2,000 words. The prose is; with tables and headings the file is about 2,100. I kept the tables because they carry the decision content.
- R2-L1: the reviewer's absolute-count figure is left to the vet (no flock size is known), with a default N for small flocks only.
- R2-G1: the second-signature role for the representative is limited to the power-of-attorney route, not general dual signing, to protect the owner's time budget.
- R2-A2 (c): consultant on call in G3 is included, but I did not make the L1 regime stricter than the existing A1 approvals.

**MINORs folded in (cheap):** R2-L4 act-first; R2-L5 missing signs and abortion scaling, baselines tighten only (A1/A2); R2-L6 tag stays on suspect carcass (A1); R2-L7/R2-A4; R2-L8 withdrawal-check line on gate pass (A3); R2-L9 notifiable scenario in G1 and kill trigger excludes emergencies; R2-L10 vet access in G1; R2-L11 water thresholds relative to design; R2-L12 drench exceptions; R2-L13 welfare lines; R2-A6 G1 pass definitions; R2-A7 crop/feed signals; R2-A8 chemical column; R2-A9 forage separate from cash crops; R2-A10 machinery; R2-A11 "other" column; R2-A12 combined outbreak-in-peak tabletop; R2-A13 yield verification; R2-A14 capital lines; R2-G6 core set; R2-G7 leave in charter and A3 criteria; R2-G8 privacy/labour row; R2-G9 gate log reporting line; R2-G10 small-staff controls; R2-G11 auditor biosecurity; R2-G12 MFA/call-back; R2-E6 coordinator; R2-E7 charter variant and wage test; R2-E8 representative vetting; R2-E9 "clean" defined, spot-count frequency, whitelist benchmarking; R2-E10 levels renamed A1–A3 and codes disambiguated; R2-E11 presence front-loaded.

## Part 2: v1 → v2 (round-1 reviews)
Section numbers (S4, S5...) refer to PLAN-v2.md; their content now lives in the PLAN.md sections and appendices indicated in Part 1. Codes: R1-L livestock, R1-P poultry/crops, R1-G governance, R1-E economics.
Codes: L = livestock, P = poultry-crops, G = governance, E = economics. Minor items were folded in where cheap (e.g. L13–20, P14–25, G13–24, E13–19); Stata/R dropped and deliverables made testable.

| Item | Where / how addressed |
|---|---|
| R1-L1 notifiable disease | S6 notifiable design: suspect list, standstill, no carcass opening, automatic same-hour owner/vet notice; reporting not owner-dependent; Gate 0 names authority |
| R1-L2 zoonosis/worker safety | S6 worker safety line; workers' compensation in S5 insurance |
| R1-L3 biosecurity/quarantine | S6 layout and quarantine defaults (30 days), staff flow, visitor log |
| R1-L4 species differences | S6 species rules, retained species only; vet signs calendar (S9) |
| R1-L5 worms/FAMACHA | S6: FEC-guided selective treatment, annual resistance test, competency check |
| R1-L6 drugs/withdrawal | S6 medicines: vet-of-record, locked register, no-sale flag, cold chain |
| R1-L7 labour | S4 labour model, 7-day coverage, birthing surge; staffing constrains enterprise choice |
| R1-L8 too many enterprises | S4 rationalization (default 2–3 in year 1); audit and SoD in S5. Not "start with one": the G1 screen decides, because existing stock may force a managed sell-down |
| R1-L9 ID/traceability | S6 individual ID, movement documents |
| R1-L10 disposal | S6 fallen-stock method per local law |
| R1-L11 thresholds/alerts | S7 table; escalation timers in S5; silence alerts; quarterly chain test |
| R1-L12 poultry safety | S6 poultry specifics, layout rule, power/ventilation; S8 stand-alone alarms |
| R1-P1 poultry undecided, location gate | G0 intake; S4 poultry decided at G1; economic screen |
| R1-P2 enterprise sprawl | S4. Partly rejected: no fixed "one ruminant + poultry" default, since the margin and staffing screen should choose; poultry carries a burden of proof |
| R1-P3 biosecurity system | S6 layout, zoning, log, outbreak plan |
| R1-P4 notifiable duty | S6 (as L1) |
| R1-P5 mortality triggers | S7 table. Conflict with L11 (0.1% for all poultry) resolved: broilers 0.5%/day, layers 0.1%/day, since broiler baselines are higher; doubling is red for both. Evening form plus silence alert |
| R1-P6 power/water SPOF | S4 water; S6 generator, fallback; S8 GSM alarms |
| R1-P7 cold chain | S6 medicines/vaccine fridge; egg room, processor/cold-chain named in the G1 poultry decision |
| R1-P8 drug enforcement | S6 medicines |
| R1-P9 feed budget | S4 shared model at G1, not at the end; mycotoxin and moisture rules |
| R1-P10 labour peaks | S4 labour model; S6 crops histogram; S10 no launches inside peaks |
| R1-P11 seasons/today | S10 conditional table, fast-track rule, lead times; G4 requires a full cycle. A full 18-month layer cycle is not demanded; one placement plus ruminant and crop events suffice |
| R1-P12 climate/water | S4 water budget, destock trigger; crop insurance via S5 |
| R1-P13 manager SPOF/verification | S5 audit, reconciliation, benchmarks, incentives on audited numbers; owner crisis time in S8 |
| R1-G1 manager SPOF/fraud | S5 "manager cannot" list, leave, rotation (add compulsory 10-day leave and unit-lead rotation to the charter) |
| R1-G2 segregation of duties | S5 four-way split, three-way match. Modified: owner releases each payment, except a whitelist batch, to fit the time budget |
| R1-G3 bank/cash | S5 cash and bank |
| R1-G4 audit independence | S5 audit tiers; cost vs independence resolved by scaling to G1 |
| R1-G5 inventory | S5 stock paragraph |
| R1-G6 authority | S5 tiers, cumulative caps, emergency envelope, owner-only list |
| R1-G7 incentives | S5 incentives |
| R1-G8 self-reported data | S5 data integrity |
| R1-G9 key person/collusion | S5 contract, credentials, deputy rules, whistle-blower, 72-hour playbook |
| R1-G10 owner oversight capacity | S5 representative, ladder, POA; S8 unannounced visits |
| R1-G11 insurance/entity | S5 legal and insurance, lawyer sign-off |
| R1-G12 payroll | S5 payroll. Biometrics only if legal and viable; geotag or muster otherwise |
| R1-E1 no economic case | G1 viability gate, S4 budgets and scenarios, overhead cap default |
| R1-E2 enterprise mix | S4 (as P2) |
| R1-E3 1 hr/week | S8 time budget with crisis reserve, representative, logged metric. Modified: 4–8 weeks of presence cut to about 3–4 weeks in year 1 to fit an academic's calendar |
| R1-E4 manager SPOF/economics | S5 vetting, probation, deputy scaled, 72-hour playbook; S10 recruitment from week 1 (offer after G1) |
| R1-E5 seasons/proof period | S10, G4 staged autonomy. Modified: minimum 12 months rather than up to 18, extended if cycle elements are missing |
| R1-E6 no gates | S3 gates, kill triggers |
| R1-E7 generic plan | G0 intake and baseline audit before WP drafting |
| R1-E8 technology | S8. Partly rejected: "tech last" holds for data and dashboards, but life-critical alarms stay because loss avoided is large and they run on GSM |
| R1-E9 agent limits | S9 sign-off matrix; S4 shared model first |
| R1-E10 audit thin | S5 audit and controls, costed at G1 |
| R1-E11 working capital | S3 G1 stress scenarios, 24-month cash flow, reserve, destock triggers |
| R1-E12 labour economics | S4 labour model, S8 pictorial field pack; labour-law review in S5 |

**Unresolved by design (dependent on Gate 0):** all numeric defaults, the season column, legal structure and insurance availability, and whether the economics support the management layer at all.

