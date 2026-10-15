# R6 Governance / Internal-Control / Legal-Exposure Review (final verification, PLAN v6)

Scope: PLAN.md v6, Appendix B (B0, B5, B6, B12), Appendix A, CHANGELOG.md, checked against r5-governance.md. Resolved items are not re-raised. Nothing here is rated MAJOR unless it risks material loss, legal exposure or plan failure.

## Verification of R5 MAJOR G1 (count gap): FIXED
- Cadence is now dated: opening count (~22 Oct), ~6-8 weeks (3-17 Dec), G1, then **unannounced at least every 3 months until the B6 regime starts**, then a signed handover count at manager start (B0.5; PLAN section 2 agrees).
- B6 start date is stated: the 4-a-year minimum takes effect at G2 exit; fortnightly counts from the pilot (B0.5, B6, G3 exit row). The R5 window of 5-10 months with no count no longer exists; the longest unobserved interval is about 3 months.
- A monthly register roll-forward by the coordinator is added and described as covering off-book sales and removal of stock, feed, fuel and drugs.
- Count scope, counter and cost are stated (R5-11 closed).
- Residue: the quarterly counts close the gap. The roll-forward as written covers less than it claims (item 1). The remaining points are MINOR.

## MAJOR
None.

## MINOR

1. [MINOR] The monthly roll-forward claims coverage its inputs do not provide.
   - Problem: B0.5 lists the inputs as "births, deaths, sales photos against bank receipts". All of these are produced by the person under test. An off-book sale produces no photo and no receipt, so the test cannot see it. Feed, fuel and drugs appear in no input at all. Eggs and milk (carved out of "disposal" in B0.4) are matched to nothing before the B4 benchmarks start at G2.
   - Why: The claim "covers off-book sales and removal of stock, feed, fuel and drugs" is asserted, not built. In practice it is a livestock movement check on lead-supplied data. Real detection of removals rests on the quarterly counts, so the loss window is up to 3 months. That is acceptable, but the monthly signal should not be relied on beyond that.
   - Fix: Name independent inputs. For livestock use the movement register and any traceability or transport records, plus abattoir, saleyard and buyer confirmations. For feed use supplier statements, delivery-note photos and bag counts against issue. For fuel use supplier invoices and the meter. For drugs use vet invoices against the drug register. For eggs and milk use dispatch sheets against the flock's lay rate or herd yield. Each unannounced count re-performs the previous month's roll-forward as a test of the coordinator's work.

2. [MINOR] Count cadence has three small holes.
   - Problem: (a) After G2 exit, B6 gives "minimum 4 a year, randomised" with no maximum interval, which can allow a gap of about 6 months at the point the interim regime ends. (b) Custody changes have no count: only the manager-start handover has one. Exclusion of the incumbent and move to the B0.7 bridge, the bridge's handover to a contract manager, and the interim lead's exit (N covered start, Oct 2027) are not counted, so a variance cannot be dated to a person. (c) "G2 exit" is the trigger date for B6, but PLAN section 3 gives G2 contents and no exit criterion or date.
   - Fix: (a) Add a maximum interval of 4 months in B6. (b) Require a signed count at any change of acting lead, manager or float holder. (c) Add one line defining the G2 exit date as the manager-start-minus-one-week sign-off.

3. [MINOR] Count funding is described as "pre-G1" for counts that fall after G1.
   - Problem: B0.5 and the changelog say count costs sit in the pre-G1 quoted lines beside the lawyer and books review, under the cap. The quarterly counts between G1 and G2 exit (Mar and Jun 2027 at least, and longer on a slipped start) are post-G1. B10 puts spot-counts in control cost, but the interim counts before the auditor exists have no booking rule, and the cost is not shown to be inside the 25k cap or the control-cost band.
   - Fix: Pre-G1 counts sit in the pre-G1 cap. Counts after G1 are booked to control-and-oversight cost (B10 "spot-counts/auditor"), included in the G1 hurdle's set-up and control lines.

4. [MINOR] The B0.7 bridge creates role clashes and unbudgeted exposure.
   - Problem: The consultant stockman as acting lead (a) is also named in B0.1 as a possible counter ("vet or independent stockman"); (b) is named in B5 as a fall-through emergency approver "outside the manager's line", yet now holds the float and runs the line; (c) is not covered by the B9 lawyer scope on de facto director and OHS-officer analysis, nor by who is the licensed holder for the reporting duty (A1); (d) needs the owner or representative on site for 1-2 weeks, about 40-80 h, while PLAN section 5 shows 24 h of site presence for G0 to G1 and the interim representative is view-only.
   - Fix: While the consultant stockman is acting lead, they are excluded as counter and as B5 fall-through (use the agronomist or accountant). Add the acting lead to the lawyer's day-7 brief. Mark the 1-2 week site stint as a contingency in the hours reserve.

