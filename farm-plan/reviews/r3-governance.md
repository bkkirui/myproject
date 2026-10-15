# R3 Governance / Internal-Control / Employment-Entity-Privacy Review of PLAN.md (v3)

Scope: PLAN.md, Appendix A (thresholds), Appendix B (controls), CHANGELOG.md, checked against r1 and r2 governance findings. Prior items are not re-raised unless the v3 fix failed or opened a new hole.

## Disposition of R2 MAJOR items
- R2-1 representative: partly fixed. Caps, bank notifications, vetting, non-relation and cross-check are in B2. The caps are inconsistent with the rest of the plan and unworkable against the payment cycle (item 2). Not closed.
- R2-2 whitelist and vendor hole: mostly fixed. T3 vendor creation, per-payee caps and the exception-report batch are in B3. The "someone other than the preparer" reconciliation is contradicted in B6 and absent from the small-band core, and the exception report is built by the preparer (item 3). Not closed.
- R2-3 paper versus integrity: fixed in design (PLAN section 7, B7). Residual weaknesses are minors 5 and 6.
- R2-4 emergency envelope: fixed in substance. Aggregate caps, non-payee approver, bank payment and 72-h review are present, and loss is bounded at 3% AOB per year. Operability residue is minor 4.
- R2-5 fraud protocol: fixed in structure (B8). Residue is minors 7 and 8.
- Newly found: the plan builds the control set at G2 (about 10 weeks after G1, so roughly Mar 2027) but changes nothing in the financial control environment before then (item 1).

## MAJOR

1. [MAJOR] No interim financial control package, and no opening independent count, between today and G2.
   - Problem: Every financial control (mandates, direct bank and supplier feeds, owner-only vendor creation, payment release, the entity, the data store) is built at G2 or later. The core list in B10 includes "Day-7 safety pack items" but not the financial core. Gate 0 only collects "bank signatories" in the intake. The Day-7 pack is all animal-health and safety. For about five months (to roughly Mar 2027) the incumbent keeps whatever access he has today. Meanwhile:
     - he is told a manager search has started, and "retention agreement" talks put him on notice that he is being replaced or re-papered;
     - a baseline audit of his own books is under way;
     - the owner is authorising a capped input spend through him in the this-season memo.
   - The plan also has no opening count of livestock, feed, grain, fuel and drugs. The drug inventory is reconciled, but the baseline audit does not say it counts live stock or stores. Later tests ("stock within ±2% of independent count", the cumulative-loss kill trigger, whether a variance began under the old regime or the new one) all need that baseline. Without it a loss in the pilot cannot be attributed, and the incumbent can claim any shortfall predates him.
   - Why it matters: This is the highest-risk window for an absentee owner: an unreviewed controller who knows he is being replaced, with a clean sheet of nothing to reconcile against. R2-L3 fixed the unprotected interval for animal health only. It was not applied to money. The five actions this month do not mention it either.
   - Fix: Add a Day-7 financial pack, mostly free, to the G0 exit:
     - bank mandates reviewed, with the owner (or an interim representative) added; payment release by the owner above a small float, and a freeze on new payees without the owner;
     - bank, supplier and fuel statements redirected to the owner and external accountant;
     - credentials inventory and an access list for all systems;
     - an independent opening count of livestock (against tags and registers), feed, grain, fuel and drugs by someone other than the incumbent, signed by both;
     - the reconciling person for the this-season memo named.
   - Make the legal handling of the incumbent (retention agreement, notice, role change) a lawyer item before the search is visible to him.

2. [MAJOR] The representative and payment-authority rules are mutually inconsistent and do not survive a normal payment cycle.
   - Problem, rule conflicts:
     - B1 says T2 is "owner or representative approves".
     - B2 says the representative releases alone only to T1 per item and 1.5% AOB per 30 days in total, and anything above needs the owner.
     - PLAN section 5 says the representative "acts after 2 h" on the Tier 2 queue.
     - These three cannot all be true. Either the representative approves T2, which B2 forbids, or the owner personally clears every T2 item and the 2-h rule is void.
   - Problem, arithmetic:
     - The weekly batch (payroll, feed, fuel, utilities) is a large share of AOB each month. Payroll alone is typically 20–35% of AOB per year, so roughly 2–3% a month.
     - A representative cap of 1.5% of AOB per 30 days in total cannot release a normal month's batch.
     - So either the owner personally releases every payroll and batch (the time budget does not itemise this, and any travel, illness or signal gap stops pay, which is its own employment-law exposure), or the representative routinely exceeds the cap and the cap is decoration.
   - Why it matters: Two live failure modes: payroll stalls, or the control is silently breached. The plan also gives the representative many other roles: emergency approver, 72-h reviewer of emergency events, recipient of the gate log, leader of the fraud protocol, claims handler, custodian of the "if I am gone" file. Combined with a loose release cap, that is a single point of capture again.
   - Fix: State in one table who releases what:
     - Define "scheduled recurring" payments (payroll, tax, utilities, contracted supply call-offs) as a separate class. The owner pre-approves the amounts each period, and the representative releases them as a pure execution step within the whitelist and per-payee caps, so no discretionary spend passes through the representative.
     - Keep the 1.5% 30-day cap for discretionary, non-scheduled items.
     - Delete one of the T2 statements and align section 5.
     - Name the owner's delegate for a stated number of days of unavailability, and include the cap arithmetic in the section 5 time budget.
     - Separate the representative's roles: the emergency review should not sit with the person who approved the same events.

