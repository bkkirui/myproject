# Appendix B: Authority, controls and fraud response (design defaults)

**Not for approval now.** Calibrated at G1/G2 with the lawyer and accountant (PLAN.md section 8). AOB = annual operating budget. All numbers are defaults.

## B1. Authority tiers

| Tier | Who | Limit |
|---|---|---|
| T0 | Unit lead | <=0.05% AOB per item, 0.2% per 30 days |
| T1 | Manager | Set at G0 so >=90% of the last 24 months' purchase lines fall within it (starting proposal 0.3% AOB); <=1.5% AOB per 30 days per supplier/category; within budget line. Call-offs under a **pre-approved annual supply agreement** (price band, quantity cap, owner-approved) count as T1 |
| T2 | Manager proposes; owner or representative approves | Above T1, budget overrun, contracts <12 months |
| T3 | Owner only | Capital, disposals, borrowing, contracts >=12 months, hire/fire/pay of manager, deputy and representative, related-party deals, insurance settlements, **all vendor creation and whitelist entry**, bank-detail changes (call-back to a known number) |
| Emergency | Manager acts first | See B5 |

Anti-splitting is tested at audit. The charter includes the **"manager cannot" list** (release payments, hold bank signing rights, be sole recorder of stock, sole source of dashboard data, sole price contact with buyers), **compulsory 10-working-day consecutive leave** for manager and bookkeeper with the books reviewed meanwhile, and annual rotation of at least one unit lead.

## B2. Owner's representative
Releases alone only up to T1 per item and 1.5% AOB per 30 days in total. Anything above, any T3 item and any bank-detail change needs the owner; the representative is the second signature only under the power-of-attorney incapacity route. The bank sends every release over a threshold and every mandate change to both mandate holders and the external accountant. The representative is vetted like the manager, signs the conflict declaration and code of conduct, is covered by fidelity cover, may not be related to the manager, deputy or any supplier, and has their own payments and approvals reported in the quarterly cross-check. A paid steward is contracted by the entity with notice and independence terms (lawyer); cost sits inside the cap.

## B3. Payments, vendors and whitelist
Requester (unit lead), approver (manager), receiver (a different person, goods-received note with count), payer (owner or representative releases; the bookkeeper prepares only). Three-way match. **Vendor creation is T3:** business registration or ID check, bank account in the vendor's own name, relationship declaration, 3-quote record. Whitelist entries carry a fixed purpose and a **per-payee monthly cap**. New payees, changed amounts (+10% on prior period), bank-detail changes, over-cap and match failures drop out of the weekly batch to per-item approval. The batch screen is an **exception report**, not a list; payroll ties to the master file and muster. Reconciliation is done by someone other than the payment preparer (the annual-audit accountant quarterly, or a second bookkeeper); master-data change logs go straight to the owner; bank daily limit equals the largest plausible batch. Owner credentials: app or hardware MFA; no approvals from messages or links; a "payment instruction from the owner" received by the bookkeeper is void unless in the banking system or confirmed by call-back.

**Small-staff compensating controls** (farms of 3–6 people where a separate receiver does not exist): supplier delivery note signed by the driver, calibrated bag count or weighbridge photo, representative spot-checks of deliveries, auditor samples goods-received notes.

## B4. Cash, stock, payroll, procurement, incentives
- **Cash:** buyers pay direct to farm account; unavoidable cash uses serialised receipts, two-person count, banking within 48 h; statements go to owner and external accountant; imprest petty cash with hard cap and weekly count by a non-custodian.
- **Stock:** monthly signed reconciliation; each death evidenced by timestamped photo (suspect deaths in situ, A1), witness above a value threshold, logged disposal; gate pass and two-person load-out; two-key drug store; feed by calibrated count at receipt and issue. Variance 3–5% plus feed-conversion and hen-day benchmarks; 4-week rolling trends catch slow drips. **Gate log and guards report to the representative or security contractor**, weekly copy to the owner's store.
- **Payroll:** master file with ID and photo held by the external bookkeeper; owner approves changes; pay to the employee's own account/wallet (unbanked workers: lawyer's alternative); attendance by geotagged check-in or auditor muster; casual day sheets countersigned; annual headcount-to-payroll match.
- **Procurement/sales:** three quotes above threshold, annual re-tender, yearly conflict declarations; minimum price list, owner-signed larger contracts, credit sales approved by owner. Audit scope includes **whitelist price benchmarking**.
- **Incentives:** bonus only on audited figures, 50% deferred with clawback (lawful deductions per lawyer), multi-year measures, welfare/safety gate, integrity multiplier; pool sized to be credible against the exposure estimate in B10. A charter variant exists for an equity/profit-share manager-operator.

