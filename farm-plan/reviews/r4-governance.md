# R4 Governance / Internal-Control / Employment-Entity-Privacy Review of PLAN.md (v4)

Scope: PLAN.md, Appendix A, Appendix B, CHANGELOG.md, checked against r2 and r3 governance findings. Items resolved in v4 are not re-raised. Things properly gated on lawyer or insurer sign-off are not rated MAJOR.

## Disposition of R3 MAJOR items
- R3-1 interim financial controls and opening count: the pack exists (B0, PLAN section 2) and is cheap and well aimed. It stops at Day 7, though. Nothing recurs between the opening count (Oct 2026) and the pilot (roughly Aug 2027). See item 1. Mostly fixed, one residual MAJOR.
- R3-2 representative / T2 / scheduled class: fixed. B1, B2, B5 and PLAN section 5 now say the same thing (T2 owner-approved; representative only after 48 h silence, discretionary, within 1.5% AOB per 30 days; the 2-h window is for emergencies only; the approver does not review their own emergency event). Residue is minors 4 and 5.
- R3-3 non-preparer reconciliation: fixed across B3, B6, B10, the small-band cost and the PLAN permanent minimum. Residue is minors 6 and 7.
- R3-1 incumbent handling: lawyer-gated and adequate in structure. Residue is sequencing (minor 3) and the interim-lead circularity (minor 8).
- Hours table re-added: rows sum to 391 h and the weeks sum to 51. No error found.

## MAJOR

1. [MAJOR] The interim period (Day 7 to the pilot, about 8–10 months) has one count, no recurring detection, and no rules for authority, stock-out or receipts.
   - Problem: B0 and A0 are point-in-time. Everything recurring is built at G2 or later: the tiers, three-way match, receiver, gate pass, auditor appointment, spot-counts (the 4-a-year minimum and the fortnightly pilot cadence are not dated for the interim), the payroll master file and the vendor/employee match. The person running the farm throughout is the incumbent or a contract interim lead, and there is no manager until Jun–Nov 2027. Specific gaps:
     - **Count.** The one opening count is never matched by a second one. No interim spot-count is scheduled before G3, and no signed handover count is required at manager start. A loss between Oct and the pilot cannot be attributed to anyone. The G3 test ("within ±2% of independent count") and the cumulative-loss kill trigger then start from a stale baseline. Interim livestock theft or off-book sales by an outgoing incumbent go undetected for months.
     - **Existing payees and payroll.** The freeze covers new payees only. Existing vendors (including any shell the incumbent already set up) and the payroll keep paying. The owner releases above a float, but no three-way match, receiver or goods-received note exists until G2. The vendor-bank vs employee-master match and a payroll headcount muster are not in the baseline books review. A ghost employee or related-party vendor survives the whole window.
     - **Interim authority is undefined.** "Small float" has no number. The A0.3 emergency-spend letter has no cap, no approver and no non-payee rule (B5 applies only after G2). The incumbent's ordering rights, and who receives goods, are unstated. The owner would be releasing invoices that the person ordering them has also received.
     - **Stock-out and cash-in side is untouched.** B0 controls money going out. Disposals, livestock and crop sales, cash sales and buyer payment routing are all controlled by the T3 and B4 rules that start at G2. A0.6 gives a dispatch record but no owner approval of disposals.
   - Why it matters: R3-1 identified this window as the highest-risk period for an absentee owner (an unreviewed controller who knows he is being replaced). The pack closes the door on new payees and on blind statements, but the same person has eight more months of unmatched purchasing, sales and stock, plus an emergency letter with no ceiling. It is cheap to fix and the exposure is the farm's main asset.
   - Fix (all low-cost):
     - Add an interim count schedule: an auditor or accountant spot-count at about 6–8 weeks, again at about G1, and a signed handover count at manager start. Fortnightly spot-counts apply only from the pilot.
     - Run the vendor-bank vs employee-master match, a payroll muster against the headcount and an existing-payee review inside the baseline books review.
     - State interim authority in two lines: no disposal or sale without the owner's written OK, buyers pay direct into the farm account, and a goods-received sign-off by someone other than the orderer (the coordinator or the unit lead) until G2. Put a number on the float and give the A0.3 letter the B5 default cap and the non-payee approver rule.

## MINOR

2. [MINOR] The opening count is under-specified and may collide with the season.
   - Problem: Nobody is named to carry it out, and the cost is not itemised. "Signed by both" has no dispute route if the incumbent refuses or disputes. The count falls in the S-hemisphere lambing/calving peak, so numbers move daily and A6's in-situ rule for late-pregnant stock applies. A point-in-time number needs a roll-forward to the register.
   - Fix: Name the counter (accountant plus vet or an independent stockman), allow "signed, disputed items listed", and require reconciliation to the register on the count date.

3. [MINOR] Day-7 sequencing can tip off the incumbent and run ahead of the lawyer.
   - Problem: Mandate changes and statement redirects (items 1 and 2) are visible in week 1. The lawyer clears incumbent handling only by G0 exit (~5 Nov), and B0.6 "lawyer first" is the sixth item. The count is not stated to precede or coincide with the access changes. Changing an employee's authority and redirecting statements without legal clearance carries constructive-dismissal and privacy risk (gated on the lawyer). Tipping the incumbent before the count gives him a window to tidy stock.
   - Fix: Order the pack: lawyer brief, then count and access changes the same day, then notices.

