# R9 Adversarial Review (final): Farm economist / decision theorist (PLAN.md v9, Appendix B10 and B12)

Scope: PLAN.md v9, PLAN-appendix-controls.md (B0, B10, B12), CHANGELOG.md, reviews/r8-final.md. Fresh derivation, not a check of the author's arithmetic.

## 1. Is the R8 MAJOR fixed?

**Yes.** The convention is now internally coherent and the printed flip point exposes the one input that drives the exit/hold boundary.

**Convention, re-derived.** Everything is real, on one asset base (land 2.0m + stock and machinery 0.45m). OMBM charges no land rent, so self-run income already contains the return on the owner's land. Lease rent is that same return received from a tenant, so it is not added to OMBM. Land-value change g x L is added once to every hold option and to none of the sale. The sale earns a real return on net proceeds. No land charge is subtracted from any option. I find no double count: the 60k rent and the OMBM land return are alternatives, not additive. Hold options that keep the land carry the same g x L = 20k, so g cancels between hold options. Therefore the best hold option does not change with g, and the flip point is a clean closed form: g* = (sale - best hold value excluding g x L) / L.

**Recomputed values (k, g = +1%, L = 2,000).**

| Item | Recomputed | Text |
|---|---|---|
| Self-run, Ex 1 | 110-60-40-14-15-20 = -39; +20 = -19 (-0.8%) | same |
| Self-run, Ex 2 | 250-149 = 101; +20 = 121 (4.9%) | same |
| Management co., Ex 1 | 99-35-30-5.75-7.5-20 = 0.75; +20 = 20.75 | 20.8 |
| Management co., Ex 2 | 225-98.25 = 126.75; +20 = 146.75 (6.0%) | 146.8 |
| Lease | 60+9-9-1.5-7.5 = 51; +20 = 71.0 (2.9%) | same |
| Sale | 2,450 x 0.95 = 2,327.5; x 2% = 46.55 (1.9%) | 46.6 |
| Ex 1 management co. drought stress | 0.9 x (110-150) - 35 - 30 = -101 < -50: dropped | same |
| Ex 2 self-run stress | drought 100-100 = 0; notifiable 210-100 = +110 | same |
| Ex 1 one-third limit | 110/3 = 36.7 < 40: fails | same |

**Flip points.**
- Ex 1, sale vs lease: 51 + 2000g < 46.55 gives g < -0.22%, matching "-0.2%". At g = -2%, lease = 11.0 and sale (46.6) wins. Self-run (-79) and management company (-39) are dropped, so the result is a conditional exit. Matches.
- Ex 2, sale vs self-run: 101 + 2000g < 46.55 gives g < -2.72%, matching "-2.7%". Sale vs management company: 126.75 + 2000g < 46.55 gives g < -4.01%, matching "-4.0%".

**Break-evens.**
- Self-run vs lease: OMBM - 149 = 51 gives OMBM = 200k (40%). Matches.
- Self-run vs sale: OMBM - 149 + 20 = 46.55 gives 175.6k (35%), matching "about 176k". It holds only at g = +1% (g does not cancel against sale). The text says "g cancels between hold options" so it is accurate, but 176k should be labelled "at default g".
- Management company vs self-run: 0.1 x OMBM = 50.75 gives 507.5k, above the 500k revenue. "Wins at every credible margin" is true.
- Pre-G1 cap 25k = 22.7% and 10% of OMBM. Matches.

Rate-on-base figures and tie logic (5% of top) check out. Step 5 compares a value that includes g x L with 10% of OMBM; acceptable as a default.

**Omitted or one-sided items (none flips a worked example).**
- Cash tax: sale carries tax on the gain inside the 5% default (flagged as possibly low, accountant to quantify), but hold-option income (rent, OMBM) is pre-tax. The bias runs against sale, so it makes restructure/hold look better than it may be. It is disclosed ("tax can be far higher").
- One-off costs are amortised over 4 years, while the lease or self-run lives much longer. This overstates annual cost for restructure and self-run relative to sale (whose 5% cost is permanent). It is conservative and symmetric across hold options, so it does not reorder them.
- The set-up line (20k "interim lead and consultant backstop") and the B10 control line ("consultant backstop for the first cycle", inside the 40k) can both charge the consultant. This is a possible 5k/yr double charge against self-run only. Conservative; MINOR.
- Working capital (50k) is in K but not in the asset base, so lease and sale omit about 1k of return on released working capital. Trivial.
- Land-value risk is stated, not charged, while self-run is charged r x K. This is acknowledged and is what the flip point exposes. Acceptable.

