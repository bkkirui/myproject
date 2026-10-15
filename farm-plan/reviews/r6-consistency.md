# Review r6 - Final verification of v6 (veterinarian / agronomist / integrator, adversarial)

Scope: PLAN.md v6, Appendix A, Appendix B, CHANGELOG.md, against r5-consistency, r4-livestock, r4-agronomy. [MAJOR] = material loss, safety/legal exposure or plan failure. [MINOR] = fix but not fatal. Resolved items are not re-raised. Thresholds are defaults for the vet or agronomist to replace; I judged them for internal consistency and unsafe direction only.

## Checks performed

1. v6 edits, safety and consistency.
   - Young-stock escalation (A1 step 2 and A2 row): adults escalate on >=2 deaths in a group. Young stock escalate only on survivor signs or no attributable cause. The group definition (same paddock, shed or age cohort) now sits in both places. The r5 circularity is gone. Safe and consistent.
   - Egg-drop trigger (A1): egg drop >=10% with deaths at or above the red floor (6 birds or the percentage, whichever is larger). Husbandry-caused egg drops no longer trigger standstill on their own. Direction is safe. One wording residue is item 2.
   - Small-flock cumulative tiers (A2 floor row): amber >5% in 7 days with a vet call in 24 h; red >10%, which means lockdown and vet triage. Week-1 broods under about 300 use the percentage leg. A 50-bird flock losing 5 a day reaches red through the cumulative leg, so the floor no longer hides small-flock losses. Safe.
   - S interim-lead term: a Jun-Jul S start has no peak in progress. The lead leaves about Aug 2027, the manager runs the Aug-Feb peak with the consultant on call, and G3 says "S: the manager, consultant on call". PLAN section 3, the G3 row and the CHANGELOG now agree. A2 level text (clean quarter with the manager running) fits.
   - Pilot timing against the hours table: section 3 now says "straight after G2b (>=8 wks long)" and the table has no gap. 3+12+18+8+10 = 51 weeks ends about 7 Oct 2027, inside year 1 (to 14 Oct). Resolved.
   - Q3 2029 slip case: it is on the front sheet and in the season table. Jun 2028 start plus 12 months plus a trough leave in Jun-Jul 2029 gives Q3 2029. Consistent.
2. Dates, weeks and hours (recomputed). 15 Oct to 17 Dec is 9.0 weeks. To 29 Jan is 15.1 weeks. G0 to 5 Nov is 3.0 weeks, and the window memo on 29 Oct is day 14. 29 Jan plus 18 weeks is 4 Jun, G2b ends 30 Jul and the pilot ends 8 Oct. Hour rows are 15, 68, 81, 72, 59, 32 and 64, which sum to 391, matching "~390 (330-450)". Hours to G1 are 15+68 = 83. 390/52 = 7.5 h/week. A3 is 273-297, matching ~280. B12 examples were recomputed: -39, 101, 8.25, 134.25, 76.5, the 24.5k margin, break-even 225.5k (45%), pre-G1 cap 22.7% and 10%, and K = 500k. All correct. PLAN has 2,252 words, matching the CHANGELOG's "about 2,250". Front sheet, body, season table and CHANGELOG reconcile on every date and count I checked.
3. Cross-references: 24 spot-checked, all resolve. Renumbered ones: PLAN "section 8" (window memo), "section 7" (sign-off), "section 5" (hours), "section 3-4"; Appendix headers now cite "PLAN.md sections 3-4"; B0.4 (disposal) cited by PLAN; B0.7 (bridge); B0.5 and B6 (G2 exit start, 4 a year, fortnightly in the pilot); A0.3 and B5 caps; A0.8, A0.9, A0.4; B0.6 and B2 ("once the entity exists" present); A2 "starts B8"; B4 to A1; B11 to B7; A6 to A4; B12 role map; B10 and "Appendix B section 10"; CHANGELOG numbering note (v3 section 9 is now 8, v3 A6 is now A7, both true); CHANGELOG R5 items to B10/B12/B0.5; Part 3 (v4 numbering) "PLAN section 8 window memo" and "section 5" hours table. No dangling reference found.
4. Defaults disclaimer: present in PLAN (header: "All figures are defaults or assumptions unless a source is stated ... none is advice") and in CHANGELOG (line 3). Appendix A and B headers also carry it. Resolved.
5. R5 coverage: all 13 R5-C items appear in the CHANGELOG (C12 under "Rejected or modified"). The round-5 MAJOR counts in the CHANGELOG (2 economics, 1 governance, 0 consistency) match the r5 verdict lines.

## MAJOR

None.

## MINOR

1. [MINOR] The S covered-start end date for the interim lead does not follow the stated term.
   Problem: the rule is "end of the peak in progress at manager start plus 4 weeks". The season table gives the S slip as "a covered start with the interim lead to Jan 2028". An S start in the Aug-Feb peak implies a term to about Mar 2028, and S also has a Mar-May peak. The table also gives no earliest A3 for the covered-start slip branch, only for "wait".
   Why: the owner could assume 1-3% interim-lead cost and consultant cover for a shorter or longer period than the rule produces.
   Fix: either change "Jan 2028" to "Mar 2028" or state the S slip rule as a date. Add "A3 about Q4 2028" for the covered-start slip.
2. [MINOR] "Deaths above the floor" in A2 layer red is ambiguous.
   Problem: the A2 layer red cell says "amber egg-drop/intake signs together with deaths above the floor", while A1 uses "the red floor (6)". The floor row has two values (3 and 6).
   Why: red here only means lockdown and a vet call in 2 h, so the risk is small, but a reader could apply 3.
   Fix: write "above the amber floor" in A2 if lockdown at 3 deaths is intended, otherwise "red floor", matching A1.
3. [MINOR] The week-1 rows and the small-flock cumulative leg overlap without a precedence rule.
   Problem: for a brood under about 300, the week-1 row (amber >1% cumulative, red >1%/day or >2% in 2 days) and the cumulative leg (amber >5%, red >10% in 7 days) both apply.
   Why: the week-1 row is stricter, so the safe reading wins, but the text does not say so.
   Fix: add "the stricter applies".
4. [MINOR] B12 Example 1 breaches the one-third-of-OMBM control limit and does not say so.
   Problem: controls are 40k and OMBM 110k, so one-third is 36.7k. Criterion 2 would fail self-run in Example 1 as well as the hurdle. The CHANGELOG says the cap is compared with OMBM in both examples, but B12 shows only the pre-G1 cap ratio.
   Why: harmless to the outcome, since lease ranks first anyway. A reader testing criterion 2 against the example finds an unstated failure.
   Fix: add one clause to the Example 1 result cell: "also fails the one-third limit (40k vs 36.7k)".

VERDICT: 0 MAJOR remaining