3. [MAJOR] Preparer independence is claimed in B3 but not delivered, and cannot be afforded in the small-band core.
   - Problem, three conflicts:
     - B3(d) requires reconciliation by someone other than the payment preparer (accountant quarterly or a second bookkeeper). B6 and B10 assign the monthly bank and supplier reconciliation to "the external bookkeeper", the same person who prepares the payments, holds the master files and sends the batch.
     - The "exception report" that makes the batch reviewable is produced by that same preparer. If the preparer mislabels or omits a new payee, a changed amount or an over-cap item, the owner sees a clean report. B3 also says master-data change logs go "straight to the owner", but a log produced from the preparer's own system is not independent.
     - The small-band minimum set is "core only". The core has an external bookkeeper and an annual accountant review but no independent quarterly reconciler. So at small scale the non-preparer reconciliation happens once a year, which is the control R2-2 asked for failing in the band most likely to apply.
   - Why it matters: The bookkeeper is the largest unaddressed insider (payment preparation, master files, ID copies, reconciliation, 24/7 trust). A single outside party who prepares, edits master data, reconciles and reports exceptions to an owner who reads a screen in minutes is the textbook hole R2-2 described.
   - Fix:
     - Generate exception logic in the banking platform (new payee, changed bank details, over-cap, changed amount) or by a second party, not the preparer.
     - Make the owner (or accountant) the holder of the whitelist and payee-change log from the bank.
     - Put a non-preparer reconciliation, at least quarterly, into the core list and the small-band cost (for example the owner's review of direct feeds against the bookkeeper's ledger by an accountant sampling).
     - Resolve the B3/B6/B10 wording to one rule.
     - Add a routine match of vendor bank account, address and phone against the employee master file (a standard forensic test the plan lacks).

## MINOR

4. [MINOR] The emergency envelope has no payment instrument and its fall-through approver is not independent.
   - Problem: The manager may not hold signing rights, cash is excluded, and vendor creation is T3 with a quote record. A 2 a.m. tanker, generator hire or non-whitelisted vet callout therefore cannot be paid under the envelope, so the manager pays personally (a reimbursement channel with no control) or the owner or representative releases anyway, which defeats "act first". The deputy, as fall-through approver, is the manager's subordinate. The 2-h contact log is kept by the manager, so it is self-reported.
   - Fix: Allow commitment now with payment released later on the 72-h review. Add a pre-approved emergency vendor list entered at G2 (vets, water carters, fuel, electricians) and an owner-held capped card or float. Notice to the owner and representative should be sent through the entity system or carrier log, not self-logged. Name an approver outside the manager's line (the vet-of-record cannot be the payee; consider the agronomist or consultant stockman).

5. [MINOR] The no-signal fallback reopens the self-report path, and nobody reviews the raw store routinely.
   - Problem: "SMS count plus paper audited at spot-counts" is manager-editable and unsigned, which is what R2-3 objected to. Offline in-app captures take the device clock unless the app attests it. Unit leads are the manager's subordinates and own the capture, so they can be pressured. Duplicate-image and metadata checks are "at audit", but no one owns daily or weekly review of the raw store, and the coordinator's role and independence are undefined. Completeness at 95% proves submissions exist, not that they are true.
   - Fix: Entity-owned devices (no personal-phone capture), offline capture with queue, signal-recovery sync and a device-clock flag, a named raw-store reviewer independent of the line, and weekly random photo sampling by the reviewer.

