# Review r4 - Livestock / Poultry Health / Biosecurity (adversarial, round 4)

Scope: PLAN.md v4, Appendix A (thresholds), Appendix B (controls), CHANGELOG.md, against r2-livestock.md and r3-livestock.md. [MAJOR] = material loss, safety/legal exposure or plan failure. [MINOR] = fix but not fatal. Items gated on Gate 0 or on vet/agronomist calibration are not raised unless the written rule is wrong as drafted. Resolved items are not re-raised.

## (a) Were the prior MAJORs genuinely fixed?

- R2-L1 (poultry thresholds do not tier): fixed and stays fixed. Broiler amber 0.2%/day or 2x trailing mean, red 0.5%/day, week-1 cumulative rule, N-bird floors. Figures are plausible against normal broiler (about 0.05-0.1%/day after week 1) and layer (about 0.01-0.03%/day) mortality.
- R2-L2 (single sudden death treated as notifiable): fixed. A1 two-step triage with in-situ photo, tag left on, scavenger exclusion, 2 h vet triage with authority-vet fallback, explicit escalation criteria, "unexplained" until post-mortem, KPI on vet-confirmed cause.
- R2-L3 (unprotected interval): fixed by the Day-7 safety pack as a G0 exit criterion with a vet-led baseline review. Residual gaps are MINOR (items 3, 4, 5).
- R3-L1 (poultry red hair-trigger): fixed. Red is now lockdown plus vet phone triage within 2 h. Report and standstill follow only on named signs or if the vet cannot attribute a cause. The "whichever is smaller" wording is gone, N-bird floors and a doubling floor are in, power and temperature failure is a welfare emergency, and the intake and egg-drop reds are raised to 20% with amber at 10%. See item 1 for two residual wording problems, both MINOR.
- The R3 MINORs I checked (ruminant sign scoping, Day-7 additions, emergency cap carve-outs, medicines under protocol, poultry vet route, vet-only red resets, euthanasia means, rabies, windrow composting, exemption list, late-pregnancy counts) are present as the CHANGELOG claims. I found no CHANGELOG entry that overstates what the files contain.

Labelling of invented numbers: PLAN line 3 and the Appendix A and B headers state that all figures are defaults calibrated by the named professional. A2 repeats "vet/agronomist-calibrated defaults" and reserves red resets to the vet. The decision-sheet cost and hour figures are marked "indicative" and "quotes replace these defaults". I found no number presented as fact that should not be. Two soft spots are in item 12.

## Findings

1. [MINOR] Poultry thresholds: three wording defects remain in A2, none of which fires a report.
   Problem: (i) Layer red includes "or any amber with deaths". Layer mortality amber (>0.05%/day) is itself deaths, so on a literal reading amber mortality is always red and the tier collapses for that signal. It presumably means amber egg-drop or intake signs with deaths. (ii) "Broilers, week 1" gives amber at >1.0% cumulative and red "vet-set", so with no default a catastrophic brooding failure (chilling, omphalitis, aspergillosis) has no red until the vet writes one. A0 item 8 uses the A2 red rule as the interim rule, so on Day 7 it is blank for week-1 chicks. The same gap applies to day-old layer pullets, which have no week-1 carve-out. (iii) The small-flock floor (amber >=3, red >=6 birds per house per day) has no cumulative leg, so a 100-hen flock losing 2 a day for a week (14%) never alerts.
   Why: leading-indicator tiers are the main early warning. Low consequence because red is only lockdown plus a vet call.
   Fix: reword (i) as "amber egg-drop or intake signal together with deaths above the floor"; give week 1 a placeholder red default (for example >1%/day or >2% in 2 days) marked vet-replaceable; add a vet-set 7-day cumulative leg for small flocks.

2. [MINOR] Respiratory signs or egg drop "with deaths" are unscaled as an immediate-report trigger.
   Problem: A1 sends poultry "respiratory signs with deaths" and "egg drop with deaths" straight to standstill and report with no triage. One wheezy bird plus one death, or one hot day, meets that on its face. Infectious bronchitis, ILT, E. coli, ammonia and heat all produce it routinely.
   Why: the relabelling and under-calling risk I rated MAJOR in r3 survives at lower volume. This is the one route by which a husbandry event still auto-reports.
   Fix: scale it ("multiple birds in a house with deaths at or above amber, or egg drop at or above 10% with deaths above the floor"). Keep it as the vet's calibrated default.

3. [MINOR] Young-stock red "(as A1)" reintroduces the multi-death trigger for neonates.
   Problem: A2 young-stock red is ">=2 deaths in a group within 24-48 h (as A1)". A1 step 2 lets that criterion escalate to report and standstill. "Group" is undefined. Two lamb, kid or calf deaths in 24-48 h is routine in a lambing or calving mob (scours, pneumonia, cold snaps, starvation), so red fires daily in the peak. It is the ruminant version of the problem the two-step triage solved for adults.
   Why: the same relabelling risk, concentrated in the birthing peak.
   Fix: define "group" (same paddock, shed or cohort of the same age), exempt neonatal deaths within the first days of life when they are inside the seasonal baseline, and keep young-stock red as "vet call within 2 h". Escalation to standstill then follows the existing step-2 signs (survivors with fever, vesicles or neurological signs, bleeding, no cause).

4. [MINOR] The Day-7 pack has no interim treatment protocol.
   Problem: A3 limits treatment to "manager order within the vet's written protocol only", but those protocols are G1/G2 outputs. Between Day 7 and G2 (months) the incumbent keeps treating on whatever basis he has used. The pack reconciles the drug store and checks withdrawal at sale, but it does not stop new antimicrobial or prescription-only use outside a protocol.
   Why: residue and prescription-legality exposure is real in the interim, and the owner holds the legal risk once signing the pack.
   Fix: add one line to A0: the baseline vet issues a one-page interim treatment list (what the incumbent may give without a call, what needs a call, critical antimicrobials vet-only). It is entered in the drug register with the same no-sale flag.

