# Review r3 - Livestock / Poultry Health / Biosecurity (adversarial, round 3)

Scope: PLAN.md v3, Appendix A, Appendix B, CHANGELOG.md, against r1-livestock.md and r2-livestock.md. [MAJOR] = material loss, safety/legal exposure or plan failure. [MINOR] = fix but not fatal. Figures that are explicitly vet-calibrated defaults and gated at G0/G1/G2 are not raised unless the written rule is wrong as drafted.

## (a) Were the r2 MAJORs fixed?

- R2-L2 (single sudden death treated as a notifiable event): genuinely fixed. A1 now has the two-step triage with unopened carcass, in-situ photo, tag left on, 2 h vet phone triage, defined escalation criteria, "unexplained" until post-mortem, and a KPI that uses vet-confirmed cause. The pattern is correct for ruminants.
- R2-L3 (unprotected interval): fixed for the emergency case. The Day-7 pack and the vet-led baseline review are in place and are a G0 exit criterion. Residual gaps are in item 3 (MINOR).
- R2-L1 (poultry thresholds): fixed in tiering, but the fix introduced a new defect. See item 1 [MAJOR].

All other R2 MINORs I checked in the CHANGELOG are present as claimed: act-first, missing signs, abortion scaling, tag-on, withdrawal line on the gate pass, notifiable scenario in G1, vet access in G1, water relative to design, drench exceptions, welfare lines, ionophore/litter/copper rule.

## Findings

1. [MAJOR] The poultry red tier is a hair-trigger that auto-fires a whole-holding standstill and authority report, with no poultry equivalent of the ruminant two-step triage.
   Problem: A1 lists "a red poultry threshold" under *immediate standstill and report (no triage)*, and A2 says poultry red means lockdown, vet call and the notifiable-suspect response. Several red cells then fire on routine events, as drafted:
   - Small flocks: "N birds or the percentage, whichever is smaller". For a layer flock under about 1,000 birds, 0.1% is under one bird, so the smaller value means any single death is red. Normal layer loss is about 0.01-0.03%/day (more in free-range with predation), so a 500-hen flock will go red every few days.
   - The small-flock row has no week-1 carve-out. Normal brooding mortality is 0.3-0.5%/day in the first days. Six dead chicks a day in a 1,500-chick brood is routine but is red.
   - "Doubling in 24 h" has no absolute floor. 5 to 10 dead birds in a 20,000-bird house is red.
   - Layer "feed/water intake drop >10%" and "egg drop >=10% in 2 days" are red. Heat, a feed change, a lighting fault or a blocked drinker produce these routinely. Published poultry-disease suspicion triggers sit at larger intake drops (of the order of 20%) over longer periods.
   - Power loss or house over-temperature is also red, so a ventilation failure with heat deaths becomes a "notifiable suspect" report.
   Why it matters: this is the same mechanism I rated MAJOR in r2 for ruminants. If every husbandry event is a suspect-disease report, staff learn that red is expensive. They then relabel causes (the bonus uses mortality) or stop calling, and a real HPAI or Newcastle event is missed. A false official suspicion also freezes sales, which the owner pays for.
   Fix: apply the two-step logic to poultry. Red = house lockdown plus vet phone triage within 2 h (not an automatic report). Go straight to report and standstill only on the defined poultry signs already in A1 (swollen head/comb, respiratory signs with deaths, egg drop with deaths) or when the vet cannot attribute a cause. Remove the small-flock "whichever is smaller" wording; use the N-bird count alone, with a floor. Exclude week 1 from the small-flock row. Add an absolute floor to the doubling rule. Treat power/temperature red as a welfare emergency (separate response) unless disease signs are present. Keep all numbers as vet-calibrated defaults.

2. [MINOR] The ruminant "no triage" list is still over-broad on three signs.
   Problem: "neurological cases" (grass tetany, listeriosis, polioencephalomalacia and tetanus are common), "skin nodules or pox lesions" (orf in lambs and kids, warts, tick and fly lesions) and "drooling" (plant awns, choke, orf) each trigger an immediate standstill and report with no triage. Single-animal events of this type occur in most flocks every year.
   Why it matters: same relabelling and under-calling risk as item 1, at lower volume.
   Fix: for these three signs, specify "multiple animals, generalised, or vet cannot exclude" as the report trigger. A single animal gets vet triage within 2 h with isolation in the meantime. Keep vesicles plus lameness/drooling in several animals, abortion storms and haemorrhage as immediate.

3. [MINOR] The Day-7 pack covers emergencies but not the ordinary interim losses between G0 and G2 (about Nov 2026 to Apr 2027).
   Problem: SOPs are signed about 10 weeks after G1, and the memo in section 9 covers irreversible crop and input acts only ("everything else continues as is"). The pack has no withdrawal check at sale or load-out, no check of birthing-season arrangements (the S temperate column has lambing and calving under way now: night watch, colostrum, clostridial cover, predators), and no check on the ionophore and copper separation if poultry and sheep co-exist.
   Why it matters: residue violations and peri-birth losses are the likeliest actual losses in the interim. The incumbent's practice is unknown.
   Fix: add three lines to the Day-7 pack, each owned by the baseline vet: an interim withdrawal check on every sale or dispatch, a one-page live-season check (birthing, feed-flow, copper), and a named stockperson for the peak.

