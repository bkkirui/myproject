# Review r2 - Livestock / Poultry Health / Biosecurity (adversarial, round 2)

Scope: PLAN.md v2 against my r1 findings (r1-livestock.md, r1-poultry-crops.md). Tags: [MAJOR] = material loss, safety/legal exposure or plan failure. [MINOR] = fix but not fatal. Items that depend on Gate 0 answers and are gated there are not raised.

## (a) Were the r1 MAJORs fixed?

Genuinely fixed, not re-raised: L2 (zoonosis/worker safety), L3 (biosecurity and 30-day quarantine, staff flow), L4 (species rules, copper, colostrum), L5 (FEC-guided selective treatment), L6/P8 (vet-of-record, locked register, no-sale flag), L7 (labour as a constraint on enterprise choice), L8/P2 (rationalization), L9 (ID and movement documents), L10 (fallen stock), L12/P6/P7 (poultry power/ventilation, GSM alarms, vaccine fridge), P1 (poultry decided at G1 with a burden of proof), P11 (season table), P12 (water and destock trigger).

Fixed in form but with defects introduced by the fix: L1/P4 (notifiable disease), L11/P5 (thresholds). See items 1 and 2.

## Findings

1. [MAJOR] Poultry mortality thresholds are internally inconsistent, and the broiler numbers are wrong for the stated purpose.
   Problem: Section 7 sets broiler amber at > 0.5%/day (after week 1) and red at > 1% in 2 days. That is the same rate (0.5%/day), so red is no stricter than amber. The only real red is "doubling in 24 h". Typical post-week-1 broiler mortality is about 0.05-0.1%/day. A 0.5%/day amber is therefore 5-10 times normal, and the first alert arrives after 100 dead birds a day in a 20,000-bird house. The change log justifies this as "broiler baselines are higher", which is true only for week 1 and is why week 1 is excluded. Layer amber of 0.1%/day is about 5-10 times a normal 0.01-0.03%/day, which is acceptable but undocumented. Percentages are meaningless for small flocks (0.1% of 300 hens is 0.3 birds), so the rule needs an absolute count floor. Section 7 never says the poultry red triggers are the HPAI/Newcastle suspect triggers (only the ruminant cell says "notifiable-suspect rules apply"), so a poultry red could be handled as a husbandry call with no lockdown or authority report.
   Why it matters: this is the plan's main early-warning for the enterprise with the fastest and most total loss, and my own r1 fix produced a table that tiers nothing.
   Fix: broilers amber > 0.2%/day or 2x the flock's own trailing 7-day mean; red > 0.5%/day or doubling in 24 h or any single-day count above a stated absolute number. Add a week-1 rule (e.g. > 1.0% cumulative by day 7 is amber, vet review). Add "or N birds, whichever is smaller" for small flocks. State in the poultry cells that red means house lockdown, a vet call and the notifiable-suspect response in Section 6. Keep the figures marked as vet-calibrated defaults.

2. [MAJOR] The notifiable-disease design treats every single sudden adult death as a suspect-disease event, which is unworkable, and it sits beside a mortality bonus that rewards relabelling.
   Problem: Section 6 puts "sudden deaths with no cause" on the suspect list. Section 7 makes "any sudden unexplained death" in adult ruminants red / call now. The response is a whole-holding standstill (animals, carcasses, milk, eggs, manure, vehicles, people) plus a call to the vet and the authority. Lightning, bloat, clostridial disease, hypomagnesaemia, snakebite and plant poisoning produce isolated sudden deaths in every herd every year. In a sizeable herd that means several full standstills and authority calls a year. Staff and managers will learn that "unexplained" is expensive and will find explanations (the plan pays bonuses on mortality KPIs and the cause is often unverifiable without a post-mortem), or will stop calling. Both outcomes destroy the habit needed for a real FMD, anthrax or HPAI event. The opposite risk also exists: a rule that never distinguishes anthrax-endemic regions from lightning-prone ones is wrong in both directions.
   Why it matters: legal exposure from non-reporting, plus either needless trading disruption or a trained reflex to under-report, plus a perverse incentive on cause-of-death data.
   Fix: make it a two-step triage written with the vet and authority. (i) Any sudden death: carcass left unopened and covered, photographed from a distance, vet phone triage within 2 h (not a full standstill). (ii) The vet or authority escalates to report and standstill on defined criteria: anthrax-endemic region or history, 2 or more deaths in a group in 24-48 h, bleeding from orifices, fever/vesicle/neurological signs in survivors, or the vet cannot attribute a cause. Add a rule that cause "unexplained" stays "unexplained" until a vet or authority post-mortem, and that the mortality KPI uses vet-confirmed cause. Add a live call test of the 24-h authority and vet numbers to the G2 outbreak tabletop (confirm sample-submission and out-of-hours contacts).

