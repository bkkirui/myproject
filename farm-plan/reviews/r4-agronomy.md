# Review R4: Agronomy and Farm Systems Integration (adversarial, round 4)

Scope: PLAN.md v4, Appendix A, Appendix B, CHANGELOG.md, checked against r2-agronomy.md and r3-agronomy.md. Today is 2026-10-15. Gate-0-gated items are not major. Resolved items are not re-raised.

## Status of the prior MAJORs

| Prior | Verdict | Note |
|---|---|---|
| R3-A1 troughs, start dates by hemisphere | Fixed | One table (section 3) is the source. Troughs (N Nov-Jan, S Jun-Jul) match the A3 leave rule, B11 and the changelog. Start and A3 dates are consistent across the front sheet, body and changelog (S Jun-Jul 2027 / Q3 2028; N Nov 2027 / Q1 2029; N covered Jun 2027 / Q3 2028). Residual wrinkles are items 1-3. |
| R3-A2 window memo and spend cap | Fixed | Agronomist and interim lead are in the five actions. The cap is a rule (lesser of owner figure and last year's spend for that window). It sits outside the pre-G1 cap, and shrinkage counts to the loss limit. Interim payment controls, a named reconciler and a rolling refresh (next 1 Dec) are present. Residual gaps are item 6. |
| R3-A3 Farm Model owner and funding | Fixed | The owner is named at G0 with hours and fee. Pre-G1 cost covers agronomist, nutritionist/vet and hydrogeologist input. Section 7 has the signers. A conditional pass makes the manager offer probation-length. Post-G1 upkeep is a MINOR (item 10). |
| R2-A3 drought | Fixed | Leading triggers, 90-day projected feed-days red, irrigation demand, and staged rows pre-authorised in the G1 drought plan. Pre-G1 gap is a MINOR (item 11). |
| R2-A4 feed, litter, medicated flows | Fixed | A4 is adequate and ionophore/copper separation is in A0.7. The operator is not yet in post (item 7). |

Dates checked: 15 Oct to 17 Dec is 9 weeks, to 29 Jan is 15 weeks. The G0 exit of ~5 Nov plus 12 weeks reaches 29 Jan. The year-1 hours rows sum to 391. The A3 hours sum to 273-297, so ~280 holds. The window memo falls on day 14, which is 29 Oct. Cost example: 2-4% of 500k is 10-20k, plus 1-3% is 5-15k, cap 25k. Defaults are labelled globally (PLAN line 3, Appendix A and B headers). No unlabelled invented figure is material.

## MAJOR

None. No remaining item causes material loss, legal exposure or plan failure on its own.

## MINOR

1. [MINOR] Interim-lead term is ambiguous for the N covered start, by up to a year.
   - Problem: Section 3 defines the term as "until the manager has completed one full peak after start plus a 4-week handover". The N covered start (Jun 2027) puts the manager mid-peak (Mar-Sep), so the first full peak is 2028 and the term would run to Oct 2028. The season table says "interim lead through Oct" (2027). The S case is clean (peak Aug-Dec, term ends about Jan 2028).
   - Why: It changes interim-lead cost by roughly 12 months and contradicts "earliest A3 Q3 2028 (covered)", since the interim lead would still be in post.
   - Fix: State one rule for the N covered start (for example: the interim lead leaves Oct 2027 and the consultant stockman/agronomist covers the 2028 peak), or restate the term and the A3 date.

2. [MINOR] The S column has no slip rule, and its peak list contradicts its own rows.
   - Problem: (a) A S start of Jun-Jul 2027 needs near-fastest recruitment (search from ~5 Nov, offer after 29 Jan, 3-6 months, plus candidate notice). A slip of 4-6 weeks puts the start in the Aug-Dec peak. Only the N column has a covered-start fallback, and "plan on Q1 2029" is not tied to S. (b) The S "Peaks" row omits Dec-Feb, yet the Dec-Feb row lists hay, weaning and dry-season stocking, and A5 says hay is made "in the labour-peak season". The main S winter-cereal harvest (Nov-Jan) is not listed.
   - Why: The owner reads Jan-Feb as free time, and the S leave and start windows (Jun-Jul only) are the single narrowest in the plan.
   - Fix: Add an S slip rule (covered start with the interim lead to Jan 2028, or wait for Jun 2028 with A3 about Q3 2029). Add Dec-Feb hay, weaning and harvest to the S peak row.

3. [MINOR] Section 3 and section 5 disagree on G2 length, and the reference-path pilot runs in a peak.
   - Problem: Section 3 says G2 is G1 + ~10-15 weeks. Section 5 allots 18 weeks (29 Jan + 18 weeks is about 4 Jun, the manager start). The pilot (Aug-Oct 2027) falls in the S Aug-Dec peak and the N Mar-Sep peak tail, so under the plan's own rule the interim lead runs it. G3 then proves the interim lead rather than the manager, and A1/A2 are earned on that. "Field test waits for the next trough" cannot work for lambing or planting SOPs, because nothing is being born or planted in a trough. "≥8 wks after G2b" is ambiguous.
   - Fix: Say G2 ends at manager start (the 18-week row spans G1 to start). Say who G3 measures and that the A3 clock starts at manager start. Field-test seasonal SOPs at their next in-season occurrence with the consultant on call. Reword the G2b/G3 gap.

4. [MINOR] The interim lead is "named" in October, but the incumbent's eligibility is decided at G0 exit (~5 Nov).
   - Problem: Action (3) says name the interim lead this month. Section 3 lets the incumbent serve only if the baseline audit finds no related-party or unreconciled-stock issue. A contract manager takes 6-10 weeks and is "sourced before G1". If the incumbent is disqualified, the replacement arrives mid-Dec to mid-Jan, inside the S lambing/planting peak and the N winter.
   - Fix: Make the October naming provisional. Start sourcing a standby contract manager now, and price it in the 1-3% line.

5. [MINOR] The interim lead's cost is classified twice.
   - Problem: It is "management cost" (section 3, B10 exclusion) and also a one-off set-up cost amortised in the G1 hurdle (section 4). It is also the 1-3% pre-G1 line on the decision sheet.
   - Fix: One sentence saying which part sits where (pre-G1 spend is a one-off, post-G1 pay is management cost), so the hurdle does not double-count it.

6. [MINOR] The window memo has four gaps.
   - Problem: (a) The cap anchors on "last year's input spend", which comes from books that are under audit. (b) The memo lists restocking and long contracts as irreversible acts, but the cap covers only "input spend". (c) Livestock sales and breeding decisions (tupping, weaning, sale timing) are not named. (d) The agronomist is not required to be independent of input retailers, who are the usual source of padded orders.
   - Fix: Make the cap the lesser of the owner figure, last year's audited spend and the agronomist's quantity. Extend it to stock purchases and sales. Require a conflict declaration from the agronomist.

7. [MINOR] The A4 operator does not exist until the manager starts.
   - Problem: A4 is "operated by the manager" (Jun 2027 at the earliest, or Nov 2027 in the N case). The ionophore/copper separation sits under A0.7, which is a ruminant live-season item. The poultry item A0.8 has no feed-flow or litter rule.
   - Fix: Name the interim lead as A4 operator until the manager starts. Add to A0.8: no litter on sheep pasture or in feed, and medicated feed kept off shared equipment.

8. [MINOR] Tropics and other climates have no dates and no G0 exit item.
   - Problem: Section 3 says the agronomist builds the calendar "at G0", but G0 exit does not require it. The dated path, trough rules and A3 date are undefined there.
   - Fix: Add "season calendar for non-temperate sites" to the G0 exit list.

9. [MINOR] The feasibility screen and B10 use different small-farm thresholds.
   - Problem: The decision sheet says under ~250k "probably fails". B10 says under ~150-200k "is expected to fail", while its small band (<250k) has a ~7% cap.
   - Fix: One threshold, or say 150-250k is the grey zone that goes to the restructure comparison.

10. [MINOR] Farm Model upkeep after G1 is not funded or timed.
    - Problem: The re-confirmations (first harvest, dry season, birthing season) all fall after G1. B10's numerator, the section 5 hours and the post-G1 budget do not list the model owner. The owner's qualification is unspecified.
    - Fix: Add model upkeep (hours and fee) to B10 and name who may hold the role (for example the coordinator with agronomist co-sign).

11. [MINOR] Pre-G1 drought responses depend on the owner.
    - Problem: Staged sale rows are pre-authorised only in the G1-signed plan (29 Jan). The S Dec-Feb dry season and the N winter-feed decision fall before that. The window memo supplies season-points but no authority.
    - Fix: Let the owner-approved window memo carry interim staged rows with sale ceilings.

12. [MINOR] A2 poultry floors are discontinuous at about 1,000 birds, and chemical/nutrient regulation is missing.
    - Problem: A flock of 999 reds at 6 birds/day. A flock of 1,000 reds at 1 bird/day (0.1%). A4/A5 and section 7 name chemicals and nutrient budgets but not applicator licensing, restricted-use chemicals or statutory manure/nutrient limits.
    - Fix: Make the floor scale (for example the larger of N birds and the percentage). Add a regulatory-compliance line to the agronomist/lawyer sign-off.

13. [MINOR] The changelog's older parts use stale section numbers.
    - Problem: Part 2 says "PLAN = PLAN.md" but cites v3 numbering (section 9 for the memo, now 8; section 8 sign-off rows, now 7; WP4; "A6" for the model tags, now A7).
    - Fix: Add a line saying Part 2 uses v3 numbering, or update the references.

VERDICT: 0 MAJOR remaining
