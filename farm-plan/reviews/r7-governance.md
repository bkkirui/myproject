# R7 Governance / Integrator Review (final audit, PLAN v7)

Scope: PLAN.md v7, Appendix A, Appendix B, CHANGELOG.md, checked against r6-governance.md and r6-consistency.md. Resolved items are not re-raised. [MAJOR] only for material loss, legal exposure, safety or plan failure.

## Verification of the v7 edits

| v7 edit | Result |
|---|---|
| Independent roll-forward inputs (B0.5) | Fixed. Livestock, feed, fuel, drugs, eggs and milk each have a third-party input. Photos are secondary. The count re-performs the prior month. The text no longer relies on the monthly signal beyond the quarterly counts |
| Max interval and custody-change counts | Present in B0.5 and PLAN section 2. B6 itself does not carry the maximum (minor 1) |
| G2 exit definition | Defined in B0.5 (manager start minus one week). PLAN section 3 does not define it, but section 2 and B0.5 agree (minor 1) |
| Bridge-lead limits (B0.7) | Present. One residual clash with B0.2 (minor 3) |
| Disposal carve-outs (B0.4) | Workable. Two holes (minor 4) |
| Emergency payee list | Present in B0.2. B5 still says the list is "entered at G2" (minor 5) |
| Payroll baseline class (B1) | Present. Baseline-contamination point (minor 6) |
| POA and T3 routes (B0.6, B2, B9) | Present. Residual concentration (minor 7) |
| Clearance (a)/(b) tags | Mostly done. The claim "every step is tagged" is overstated (minor 2) |
| S slip dates | "Mar 2028, A3 ~Q4 2028" is consistent with the rule. A start Sep 2027 to Jan 2028 gives A3 in Q3 2028 to Q1 2029, so "about Q4" is a midpoint, not an error |
| Layer red floor | A1 and A2 both say "red floor (6 or the percentage)". Consistent |
| "Stricter applies" | Present in A2 |
| Example 1 one-third limit | Present: 40k vs 36.7k |

## Recomputed dates, hours and money (all agree)
- 15 Oct plus 3 weeks is 5 Nov. Plus 9 weeks is 17 Dec. Plus 51 weeks is about 7 Oct 2027, inside year 1.
- Opening count 22 Oct plus 6 to 8 weeks is 3 to 17 Dec. G1 is 17 Dec, so the ~6-8-week count and the G1 count coincide (see note below).
- 29 Jan 2027 plus 18 weeks is 4 Jun. G2b ends 30 Jul. The pilot ends 8 Oct.
- Hours: 15+68+81+72+59+32+64 = 391, matching ~390. Hours to G1 are 83. A3 is 273 to 297, matching ~280.
- B12: -39, 101, 8.25, 134.25, 76.5, 24.5k margin, break-even 225.5k (45%) and 582.5k, pre-G1 cap 22.7% and 10%. All correct.
- PLAN word count is 2,258, against the CHANGELOG's "about 2,260".
- The CHANGELOG round-6 counts (1 MAJOR economics, 0 governance, 0 consistency) match the r6 verdict lines.

## Cross-references spot-checked (28, all resolve)
PLAN to Appendix A0, B0, B0.4, B0.7, B6, B8, B10, B12 and "section 3-8". B0 header to B0.4, B0.3, B0.6 and B0.7. B0.1 to A6. B0.2 to B2 and B3. B0.4 to B1, B3, B5 and A0.3. B0.5 to B6, B10 and B12. B0.6 to B2. B1 to B3. B4 to A1. B11 to B7. B12 to B10. A0.8 to A2. A1 to A2. A2 to A1 and B8. A4 to A0.8. Appendix headers to "PLAN.md sections 3-4". CHANGELOG numbering note (v3 "section 9" is now 8; "A6" is now A7). No dangling reference found.

## Defaults disclaimer
Intact. PLAN header: "All figures are defaults or assumptions unless a source is stated ... none is advice". Present in CHANGELOG line 3, in the Appendix A and B headers, and in the B12 heading ("illustrative assumptions, not forecasts").

## MAJOR
None. Each point below is bounded by the quarterly unannounced counts, the owner's signature on every payee and schedule, and the lawyer-led B8 route.

## MINOR (fix if time permits; none blocks the decision)