6. [MINOR] Vendor KYC and the 3-quote record are supplied by the party being controlled, and seasonal volatility will flood the exception report.
   - Problem: The registration check, quotes and relationship declaration are prepared by the manager or vendor. A real shell with a real registration passes. The +10% on prior-period trigger will fire constantly on seasonal feed and fuel, which produces exception fatigue, the same rubber-stamp outcome.
   - Fix: Independent registry and beneficial-owner lookup by the bookkeeper or accountant, compared with the staff list. Seasonal baselines, or an absolute floor plus the supply-agreement price band, instead of a flat +10%.

7. [MINOR] Spot-count tolerance and the fraud trigger are not coherent.
   - Problem: "Clean" is within ±2% (PLAN section 3, G3). Shrinkage amber is 3% and red is 5% (A2). A failed spot-count starts B8 but is not defined. A count between 2% and 5% is neither clean nor failed. Live counts on extensive stock are often not accurate to ±2%, so a noisy trigger either fires constantly or is ignored. B8 then involves covert steps (securing records first, imaging devices, suspension) on an employee, which carries employment-law and privacy exposure if the trigger was a miscount.
   - Fix: A graded rule: recount by a second team and reconcile known movements within 48 h, then start B8 if the variance persists beyond red. Define "failed" explicitly. Lawyer to confirm that device imaging covers only entity-owned devices.

8. [MINOR] The fraud protocol has gaps if the representative or bookkeeper is the subject, and the whistle-blower route has no destination.
   - Problem: B8 is "led by owner or representative"; the hotline's recipient is not named in B9. A report about the representative, the bookkeeper or the owner's own delegate has nowhere safe to go, and a hotline answered by anyone in the line destroys reporter protection.
   - Fix: The hotline goes to the owner and the lawyer or external auditor, never to the manager, deputy or representative. Add an alternate protocol lead (the lawyer) when the representative is conflicted.

9. [MINOR] The entity and POA mechanics are not aligned with the plan.
   - Problem: Until the entity exists (2–3 months) the owner is personally employer and holder, and the transfer of licences, holding registration, tenure and lender consent can carry tax, stamp duty and non-transferability issues. The plan assumes entity creation is routine. B2 and B9 rely on a personal power of attorney for the representative's second-signature role, but a company bank account is signed under a company mandate or alternate-director resolution, not the owner's personal POA. A manager who runs operations while "never director" may still be a de facto or shadow director or an OHS "officer" in some jurisdictions. A representative with payment authority is exposed the same way.
   - Fix: Make these explicit lawyer scope items: transfer map and cost, entity-level mandate or alternate-director route, de facto director and OHS officer analysis for the manager and representative.

10. [MINOR] Authority limits are set from the incumbent's own history, and the manager search runs before the role is decided.
   - Problem: T1 is sized so that 90% of the last 24 months' purchase lines fall within it. If that history is inflated or fraudulent, the baseline legitimises it. Manager search starts now with wage tests of 3–5 candidates against "the control set" before G1 decides whether there will be a manager, which raises candidate-misrepresentation and data-protection exposure.
   - Fix: Calibrate T1 on audited lines only, or after the baseline books review. Add a lawyer-approved candidate notice (role contingent on G1, data handling) before the search is visible.

11. [MINOR] The small-band control cost cap is probably unreachable, and the pre-G1 spend cap may be too.
   - Problem: Under 250k revenue the cap is about 7% (about 17k at the top of the band). Core items are a bookkeeper, 4+ auditor visits, an annual accountant review, a part-time representative, fidelity premium, amortised legal and entity cost, hotline, GSM alarms, coordinator and a year-1 consultant stockman. My order-of-magnitude estimate, which the accountant should confirm, puts that above the cap for a typical small farm. The pre-G1 cap (about 1.5% of revenue, about 3.75k at 250k) would not cover a lawyer plus a vet-led audit plus a coordinator plus a search. The plan handles this by saying "scale down or lease", which is legitimate, but the owner learns it only after spending.
   - Fix: A one-page feasibility screen at the start of G0: below a revenue band, go straight to the lease or restructure comparison. State in the decision sheet that small farms are likely to fail this screen.

12. [MINOR] The owner-hours budget does not itemise the owner-only tasks the controls added.
   - Problem: Section 5 does not list T3 vendor KYC, exception-report review, call-backs for bank changes, 72-h emergency reviews, the quarterly representative cross-check, and the single owner admin role on the data store (a key-person risk if the owner is unreachable). The owner-hours kill trigger is set at 150% of the phase total, so it can fire on omissions.
   - Fix: Add these as line items in the section 5 table, and name a second admin (the lawyer or the representative under the entity mandate).

VERDICT: 3 MAJOR remaining