5. [MINOR] The "no disposal without written OK" rule still conflicts with plan mechanisms and everyday trade.
   - Problem: (a) The window memo (section 8) decides sale timing and carries staged drought rows with sale ceilings. The stalled-feed rule (B0.6) acts "if the owner is unreachable". B0.4 does not say these are the owner's written OK, so the literal rule forbids what the plan prescribes. (b) The standing OK covers "named routine buyers" only. Routine culls to a new or one-off buyer, on-farm slaughter for staff rations, and scrap of worn machinery have no route. A rule people cannot follow gets ignored (the R5-5 concern).
   - Fix: State in B0.4 that an owner-signed window memo row and a G1 drought plan row are the written OK within their ceilings. Add an item-by-item OK route with a 24-h owner response target for one-off buyers, and name the staff-ration and scrap cases as logged exceptions with a monthly cap.

6. [MINOR] The new-payee freeze blocks emergency payees faster than onboarding can clear them.
   - Problem: B0.2 onboarding targets 5 working days. B5 pays emergency vendors at the 72-h review, and the pre-approved emergency vendor list is "entered at G2". Until then, a water carter, electrician, second vet or authority-appointed contractor needed in a first-month emergency is a new payee that cannot be paid within the B5 timing. The vet-of-record can be onboarded in the first week, but the others cannot.
   - Fix: Onboard a day-7 emergency list (vet-of-record, second practice, water, fuel, electrician) through the B0.2 route in week 1. Add an exception for unlisted emergency payees: the accountant does the registry check inside the 72-h review and the owner approves with call-back.

7. [MINOR] The scheduled class uses a flat +10% test while B3 says seasonal baselines replace it.
   - Problem: B1 returns any schedule over budget line +10% or +10% on the prior period to per-item approval. B3 explicitly replaced the flat +10% with seasonal baselines for the bank's exception rules. In a lambing, planting or harvest peak, casual headcount and wages will exceed +10% on the prior month routinely. Each added casual is also a "new payee needing the owner's approval with ID" (B0.2). Payroll then falls back to per-item approval during the peak, which is the queue the scheduled class was meant to remove (R5-7).
   - Fix: Use last year's payroll by month as the baseline for payroll schedules, with a headcount cap per period from the roster. Allow a pre-approved casual pool (named gang or contractor) onboarded once per season.

8. [MINOR] The incapacity route is thin and the holder is unvetted.
   - Problem: (a) B0.6 and the delegate are limited to T2 powers. The scheduled class needs the owner to pre-approve each period's schedule, and the plan does not say whether the POA holder or delegate may sign it. If the owner is incapacitated, payroll stops after the current period. (b) B2 says beyond 14 days the "entity-level alternate mandate applies", but before the entity exists (G1 to manager start at the earliest) it does not. T3 items such as an emergency destock outside the memo, bank-detail changes and borrowing have no route. (c) B0.6 requires only "a named holder". It does not require the B2 representative vetting, fidelity cover or conflict declaration, so a POA holder can have bank powers without the checks the representative must pass. B9 still lists a power of attorney without limits.
   - Fix: Say that the POA holder or delegate may sign the scheduled-class schedule within the prior approved totals. For T3 items before the entity exists, route them to the lawyer plus the accountant with the will and trust executor named for that interval. Require B2 vetting, fidelity and conflict declaration for any POA holder. Add "limited, per B0.6" to B9.

9. [MINOR] The two lawyer clearances do not say which B0 steps fall under which.
   - Problem: Clearance (a) covers the count, bank and statement changes, credentials inventory and freeze. B0.4 also cuts the incumbent's existing authority to a float, bans sales without OK, mandates goods-received sign-off and changes who approves payroll. These are workplace directives and arguably changes to duties, and the plan assigns them to neither (a) nor (b). If the go is late, the count is not in the list of steps that proceed, so the baseline slips. Quiet contract-manager sourcing in week 1 (B0, PLAN section 3) is also in neither clearance, while the incumbent is the default interim lead and has had no notice.
   - Fix: Tag each B0 step as (a), owner-only (proceeds regardless), or (b). Say what happens to the count if the go is late (owner-only count by the auditor with a witness, no employee-terms change). Put the contract-manager sourcing under the lawyer's day-7 brief explicitly.

10. [MINOR] Role concentration in the interim is real and the role map does not catch it.
    - Problem: The accountant prepares the scheduled-class schedule (B0.4), runs onboarding checks (B0.2), holds the payee log (B3), may be the emergency approver and may co-release with call-back (B0.2). That is the preparer, the payee creator and the releaser in one person, contrary to B3 "the bookkeeper prepares only". The coordinator runs the roll-forward, receives delivery-note photos, gets daily poultry mortality (A0.8), is the raw-store reviewer and may be the emergency approver. B12 caps roles at three "without the owner's sign-off", so the owner can sign this off, but the plan does not list the sign-off or the compensating checks.
    - Fix: Co-release excludes payments to payees the accountant onboarded and schedules the accountant prepared, unless the owner has signed the schedule and the payee in writing. Name the emergency approver as the agronomist or coordinator, never the accountant, when the accountant is the co-releaser. Record the owner's role sign-off in the G0 exit list.

VERDICT: 0 MAJOR remaining