## B5. Emergency envelope
Default <=1% AOB per event, **aggregate cap 3% AOB per year and 1.5% per quarter**, after which every event needs the owner or representative. The manager logs notice (call/SMS) to owner and representative **at declaration**. If both are silent for 2 h, the fall-through approver is the deputy, counted only after the logged contact attempts, and **never the payee**; a vet cannot authorise spend on their own invoice. Payment by whitelisted vendor or direct bank transfer, not cash, with photo and incident note. Owner or representative reviews each event within 72 h; a repeating category triggers an audit check.

## B6. Audit
The owner appoints, pays and instructs the auditor; reports go to the owner first; auditors are not peers, rotate at most every 2 years and declare conflicts. The charter grants access to premises, records and staff interviews without manager consent. Tiers: monthly bank/supplier reconciliation by the external bookkeeper from direct feeds; randomised unannounced spot-counts (minimum 4 a year at the small band, 6–12 otherwise; fortnightly in the pilot) counting live animals against tags, payroll muster, procurement against market price, sales against bank; annual licensed-accountant review with bank/supplier/buyer confirmations. Vet who prescribes does not certify deaths for insurance claims.

## B7. Data integrity, privacy and labour law
The entity (not the owner personally) owns data stores, accounts and domains; owner is admin, manager is editor with no delete; append-only log with user, timestamp, photo or GPS on deaths, deliveries, sales and feed issues; duplicate-image and metadata checks at audit. Independent feeds the manager cannot touch: bank, supplier statements, vet invoices, fuel and power meters, gate records. The lawyer's privacy row covers cameras, biometrics, geotagged check-in, vehicle tracking, ID copies held by the bookkeeper (processor terms, retention, access log), the hotline, background and lifestyle checks, and staff notices in local language. Labour row: working-time and rest rules for night watch and 7-day cover, lawful deductions, right-to-work and age checks for casual labour and contractors. Retention: financial 7 years or local law; animal and drug records per regulator; off-site backup under entity control.

## B8. Fraud-response protocol (one page; lawyer and insurer sign)
Triggers: failed spot-count, variance above red, whistle-blower report, bank anomaly. A single trigger **starts the protocol**; it is not a kill trigger. Led by owner or representative, never the line. First 24 h: secure bank access, credentials, records, stores and cameras; image devices; manager informed only after records are secured; suspension on pay as local law allows; interview protocol. Notify the insurer within the policy's deadline; police-referral criteria set in advance; no-retaliation for the reporter; dismissal only after a documented hearing. Sudden manager exit uses the 72-hour playbook (bank control, count, stores, staff briefing, credentials revoked within 1 h, keys re-set).

## B9. Continuity and legal
Separate farm entity (owner director; manager an employee, never director or signatory); written contracts (90-day notice, return of records, confidentiality, clawback per lawyer); manager vetting (non-nominated references, lawful checks, probation); named deputy unrelated to the manager; code of conduct and anonymous channel; power of attorney, standing letter of instruction, "if I am gone" file with the representative, will/trust; insurance (fidelity/crime for manager, bookkeeper and representative; employer's and public liability; property; motor; livestock/crop where available), with claims run only by owner or representative.

## B10. Control-and-oversight cost: definition, bands, expected-loss test
**Included (numerator):** external bookkeeper; spot-counts/auditor; annual accountant review; representative or steward; hotline; fidelity premium; entity/legal (amortised over 3 years); GSM alarms and sensors (amortised); consultant stockman backstop (year 1); data store, geotag/camera tooling; coordinator. **Excluded, reported separately as "management cost":** manager and deputy pay. Vet-of-record and agronomist routine services are production inputs. Denominator: base-case gross revenue.

| Band (base-case gross revenue, currency-equivalent default) | Minimum set | Cap on control-and-oversight cost |
|---|---|---|
| Small (<250k) | Core only; spot-counts at 4+/yr; part-time representative | ~7% |
| Medium (250k–1m) | Core plus quarterly accountant review, steward at part-time | ~8% |
| Larger (>1m) | Full set | ~8–10% |

**Core (never dropped):** owner/representative-held mandates; bank and supplier feeds direct to owner; external bookkeeper; owner-only vendor creation; individual ID and death evidence; randomised spot-counts; annual accountant review; Day-7 safety pack items; compulsory leave; fraud-response protocol. If the core does not fit the cap, the answer is scale down or lease.

**Expected-loss test (optional controls):** for each channel (feed, drugs, livestock, fuel, cash sales, payroll, procurement) estimate annual exposure x probability x detection effectiveness against the control's annual cost. Controls below break-even are cut; the owner signs the residual risk. The bonus pool is sized against the same exposure estimate. Wage expectations of 3–5 manager candidates are tested against the control set before it is finalised.