1. [MINOR] The count rule is stated in three places with slightly different wording.
   - PLAN section 2 says "at least quarterly (maximum 4 months) until B6 starts". B0.5 says "at least every 3 months" until B6 starts and puts the 4-month maximum on the B6 regime. B6 itself says only "minimum 4 a year" and never states the maximum interval.
   - PLAN section 3 still gives no G2 exit definition. B0.5 is the only place.
   - Fix: add "maximum interval 4 months" to B6 and one line "G2 exit = manager start minus one week" to the PLAN section 3 G2 row.

2. [MINOR] "Every step is tagged" (B0 header, CHANGELOG R6-G9) is not literally true.
   - B0.3 (vendor vs employee master match, payroll muster vs headcount) processes staff data. It has no tag, though the lawyer's day-7 brief covers its lawful basis and notice. B0.2 onboarding and B0.6 POA are also untagged.
   - Sourcing is listed under (b) at G0 exit (~5 Nov) but also "named in the day-7 brief", while PLAN section 3 says quiet lawyer-led contract-manager sourcing starts in week 1 and the table says the manager search begins only after clearance. The reader must infer that week-1 quiet sourcing is lawyer-led and the open search waits for (b).
   - Fix: tag B0.3 as "(a), or owner-only desk match on vendor files until the go". Say "week 1 quiet sourcing under the brief; open search at (b)".

3. [MINOR] B0.7 and B0.2 disagree about the fall-through approver.
   - B0.7 says "the agronomist or accountant is used instead". B0.2 says that when the accountant co-releases, the emergency approver is the agronomist or coordinator, never the accountant.
   - Fix: B0.7 should read "agronomist or coordinator (accountant only if not co-releasing)".

4. [MINOR] The disposal carve-outs leave two soft spots.
   - "Monthly cap" for staff rations and machinery scrap has no figure or setter. Scrap of machinery is a classic quiet-removal channel.
   - Fallen-stock and welfare-euthanasia carve-outs lean on death evidence (timestamped tagged photo, B4). B4 is not stated to apply from day 7, and A1 covers only ruminant sudden death.
   - "Daily egg or milk dispatch to those buyers" implies dispatch to other buyers needs item-by-item OK.
   - After G2, B1 lists "disposals" as T3, which read literally covers every routine sale. No post-G2 equivalent of the standing OK is stated.
   - Fix: the owner sets the cap in money at G0 (default a small share of the float). State that the B4 death-evidence rule applies from day 7. State that routine post-G2 sales run under an owner-signed standing OK renewed at G2.

5. [MINOR] The emergency payee list has two dates.
   - B0.2 onboards a day-7 list in week 1. B5 says the pre-approved list is "entered at G2". They are compatible only if B5 means the full list.
   - Fix: B5 should say "extends the B0.2 day-7 list at G2".

6. [MINOR] The payroll baseline and casual pool can inherit a contaminated or opaque base.
   - Last year's payroll by month is the baseline. If a ghost employee exists, the B0.3 test finds it, but the baseline is not stated as restated for findings or wage changes.
   - A gang or contractor pool hides headcount behind one payee. B4 day sheets and muster are the only check.
   - Fix: "baseline restated for B0.3 findings and award changes; pool payments require countersigned day sheets and a muster sample in each count".

7. [MINOR] Accountant concentration persists.
   - The co-release exclusion and the owner's signature on every payee (T3) and schedule make the exclusion mostly vacuous. The accountant still prepares, runs the registry check, holds the payee log and co-releases.
   - If the owner is incapacitated, the owner cannot sign, so no one can release accountant-onboarded payees. Meanwhile T3 goes to the lawyer plus the accountant.
   - The residual risk is accepted by PI/fidelity cover, the different-firm reconciler and the role-map sign-off. Fix: name a third counter-signer (the executor or the vetted POA holder) for T3 during incapacity.

8. [MINOR] Small timing and hours notes.
   - The ~6-8-week count (3-17 Dec) and the G1 count (17 Dec, or 29 Jan on the plan date) coincide or nearly coincide. Say one count may serve both if within 2 weeks.
   - The 24-h one-off-buyer OK route and monthly schedule signing add owner minutes. Note them inside the 2.5 h/week routine line.

VERDICT: 0 MAJOR remaining
