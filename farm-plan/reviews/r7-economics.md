# R7 Adversarial Review (final): Economics / Decision theory (PLAN.md v7, Appendix B10 and B12)

Lens: farm business economist / decision theorist. Resolved items are not re-raised.

## R6 MAJOR (incomplete decision procedure): fixed

B12 now has a numeric stress limit (worst single scenario cash loss <=10% of K, cash above floor, owner signs the amount). It has a drop rule (value <=0 or failed stress), a ranking, a tie rule (within 5%, then lower hours, then lower worst-scenario loss) and an explicit "no viable option, do not proceed" outcome. Section 4 criterion 1 matches B12, and the closing line is true as written: proceed cannot be returned at value <=0 or after a failed stress test.

## Recomputation

- Example 1 (OMBM 110k):
  - Self-run: 110-60-40-14-15-20 = -39. Dropped.
  - Management company: 99-35-30-5.75-20 = 8.25. Ranks second.
  - Lease: 78-1.5 = 76.5. Ranks first, so restructure to lease.
- Example 2 (OMBM 250k):
  - Self-run: 101.
  - Management company: 225-35-30-5.75-20 = 134.25.
  - Lease: 76.5.
  - Management company ranks first. Without it, self-run is 24.5k above lease, so proceed.
- Break-even of self-run against lease: 76.5+149 = 225.5k, which is 45.1% of revenue.
- Pre-G1 cap of 25k: 22.7% of 110k and 10% of 250k.
- Self-run's drought stress in Example 2 reconciles. A 30% revenue drop is 150k, so OMBM falls to 100k. Less 100k of management and controls, cash after is 0, inside the 50k limit.
- Sheet arithmetic: pre-G1 spend 10–20k plus 5–15k at 500k; section 5 rows sum to 391 h over 51 weeks; A3 is about 280 h.
- Screen against B12: any option that wins on B12 over lease also clears the screen, so the screen is necessary, as stated.

## Edge cases

1. **All options dropped, or only self-run declared and it is negative (Example 1 with lease and the management company unavailable).** Self-run is dropped and step 5 returns "no viable option". The money already spent is sunk and does not alter the result. Works.
2. **Self-run is the only option, positive, but fails stress.** It is dropped and step 5 returns no viable option. The prior failure mode is closed. Works.
3. **Tie between lease and grazing.** Lower hours win, which is lease (30 h against 40–80 h). Works. Two points (item 3 below): the 5% tie is not transitive, and grazing has no stress definition.
4. **Owner will not sell but sale is ranked.** Sale is excluded because it is acceptable only if the owner would sell, and land cancels in the hold options. Works. The opposite case, an owner who would sell, is item 1.
5. **Sunk pre-G1 spend flips the result.** It cannot. It is excluded from every value and enters only the kill trigger, so the ranking never flips. The post-G1 set-up (60k) is charged to self-run only. Lease, management company and grazing carry no transition cost (lawyer, tenant search, stock-sale commission and tax). That bias is under 10k a year against a 24.5k margin, so it does not flip Example 2, but it favours restructure. See item 4.
6. **Marginally positive winner.** Self-run at +1k, with nothing else acceptable, returns proceed. The inputs are assumed, so there is no margin for estimation error. See item 5.
7. **Top option cannot be executed.** A lease or management-company quote is indicative, and a lessee may not exist. The rule does not say the next-ranked option applies.

## Findings

1. [MAJOR] The land charge is applied to the hold options but not to the sale option, so the would-sell branch is biased toward exit.
   - Problem: B12 subtracts land price x declared return from "every hold option" and values sale as "proceeds x declared return", gross. The ranking therefore compares net values against a gross one.
   - Example: land 2m at 4% is 80k, and stock and machinery add 18k, so sale is 98k. Example 2 self-run is 101k absolute, and 21k after the charge. The rule ranks sale (98) over self-run (21) and returns **exit**. On a like-for-like basis self-run (101) beats sale (98). The 80k bias is about the size of the entire margin. It can also drop a sound lease (76.5 absolute, -3.5 after the charge) for a reason that does not reflect economics.
   - Why: the intake explicitly asks "would you sell", so this branch will occur. It recommends an irreversible sale on an arithmetic inconsistency. "Proceeds" is also ambiguous between land only and land plus stock.
   - Fix: apply one convention to every option. Either subtract land x return from sale as well (sale then equals the return on stock proceeds, 18k in the example), or subtract nothing from any option and compare absolutes. Define sale proceeds as land plus stock and machinery net of selling cost and tax. R6 accepted the 98-against-21 result, which is how this slipped through.

2. [MINOR] Stress is defined only for self-run in practice. Management company, grazing and manager-operator retain K or fees but have no stress formula.
   - Example 1's management company would fail the same drought scenario. A 30% drought on a 500k revenue farm takes OMBM 110 to -40, so 0.9x(-40)-35-30 is about a 100k loss against the 50k limit. It would drop out, but lease still ranks first, so the result is unchanged.
   - The Example 2 self-run stress cites the drought only. The notifiable-event scenario, with the largest enterprise at full loss and sales stopped for 90 days, is not shown and could be worse.
   - Fix: add one line that stress is computed on each option's own cash flows after fees. Show the worst scenario for Example 2.

3. [MINOR] The tie rule (within 5% of the higher value) is not transitive. Values 100, 96 and 92 chain A to B and B to C but not A to C. Fix: compare each option to the top value only.

4. [MINOR] Restructure options carry no transition cost (lawyer, tenant or operator search, stock-sale commission and tax) while self-run carries 15k a year of set-up. Add a one-line placeholder for transition cost, or note that the comparison is biased toward restructure. Also, if the top option cannot be executed at the quoted terms, the next-ranked option should apply and be re-run.

5. [MINOR] "No viable option" is a fourth outcome that does not appear on the decision sheet row for G1 outcomes (proceed, restructure, exit). B12 step 4 also lists manager-operator as a rankable top choice although it has no value without a quote. A winner that is only marginally positive has no minimum margin over zero or over the next option. Fix: add "no viable option" to the sheet, and either exclude the unquoted manager-operator from step 4 or state it cannot rank. Optionally add a minimum margin, for example the pass is conditional if the winner's value is under 10% of its OMBM.

## Front sheet against Section 4 and B12

Consistent on the points that matter:
- The decision sheet's screen, pre-G1 cap, hours (83 to G1, 390 in year 1, 280 at A3), dates and stop points agree with sections 3–5 and B10/B12.
- The outcomes row defers to the section 4 ranking, and the lease, grazing and management-company hours bands (20–40, 40–80, 80–150) bracket the B12 inputs of 30 and 115.
- Only the "no viable option" outcome in item 5 is missing from the sheet.

VERDICT: 1 MAJOR remaining