## 2. Four edge cases of my own

1. **Declared return as the swing input.** Ex 1: lease beats sale only while the real return on proceeds is below 71.0 / 2,327.5 = 3.05%. An owner who quotes a nominal 4-5% (the old plan's number) flips Ex 1 to exit. The intake and B12 now require "real", but the printed output shows only g*. **[MINOR]** Print the equivalent return* (here 3.05%) next to g*, and add "if you quote a nominal rate, subtract expected inflation".
2. **Leveraged farm.** B12 says debt is "repaid from proceeds" for sale, while hold values are before interest. That compares equity (sale) with assets (hold). With 500k debt at 3% real: lease on an equity basis is 71 - 15 = 56 and sale is (2,327.5 - 500) x 2% = 36.6, whereas the as-written mix gives 71 vs 36.6. This overstates the hold margin by about 15k, roughly 0.7 points on g*. **[MINOR]** One line: value all options before debt (sale on gross proceeds) or all after interest. This cannot flip the worked examples, which assume no debt.
3. **Set-up cash in the stress test.** Ex 2 self-run drought net cash is 0 with no set-up cash. If the 60k set-up is paid in the stress year (cash, not amortised), it is -60, below the -50 limit, and self-run fails. Ex 2's "if no management company, self-run proceeds" would then become "restructure to lease". The stress text says "own cash flows after fees" and is silent. Ex 2's headline (management company first) is unaffected. **[MINOR]** State whether set-up and transition cash falls in the stress year; the conservative reading is yes.
4. **Strongly negative g with no management company, Ex 2, g = -3%.** Self-run is 101 - 60 = 41, below sale (46.55) and above zero. Lease is 51 - 60 = -9 and is dropped. Result: conditional exit, consistent with the -2.7% flip, even though self-run is profitable. If the owner would not sell, self-run (41) is the top and "proceed" returns. Both follow from the rules. A pure data point, no defect.

## 3. Front sheet against B12

Matches. G1 criterion 1 mirrors B12: real terms, same-asset-base income, hold options include land return and g x L, sale only if the owner would sell, the drop rule with the -10% K stress default, the ranking outcomes, the printed g*, the "not executable" fall-through and the 10%-of-OMBM conditional pass. Gate 0 intake asks for sale price, real return, g and the alternatives. The recommendation is "approve Gate 0 and Gate 1 only"; manager offer and SOPs are expressly deferred. The cap of 25k (5% of 500k) matches B12's cap line. Minor wording: the sheet says "exit", criterion 1 and B12 say "conditional exit"; align on the next edit (MINOR).

## 4. Skim for contradictions

- **Hours.** 15 + 68 + 81 + 72 + 59 + 32 + 64 = 391 over 3 + 12 + 18 + 8 + 10 = 51 weeks. Each row recomputes. 83 h to G1 and about 280 h at A3 (2.25 x 52 + 36 + 32 + 24-48 + 64 = 273-297) match the sheet.
- **Dates.** 9 weeks from 15 Oct = 17 Dec; 15 weeks = 28-29 Jan. +18 weeks = early June 2027, which fits the reference manager start. 51 weeks ends about 6 Oct, inside year 1 (to 14 Oct). Consistent.
- **Caps and cross-refs.** B0.5/B6 4-month maximum, G2 exit definition, B10 bands 7-10% vs the sheet's 7-8% screen, A0/A6 (in situ counting, "Spot-counts and standstill") all resolve. No stale economics (582k, 93.1, 4% return) remain outside historical CHANGELOG rows and old versions.
- **[MINOR] Earliest A3 dates.** The A3 row requires the full cycle to be run by the manager, not the interim lead. Under that rule, the N covered start (manager runs from Nov 2027) and the S slip case (interim lead to Mar 2028) most plausibly reach A3 one to two quarters later than "Q3 2028" and "~Q4 2028". They are labelled "earliest", and "plan on Q1 2029" is safe, so nothing misleads the decision.

## Verdict

The R8 MAJOR is closed: convention, g handling, flip points, break-evens and both worked examples reproduce. No sign error, no double-counted land return, and no omitted cost that reorders a worked ranking. The remaining items (return* print, debt basis, set-up cash in the stress test, consultant double charge, sheet wording, early-A3 labels) are MINOR and can be tuned at G1 with real inputs.

VERDICT: 0 MAJOR remaining
