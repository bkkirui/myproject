# R8 Adversarial Review (final): Economics / Decision theory (PLAN.md v8, Appendix B10 and B12)

Lens: farm economist / decision theorist, fresh eyes. Scope: PLAN.md, both appendices, CHANGELOG, r7-economics.md.

## 1. Is the R7 MAJOR (land-charge asymmetry) fixed?

**Yes, as to the asymmetry R7 found.** The convention is coherent:
- OMBM charges no land rent, so self-run income already contains the return on the land the owner keeps.
- Lease rent (60k) is that same land return, received from a tenant instead of earned by operating. It is not added on top of OMBM.
- A lease option that earns rent and a self-run option whose OMBM excludes land rent therefore each count land return exactly once. Sale converts the whole base to cash at the declared return.
- No land charge is subtracted from any option, so the 98-against-21 bias is gone.
- The like-for-like check (value divided by the 2.45m base) is a useful guard.

**Recomputation (all match the text):**

| Item | Result |
|---|---|
| Self-run, Example 1 | 110-60-40-14-15-20 = -39 (-1.6%) |
| Self-run, Example 2 | 250-149 = 101 (4.1%) |
| Management company, Example 1 | 99-35-30-5.75-7.5-20 = 0.75 |
| Management company, Example 2 | 225-98.25 = 126.75 (5.2%) |
| Lease | 78-1.5-7.5 = 69.0 (2.8%) |
| Sale | 2.45m x 0.95 x 4% = 93.1 (3.8%) |
| Self-run against lease | OMBM 218k (43.6%, text says 44%) |
| Self-run against sale | OMBM 242.1k (48.4%) |
| Management company against self-run | 0.1 x OMBM = 50.75, so OMBM 507.5k |
| Example 1 one-third control limit | 110/3 = 36.7k, so 40k fails |
| Example 1 management company drought stress | 0.9 x (-40) - 65 = -101k, so dropped |
| Pre-G1 cap | 25k is 22.7% of 110k and 10% of 250k |
| "Self-run beats lease by 32k" | 101-69 = 32 |
| "Sale more than 5% below self-run" | 93.1 < 95.95 |

Management company at 507.5k exceeds the 500k revenue, so "wins at every credible margin" is true.

Result rows in both examples follow from the procedure. Ranking and tie logic are deterministic.

### Remaining like-for-like issues

**[MAJOR] The basis of "declared return" against hold-option return is unstated, and land value change is omitted.**
- Hold options are valued on income only: OMBM, or rent at 3% of land. Sale is valued at a cash "declared return" of 4%.
- A hold option keeps the land, which carries expected capital growth (at least inflation, usually more) and capital risk. The convention drops both. Cash proceeds earn a return that is probably nominal and, unlike land, does not keep up with inflation.
- The comparison is therefore income-yield against cash-return. It is not total return on the same assets, which the sheet claims.
- Size: Example 1's exit-against-lease gap is 93.1-69.0 = 24.1k, which is 1.2% of the 2m land value. A real land-value change of +1.2% a year, well inside the normal range, reverses "exit" to "restructure to lease". In Example 2 a +0.4% change (7.9k) closes the sale-against-self-run gap.
- Sale is irreversible and the intake asks "would you sell", so this branch will occur.
- Fix, minimal: add one input g, the expected annual real change in land value, with a default and a printed sensitivity ("lease overtakes sale at g = 1.2%"). Require the declared return to be stated in real terms. Add land capital risk to the risk charge or note it.

**[MINOR] Lease and grazing omit landlord-retained costs.**
- Self-run OMBM is after rates, insurance, depreciation and repairs on fixed improvements. The lease formula deducts none of them. A gross lease leaves them with the owner, roughly 0.3-0.6% of land value (6-12k on 2m).
- Fix: state that the placeholder rent is net of these, or deduct them.
- This does not flip either example. It moves the lease-against-self-run break-even from 218k to roughly 225-230k, and it favours restructure.