4. [MINOR] The decision sheet claims the manager start (about Apr-Jun 2027) is "in a trough", which contradicts section 9 and section 3.
   Problem: for N temperate, section 9 puts Mar-May at calving/lambing/planting and Jun-Sep at harvest/hay, yet section 3 lists "N temperate Jun-Aug" as a trough. For S temperate, Mar-May is harvest and autumn breeding. The rule at the end of section 9 says no manager start inside a peak.
   Why it matters: mitigated by the interim lead staying through peaks, so not fatal, but the headline date can mislead the owner.
   Fix: say "trough or interim-lead-covered peak" in the decision sheet, and align the section 3 trough list with the section 9 table (N temperate: Nov-Jan only).

5. [MINOR] The emergency envelope cap can block welfare and statutory spend.
   Problem: B5 caps 1.5% AOB per quarter and 3% per year, "after which every event needs the owner or representative". The fall-through to the deputy is not clearly retained after the cap. A mass-mortality disposal, water haulage in drought or authority-directed measures can exhaust the quarter.
   Why it matters: conflicts with principle 1 ("safety acts first") and with duty-of-care and legal obligations when owner and representative are unreachable.
   Fix: carve out vet attendance, humane destruction, carcass disposal and authority-directed measures from the aggregate cap (still logged and reviewed in 72 h), or state that the deputy fall-through survives cap exhaustion for these categories.

6. [MINOR] Medicines: two loopholes and one lost item from r1.
   Problem: A3 allows treatment "on vet or manager order". Prescription-only medicines should be given under the vet's written protocol or prescription, and critical antimicrobials should be vet-only. The r1 antimicrobial-stewardship point is no longer explicit. The "physical mark" does not work for egg-laying flocks, so the flag must be flock- or house-level.
   Fix: "manager order within the vet's written protocol only"; one stewardship line (critical antimicrobials vet-only, treatment rate on the KPI list); flock/house-level withdrawal flag for eggs.

7. [MINOR] Poultry competence and housing order.
   Problem: the plan has one vet-of-record. A ruminant practitioner often has no poultry competence, and G1 item 6 tests only response time and cover. A3 has no poultry vaccination programme (Newcastle, Marek, IBD, fowl pox, coccidiosis by region), no routine poultry post-mortem route, and no housing-order step for free-range birds.
   Fix: G1 item 6 should require a poultry-competent vet or lab route. Add a vet-signed poultry vaccination and necropsy line in A3, and a housing-order response in the vet's playbook.

8. [MINOR] Triage step 1 gaps.
   Problem: no fallback if the vet cannot be reached within 2 h (go to the authority vet); no instruction to exclude scavengers, dogs and livestock from the covered carcass; "cluster of deaths" for young stock in A2 is not numeric and is not aligned with A1's "2 or more in 24-48 h".
   Fix: add the three phrases.

9. [MINOR] Standstill and visitor mechanics.
   Problem: the exemption list names only feed and water deliveries. Milk collection for any dairy animals, egg collection, essential animal-care labour and carcass removal are not covered. The plan says nothing about suspending auditor and visitor access during a standstill. Fortnightly pilot spot-counts of live animals (B6) need a late-pregnancy rule (count in situ without mustering) and a declared biosecurity route.
   Fix: widen the vet-approved exemption list, suspend non-essential visits during a standstill, and add the late-pregnancy counting rule.

10. [MINOR] A2 "baselines may tighten but never loosen red triggers" can collide with vet calibration.
    Problem: for free-range layers or predation-heavy systems, normal mortality exceeds the default red, so red is permanent unless the vet resets it. As written, the vet can replace defaults but a baseline cannot loosen them.
    Fix: state that only the vet may reset a red default, in writing, after a documented baseline.

11. [MINOR] Day-7 and fallen-stock details.
    - The Day-7 pack needs "lawyer confirms the manager may report for the holder", but the lawyer is only engaged by G0 exit (about 5 Nov). Say that suspicion reporting by any person does not wait for that confirmation.
    - The named euthanasia person at Day 7 needs the means and the licence in place (firearm or captive bolt, poultry method), not only a name.
    - Zoonosis SOP does not mention rabies exposure (bites) where relevant.
    - Litter composting "about 55 C for >=3 days" is the in-vessel figure; windrow systems need longer and turning. The vet or agronomist should set the method.

## Verdict

v3 genuinely fixes the r2 ruminant triage and interim-protection majors. One new MAJOR comes from the poultry threshold fix: as written, routine poultry events, including a single hen death in a small layer flock, trigger a notifiable-suspect response. Everything else is MINOR.

VERDICT: 1 MAJOR remaining