5. [MINOR] Day-7 poultry interim rules omit biosecurity, and the timing is the Northern autumn.
   Problem: A0 item 8 covers mortality counts, red rule, generator and ventilation. It does not cover wild-bird exclusion, covered feed, no open surface water, a visitor log or checking for any housing order in force. Those sit in A3 "decided at G1" (17 Dec). The decision sheet is dated 15 Oct, which for a N-temperate farm is the start of the main HPAI wild-bird exposure season, and the first auditor and baseline visits arrive in the same weeks.
   Why: the interim gap lies in the highest-risk period for the most total loss. G1 stress already models the notifiable event, so the exposure is bounded.
   Fix: add a one-line interim minimum to A0 item 8 (covered feed, no contact with surface water or wild birds, boots and visitor log, poultry visited last, check of local movement or housing orders). The baseline vet signs it.

6. [MINOR] The notifiable-event stress scenario is poultry-only.
   Problem: PLAN section 4 criterion 1 defines the notifiable event as "full poultry loss, no holding sales 90 days, 6-12 month compensation lag". A ruminant-only farm, or a mixed one, has no FMD, bluetongue or anthrax scenario. Ruminant movement restrictions often run longer than 90 days and a cull has a much larger capital value.
   Why: this is the stress test that sizes the signed loss limit, and for ruminants it is not wrong so much as absent.
   Fix: make the scenario species-appropriate (largest enterprise affected, restriction length from the authority, compensation basis from the vet or lawyer) and leave the figures as defaults.

7. [MINOR] Euthanasia means and licensing cannot be in place by 22 Oct.
   Problem: the timeline table puts the "Day-7 packs" in the 15-22 Oct row, and the intake that identifies the authority and country is itself due 22 Oct. A0 item 4 requires a euthanasia person "with the means and licence in place". Firearm or captive-bolt licensing takes weeks in most places. PLAN section 2 makes the pack a G0 exit criterion (about 5 Nov), so the two statements disagree.
   Why: a hard date nobody can meet encourages a paper tick.
   Fix: state the criterion as G0 exit. For the gap, name an interim on-call route (the vet or a licensed neighbour or contractor) and say that the euthanasia person is a named fallback until the licence is in place.

8. [MINOR] Zoonosis line omits avian influenza worker protection.
   Problem: A3 safety covers abortions, raw milk, pregnant workers and rabies. It has nothing on PPE, symptom monitoring and public-health contact for workers who handle sick or dead poultry, or who cull during a notifiable event. It also has no PPE or handling line for a suspect anthrax carcass during triage step 1 beyond "leave unopened".
   Why: staff safety and employer liability. It is a short addition.
   Fix: add the poultry-outbreak PPE and symptom-reporting line and a "no one touches a suspect carcass" instruction to the zoonosis SOP. Vet and public-health authority set the details.

9. [MINOR] Spot-count tolerance and live-animal counting.
   Problem: G3 exit requires stock within +-2% of the independent count, while A2 shrinkage amber is 3%. Counting extensive mobs with lambs or kids at foot, late-pregnant animals counted in situ without mustering, and births or deaths between visits routinely differs by more than 2%. A tolerance tighter than counting error will produce false fails and a fraud protocol start, or train staff to expect a pass.
   Why: it can stall the pilot, and a false failed count is costly. The B6 recount and known-movement reconciliation soften it.
   Fix: state the tolerance as the count method's error plus reconciled births, deaths and movements, with +-2% as the default only for fully mustered or housed counts.

10. [MINOR] Standstill suspends spot-counts and non-essential audit access, with no compensating check.
    Problem: A6 suspends spot-counts during a standstill. A manager under pressure, or one hiding losses behind a declared event, has an unaudited window of unknown length.
    Why: low probability. The integrity risk is real but small.
    Fix: during a standstill, substitute remote verification (death photos, bank, feed and drug records, vet's own records) and run a catch-up count immediately after release.

11. [MINOR] Cross-section inconsistency on the small-farm cutoff.
    Problem: the decision sheet says base revenue under about 250k probably fails the control-cost test. B10 defines a "Small (<250k)" band with a cap and minimum set, and then says under about 150-200k is expected to fail. These disagree on where the screen sits, and the vet-side consequence is that a small farm may reach the Day-7 safety spend before the economics are screened.
    Why: economics is out of my scope, but this contradiction directly affects whether Day-7 spending is wasted.
    Fix: use one figure in both places, or say the screen is a range.

12. [MINOR] Two soft spots in default labelling.
    Problem: a few numbers sit in the appendix without the word "default" and read as facts: A3 "scanning at 40-60 days" (species-dependent: sheep, goats and cattle differ), "colostrum default 10% of bodyweight within 6 h" is labelled but is a single figure for lambs, kids and calves, and PLAN section 4 "72 h storage" and "85% of rostered hours" appear as pass criteria. The blanket header covers all of them.
    Why: low. A reader of the PLAN body alone sees pass criteria without the caveat.
    Fix: add "default" in the PLAN section 4 criteria line and "species-specific, vet sets" against scanning and colostrum.

## Verdict

v4 genuinely closes the three earlier MAJORs and the round-3 poultry hair-trigger. I found no new unsafe number, no contradiction that would cause a material loss or a legal failure, and no invented figure presented as fact. All remaining issues are wording, scaling or interim-gap items for the baseline vet to settle at Day 7 or G1.

VERDICT: 0 MAJOR remaining