4. [MINOR] An interim representative can be given release power before vetting.
   - Problem: B0 allows an "interim representative" to be added to the mandate in 7 days. B2 requires vetting, conflict declaration, fidelity cover and non-relation, which cannot be done in a week. The entity does not exist, so the mandate is on the owner's account.
   - Fix: Until B2 vetting and fidelity cover are done, the interim representative holds view and call-back rights only. The owner (or accountant co-release with call-back) is the sole releaser.

5. [MINOR] Delegate and scheduled-class edges.
   - Problem:
     - The "delegate for 14 days" has undefined powers. If the delegate is the representative, the 1.5% cap and the T3-owner-only rule are bypassed. If not, a second unvetted person holds owner powers.
     - Before the entity exists there is no "alternate mandate"; B2 excludes the personal POA, but until G2 the POA is the only incapacity route.
     - Scheduled payments have no aggregate cap (payroll, tax, utilities and call-offs are most of AOB), so the safeguard is the owner's pre-approval. The owner cannot verify a payroll schedule from the bookkeeper. Call-offs are double-listed: T1 (manager approves) and the scheduled class (owner pre-approves).
   - Fix: Delegate has T2-level powers only, never T3. State POA as the interim incapacity route. The accountant prepares the schedule with a headcount and prior-period diff for the owner to sign. Pick one route per call-off.

6. [MINOR] Independence of the "non-preparer" is not specified as a different firm.
   - Problem: B3 says "the accountant or a second bookkeeper". Small farms commonly use one firm for bookkeeping and accounting. The accountant also holds the whitelist log, does registry lookups, is the named memo reconciler, receives every statement, designs controls (section 7) and performs the annual review. That is self-review plus a single point of capture, and the accountant has no fidelity cover in B9.
   - Fix: Require a different firm (or at least a different individual with separate engagement terms) for quarterly reconciliation and for the annual review, and add fidelity or professional-indemnity confirmation for the accountant.

7. [MINOR] "Audit" is used inconsistently.
   - Problem: PLAN permanent minimum says "annual external audit". B6 and B10 cost an "annual licensed-accountant review with confirmations". A statutory audit costs materially more, and the small-band cap assumes the review.
   - Fix: Pick one term and state which jurisdictions require a statutory audit (lawyer, accountant).

8. [MINOR] Interim-lead selection is circular on the dates given.
   - Problem: G0 exit requires a named interim lead. The incumbent qualifies only if the baseline finds no related-party or unreconciled-stock issue, and a single count cannot show an "unreconciled stock" history in 3 weeks. If the baseline fails him, the fallback is a contract manager with a 6–10 week lead time, whose sourcing cannot visibly start until the lawyer clears the candidate notice. Operations then stay with the excluded incumbent in the peak, or the farm is unmanaged.
   - Fix: Define the test (materiality and evidence), start contract-manager sourcing quietly through the lawyer in week 1, and state that the incumbent is the interim lead by default under the item 1 interim rules unless a defined finding is made.

9. [MINOR] The B8 trigger wording is contradictory and can delay fraud response.
   - Problem: B8 lists four triggers (failed count, variance above red, hotline report, bank anomaly) but then says a trigger starts the protocol "once a variance persists beyond red after the 48-h recount". Read literally, a hotline report or a bank anomaly waits for a stock variance. The 48-h recount also gives time for borrowed or moved animals to appear.
   - Fix: The recount rule applies to count variances only. A hotline report or bank anomaly starts the 24-h secure step at once. Recount on the same visit or within 24 h with the gate controlled.

10. [MINOR] Role concentration on the representative, and many named roles for a 3–6 person farm.
    - Problem: One part-time steward (inside a ~7% cap) is T2 backstop, scheduled-payment releaser, emergency approver or reviewer, gate-log recipient, spot-checker of deliveries, dead-man's-switch recipient, second admin, claims handler, fraud lead and custodian of the "if I am gone" file. The farm also has a coordinator, Farm Model owner, interim lead, reconciler, raw-store reviewer, deputy, delegate, consultant stockman and hotline recipient. At small scale these are weeks of coordination and capture risk.
    - Fix: Publish a one-page role map with one name per role, a maximum of three roles per person without the owner's sign-off, and merge the coordinator, raw-store reviewer and reconciler into one independent role where possible (not the representative).

11. [MINOR] The feasibility screen threshold is inconsistent and arbitrary.
    - Problem: The decision sheet says revenue under ~250k probably fails. B10 says under ~150–200k is expected to fail, yet defines a small band below 250k. A revenue line ignores margin. A 400k farm with a 10% margin cannot carry a manager, deputy and 7–8% controls either.
    - Fix: Make the day 1–3 screen margin-based (management plus control cost vs the pre-management gross margin, the same one-third test as G1) and align the numbers in the decision sheet and B10.

12. [MINOR] Pre-G1 cost default is thin for the scope listed.
    - Problem: 2–4% of revenue (for example 5–10k at 250k) must cover lawyer scope (incumbent, entity transfer map, candidate notice, emergency letter), vet baseline, books review, opening count, agronomist, nutritionist, hydrogeologist, Farm Model owner and coordinator. The cap (5%) is also below the stated maximum of 2–4% plus 1–3%.
    - Fix: Say quotes replace the default in the decision sheet (done in part) and show the lawyer and books-review lines separately so the owner can see that the cap will probably be reached at small scale. The owner should know this before approving the pack.

VERDICT: 1 MAJOR remaining