**[MINOR] Stress metric is used inconsistently in Example 2.**
- Drought is reported as "cash 0" (net cash after fees), but the notifiable event as "40k" (a reduction in OMBM).
- Net cash in the notifiable case is 250-40-100 = +110k, so the loss is zero.
- Under the "reduction" reading the drought (150k) would fail. Under the "net negative cash" reading, which Example 1's management company uses, both pass trivially.
- The 40k is also an unsourced assumption.
- Fix: define stress as net cash after management, controls, interest and tax. Drop the "40k" label, or define the metric as a drop and show that it fails.

**[MINOR] Stress ignores debt service, tax and drawings.**
- OMBM is before interest. Example 2's drought leaves exactly 0 headroom, so any interest bill fails the "cash above floor" leg.
- Sale proceeds should be shown asset-level (debt repaid from proceeds) to match the hold options, which are before interest.

**[MINOR] Transition and ramp costs.**
- "Post-G1 set-up 60k" is not defined. It is unclear whether it includes the interim lead, consultant backstop and the double-running year.
- Transition cost on restructure omits redundancy for staff the tenant or operator does not take (labour law).
- Self-run uses the A3 steady-state 280 h. The plan's own year 1 is 391 h, which is about 5.5k more in year 1 only. This does not flip anything.

**[MINOR] OMBM normalisation.**
- Unpaid family or owner labour in the last accounts overstates OMBM. The intake should require normalisation.
- "Conditional pass if value is under 10% of OMBM" is meaningless when OMBM is zero or negative, and when the winner is sale.

## 2. Five edge cases

1. **Owner would sell, and declared return is 5% instead of 4%.** Sale is 116.4k. It beats self-run in Example 2 (101) and exits. The result hinges on a single owner-declared input, which is the problem raised in the MAJOR above. The break-even return is shown only for OMBM, not for the return.
2. **Lease and management company both unavailable, would not sell, Example 1.** Self-run is -39, dropped, and "no viable option" is returned. Correct.
3. **OMBM equals 180k, passes the days 1-3 screen (OMBM-100 > 78).** Self-run is 31, below lease at 69, so the screen is necessary only. Consistent with its wording.
4. **Management company wins by 25.75k but needs mandates and entity set-up.** MC carries only 7.5k transition and no set-up. Unless the 60k set-up is genuinely absent for MC, MC is biased up by about 15k. It still wins, but it narrows toward self-run in a mid-margin farm. Minor, and folds into the set-up definition item.
5. **Top option is lease, but no tenant exists.** The next-ranked option applies and the ranking is re-run (step 4). Works. Sale of stock to fund the lease transition is covered by the transition cost.

## 3. Front sheet against B12

- The decision sheet matches B12 on screen, quotes, outcomes (proceed, restructure, exit, no viable option), cap 25k at 500k, hours bands, and the "approve Gate 0 and Gate 1 only" recommendation.
- The five actions are doable by a busy owner: intake by 22 Oct, lawyer, vet and agronomist, packs, representative candidate. The owner is not asked to approve a manager or SOPs.
- The screen is necessary for all three hold options: OMBM > 178k against a management company break-even of 186k and a self-run break-even of 218k.
- Hours: 15+68+81+72+59+32+64 = 391 over 51 weeks. 83 to G1. About 280 at A3 (273-297). Match the sheet.
- Dates: 15 Oct + 9 weeks = 17 Dec, + 15 weeks = 29 Jan. 29 Jan + 18 weeks = early June, and the Jun 2027 manager start fits the 3-6-month recruitment window.

## 4. Skim of the package

- Cross-references checked and consistent: B0.4, B0.5, B6 (4-month maximum), B8, B10, B12, A0, window memo, G2 exit definition, season table against the A3 dates, sheet against sections 4 and 5.
- The CHANGELOG quotes the old ~582k break-even in a historical row (v6). It does not contradict v8, which says ~508k.
- No dating, hours or cost-cap contradiction found that would mislead the decision.
- One watch item (not a MAJOR): the N covered-start A3 of Q3 2028 depends on counting a harvest and planting cycle that the interim lead ran in 2027. Section 3's A3 row requires those events to be covered in the 12 months. State which events must be manager-run.

VERDICT: 1 MAJOR remaining
