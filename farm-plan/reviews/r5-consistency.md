# Review r5 - Cross-file consistency and animal/crop safety of v5 (integrator, adversarial)

Scope: PLAN.md v5, Appendix A, Appendix B, CHANGELOG.md, against r4-livestock.md and r4-agronomy.md. [MAJOR] = material loss, safety/legal exposure or plan failure. [MINOR] = fix but not fatal. Resolved items are not re-raised. All thresholds are defaults for the vet or agronomist to replace; I judged them for internal consistency and obvious unsafe direction only.

## Checks performed

1. v5 edits, safety and contradictions: poultry thresholds (A2 table, floor row, week-1 row, layer red wording), young-stock group definition, A0.8 interim biosecurity, A0.9 treatment list, interim lead term and dates. No unsafe number found. Week-1 broiler amber 1% cumulative and placeholder red (>1%/day or >2% in 2 days) sit above normal first-week losses. The floors (3/6 birds) are sensible for large flocks. Contradictions are listed below, all MINOR.
2. Dates and weeks: 15 Oct to 17 Dec is 9 weeks and to 29 Jan is 15 weeks, matching "9-15 weeks". G0 (3 wk, to ~5 Nov) plus 12 wk is about 28-29 Jan. 29 Jan plus 18 wk is about 4 Jun, which matches "reference: manager starts Jun 2027". The window memo on day 14 is 29 Oct. Hours rows: 15+68+81+72+59+32+64 = 391, matching "~390 (330-450)", "~83 h to G1" and 390/52 = 7.5 h/week. A3: 2.25x52 + 36 + 32 + 24-48 + 64 = 273-297, matching ~280. B12 arithmetic: 121k vs 98k, headroom 23k, 71k alternative case and 80k land premium are all correct. CHANGELOG Part 1 matches the body for N, S and covered start, except items 2, 3 and 7 below. PLAN word count is 2,241, matching the CHANGELOG's "about 2,240".
3. Cross-references spot-checked (all resolve unless listed under findings): PLAN "Appendix B0", "Appendix A0", "section 3", "section 5", "section 7", "section 8" (window memo, in PLAN), "B10", "B12", "Appendix B section 10", "Appendix B section 8", "A6" and "B2 vetting" (from B0), "A0.3" and "B5 caps" (B0.4; B5 states 1%/1.5%/3%, matching), "starts B8" (A2), "A1" (A2 and B4), "B7" (B11), "A4" (A6), CHANGELOG R4-L4 to A0.9 and R4-L5 to A0.8, R4-G2 to B0.1, R4-G5 to B1/B2, R4-G6 to B3/B9, R4-G9 to B8, R4-G10 to B12, R4-A10 to B10, R4-E1 to B12 (98k vs 121k) and the numbering note (v3 section 9 is now 8; v3 A6 is now A7). That is 24 references. Unresolved: item 6.
4. Defaults statements: Appendix A and B state them clearly. PLAN and CHANGELOG are weaker (items 8 and 9).

## MAJOR

None.

## MINOR

1. [MINOR] Young-stock red points back to the multi-death trigger it was meant to escape.
   Problem: A2 young-stock red says "Standstill only on the A1 step-2 signs". A1 step 2 includes ">=2 deaths in a group within 24-48 h", and "group" is still undefined there (the new definition sits only in the A2 row). Two lamb or calf deaths in one paddock therefore meet both the vet-call red and a step-2 escalation criterion.
   Why: the R4-L3 fix is circular, so the neonatal-peak over-report risk survives on a literal read. Mitigated because the vet or authority, not the manager, escalates.
   Fix: in A1 step 2 apply the criterion to adults, with young stock escalating only on survivor signs (fever, vesicles, neurological signs, bleeding) or no attributable cause, and reuse the A2 group definition.

2. [MINOR] The interim-lead rule is undefined for the S reference start, and G3 then contradicts it.
   Problem: the term is "until the end of the peak in progress at manager start plus a 4-week handover". A S start in Jun-Jul 2027 is in the trough (peak Aug-Feb), so no peak is in progress and the term ends about Aug 2027. The CHANGELOG says the consultant covers the next peak. But the G3 row says "in a peak the interim lead runs it", and the reference pilot (about Oct-Dec) falls in the S peak, after the interim lead has gone.
   Why: the owner could read this as an interim lead through the first S peak when only the consultant is there, and the cost line (1-3%) and A1/A2 evidence both depend on it.
   Fix: add one S sentence: either the interim lead continues to the end of the Aug-Feb peak (cost it), or the new manager runs the first peak with the consultant on call and the pilot is measured on the manager. Make the G3 row agree.