3. [MAJOR] No interim protection exists between today and the signed SOPs, although the plan's own season table puts a peak in that window.
   Problem: Principle 4 says safety is pre-authorised and never waits for the owner. But the notifiable suspect list, standstill card, emergency spend authority, euthanasia authorisation and alert chain are Section 6/7 content that become operational only when SOPs are signed at G2 (week 6-16). G0 (weeks 0-3) only collects answers and the baseline audit may be done by "an extension officer, consultant vet or farm consultant", with no requirement for a vet-led herd and flock health baseline. Section 10 says "anything not irreversible continues as the incumbent manager planned" and the S. temperate column has lambing and calving under way now. G0 even asks whether a manager exists today. If none does, or the incumbent is weak, there is a 6-16 week window with an unknown disease status (brucellosis, TB, Johne's, CAE, resistant worms), an unknown drug-store and withdrawal status, no vet-of-record and no written reporting authority.
   Why it matters: this is the highest-risk period for an owner who has not yet seen the farm, and the plan's own principle is not operational in it.
   Fix: add a "Day-7 safety pack" as a G0 exit criterion: confirmed vet-of-record with 24-h cover, authority contact verified by call, a one-page suspect / standstill / do-not-open card posted at each site, a signed owner letter pre-authorising emergency spend and reporting (lawyer to confirm the manager may report for the holder), a named person authorised to euthanise, a water/power/fridge status check, and a drug-store inventory reconciliation. Make the baseline audit explicitly include a vet-led health review (test status, vaccination history, FEC/resistance baseline, body condition, facilities, existing movement restrictions or outstanding testing duties, drug-store legality).

4. [MINOR] The escalation ladder and the emergency authority row read as sequential waits.
   Problem: Section 5 gives the manager emergency authority, "then vet/deputy if owner and representative silent 2 h", and the ladder is "owner 30 min -> representative 2 h -> vet/adviser". Read literally, the vet is involved only after 2 h. Poultry ventilation or power failure kills in 15-30 minutes, and Section 6 says reporting never waits.
   Why it matters: a manager who is unsure will wait for the owner during the one event where waiting kills.
   Fix: state "act first, notify in parallel". The manager acts and calls the vet immediately within the 1% envelope. The ladder governs who is informed and who may extend the envelope, not whether the first response happens.

5. [MINOR] Ruminant suspect list and abortion rule: gaps and scale blindness.
   Problem: the list omits skin nodules/pox lesions (LSD, sheep/goat pox), mouth erosions with oculonasal discharge and diarrhoea (PPR, BVD/BT picture), and hot, swollen or cyanotic head/comb signs in poultry. "Abortion >= 2 in 7 days" is a rule that fires constantly in a large flock with routine enzootic abortion and misses a 20-head herd where one is already unusual. In many jurisdictions a single cattle abortion (brucellosis) must be reported or tested, so the plan's default can sit below the legal floor. Baselines that replace defaults "after 8-12 weeks" cannot represent seasonal young-stock mortality, and could loosen red rules to the new normal.
   Fix: add the missing signs; express abortion as a count or percentage of females at risk, bounded below by the national rule from Gate 0; require a seasonal or benchmark baseline for young stock; baselines may tighten but never loosen red triggers.

6. [MINOR] Tag-retention and death-photo rules contradict the do-not-open rule.
   Problem: Section 5 requires a photo of the tagged carcass, tag retained and witness. Section 6 says do not open a suspect carcass. Removing an ear tag from a possible anthrax or notifiable carcass exposes a worker.
   Fix: for suspect deaths, photograph in situ with the tag number visible and leave the tag on. Tag removal and sampling are done by the vet or authority.

7. [MINOR] Cross-species feed and litter hazards were dropped in the v2 rewrite of my r1 L14.
   Problem: Section 4 covers moisture and aflatoxin only. Missing: ionophore coccidiostats (monensin, salinomycin) in poultry feed, which are lethal to goats, sheep and cattle if feed stores, mixers or scoops are shared; urea and ruminant-protein feed rules; poultry litter on grazing land (sheep copper, grass tetany, carcass-remnant botulism in cattle) given the manure-integration plan in Section 6; poisonous-plant paddock check; water quality test.
   Fix: separate, labelled feed stores and equipment per species; no litter on sheep pasture or fed to ruminants unless the vet approves; add a poisonous-plant and water-test line to the baseline.

8. [MINOR] The "no-sale flag" lives in records that the paper-first design may not check at load-out.
   Problem: Section 8 starts on paper, and the flag is described as a record. The gate-pass rule does not require checking the treatment register for withdrawal status. Milk and eggs are named for standstill but have no residue rule.
   Fix: make the signed gate pass and egg/milk dispatch sheet list the withdrawal check (animal ID against register, physical mark seen) as a mandatory line completed by the second person.

9. [MINOR] The G1 stress set and kill triggers do not model a notifiable outbreak.
   Problem: "disease -10% stock" is not the HPAI/FMD case, where poultry are 100% culled, holding sales are frozen 30-90+ days, restocking waits at least the downtime, and compensation is late and partial. The "owner hours > budget by 50% for a quarter" kill trigger would also fire on a single declared outbreak.
   Fix: add a notifiable-event scenario (zero sales for 90 days, full-flock loss, 6-12 month compensation lag) to G1(a). Exclude hours during a declared emergency from the kill trigger and replace them with a post-incident review.

10. [MINOR] Vet-independence rule may be unachievable, and vet access is not a viability criterion.
   Problem: "the vet who prescribes does not also certify deaths" assumes at least two vets. The plan asks for vet-of-record, post-mortems, 24-h cover and phone triage, but only records "nearest vet" at G0.
   Fix: add vet response time and out-of-hours cover as a G1 criterion; if there is only one vet, use a second practice or the authority vet for death certification, and add trained-paraprofessional protocols if response time is long.

11. [MINOR] Water thresholds contradict the design target.
   Problem: Section 4 requires 24-48 h of backup storage, while Section 7 sets amber at reserve < 48 h and red at < 24 h. A compliant farm would sit permanently in amber, and in red if designed to the 24 h minimum.
   Fix: set the alert on the margin below the designed storage (e.g. amber below 75% of design, red below 50%) or design storage to at least 72 h.

12. [MINOR] "No blanket drenching" is stated without clinical exceptions.
   Problem: haemonchosis in goats and weaners can kill within 2-3 weeks, and FEC turnaround or competent scoring may not exist on a remote farm.
   Fix: add vet-defined exceptions (high-risk classes and periods, an outbreak, lab delay beyond a stated number of days) and name who runs FEC and where.

13. [MINOR] Welfare and food-safety items from r1 L17/L20 are only partly absorbed.
   Problem: no fit-to-load decision rule, no rule on dehorning/castration/docking with pain relief and legal limits, no firearm or captive-bolt licensing note for the euthanasia person, no milk/egg hygiene SOP.
   Fix: add one line each under welfare, and include egg registration, grading and layer salmonella programme rules in the G1 poultry decision where the country requires them.

## Verdict

The v2 plan resolves most r1 majors well. The three remaining MAJORs are a poultry alert table that does not tier, an unworkable single-sudden-death notifiable trigger that creates a relabelling incentive, and an unprotected interval between now and the signed SOPs.

VERDICT: 3 MAJOR remaining