3. [MINOR] Pilot timing: section 3 and the section 5 hours table disagree.
   Problem: section 3 puts G3 "at least 8 wks after G2b ends". Section 5 allots 3+12+18+8+10 = 51 weeks with the pilot following G2b directly (ends about 6 Oct 2027). With the 8-week gap, the pilot starts about late Sep and mostly falls in year 2, so the year-1 pilot row (59 h) does not belong there and routine hours for the gap are missing. Totals stay inside the stated range.
   Fix: add a gap row at routine hours and move the pilot hours to year 2, or reword to "up to 8 wks after G2b".

4. [MINOR] "Deaths above the floor" is ambiguous for the egg-drop report trigger, and it sits at amber level.
   Problem: A1 sends "egg drop >=10% with deaths above the floor" straight to standstill and report. The floor has two values (3 amber, 6 red). Egg drop >=10% is amber by itself, so amber egg drop plus 3 deaths (about 0.06% of a 5,000 house) reports and freezes the farm, while the respiratory trigger is scaled to "deaths at or above amber". Heat, lighting or feed changes cause this routinely.
   Why: it is the one place a husbandry event can still auto-report, which R3-L1 and R4-L2 aimed to remove.
   Fix: state which floor applies (the red value, 6) and match the respiratory wording.

5. [MINOR] The small-flock cumulative leg has no tier or action, and floors cap the week-1 rows for small broods.
   Problem: "vet-set 7-day cumulative leg (default >5%)" in the Floor row names no amber or red outcome. The floor row applies to all flock sizes, including week 1, so a 100-chick brood losing 5 a day (10% in two days) is amber only, because red needs 6 a day.
   Fix: say the leg is amber (vet call within 24 h) and red at a higher value (for example >10% in 7 days, vet-replaceable), and say week-1 red uses the percentage leg for flocks under about 300.

6. [MINOR] Appendix headers cite the wrong PLAN section.
   Problem: both appendix headers say defaults are calibrated at G1/G2 "(PLAN.md section 8)". Section 8 is the window memo; G1 is section 4 and G2 sits in section 3 (also inherited from v4).
   Fix: cite "PLAN.md sections 3-4".

7. [MINOR] The front sheet and the season table disagree on the S fallback date.
   Problem: the front sheet says "plan on Q1 2029". The table says S that waits after a slip gets Q3 2029, later than the plan date. The S-slip branch is where the front sheet could mislead.
   Fix: change the front sheet to "plan on Q1 2029 (Q3 2029 if an S start slips and you wait)".

8. [MINOR] PLAN's defaults disclaimer is narrower than v4's.
   Problem: v4 said "All numbers are defaults"; v5 says "Figures marked ~ or 'default'". Unmarked figures that act as criteria (G3 >=95% and ±2%, 150% kill trigger, 15% margin, stress percentages, 90-day scenario) now fall outside the sentence.
   Fix: restore "All figures are defaults or assumptions unless a source is stated; ~ marks the least certain."

9. [MINOR] CHANGELOG has no statement of its own that the numbers it quotes are defaults.
   Problem: only the last line ("Unresolved by design: all numeric defaults") touches it. The file restates thresholds and caps (for example 0.1% AOB, 5% cap, 15% margin) without any caveat.
   Fix: add one line under the title: "Figures quoted here are the plan's defaults and assumptions, not advice."

10. [MINOR] B12 uses two incompatible margin assumptions.
    Problem: the hurdle example assumes a 250k pre-management margin on 500k (50%), while the cap sentence below it assumes 5-15% net margins (25-75k). The 33-100% cap-versus-margin ratio is true only for the second.
    Fix: state that the cap sentence uses a low-margin farm, or use one margin in both.

11. [MINOR] B0.6 and B2 differ on the incapacity route.
    Problem: B0.6 says personal power of attorney until the entity exists, with a 14-day delegate. B2 says the incapacity route uses the entity mandate "not a personal power of attorney". The until/after timing is only implicit.
    Fix: add "once the entity exists" to B2.

12. [MINOR] Interim float may overrun the owner's queue budget.
    Problem: B0.4 caps the incumbent at 0.1% AOB per item (500 at a 500k AOB) and the owner releases everything above it, while the T1 limit is calibrated only after the books review. Section 5 budgets 2.5-3 routine hours a week and a 30-45 min approval queue.
    Why: for 6-12 weeks nearly all purchases go to the owner, which could breach the queue budget and tempt informal workarounds.
    Fix: state expected volume, or allow scheduled payroll and supply call-offs inside the float from the start.

13. [MINOR] The timeline row mislabels when the packs are finished.
    Problem: "15-22 Oct: Day-7 packs" conflicts with A0.4 (euthanasia means and licence are a G0-exit item) and the vet-led baseline, so the packs finish by about 5 Nov.
    Fix: change the row to "Day-7 packs started; completed at G0 exit".

VERDICT: 0 MAJOR remaining
