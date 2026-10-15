# R5 Adversarial Review: Economics / Management (PLAN.md v5 and appendices)

Lens: farm business economist. Format: numbered; Problem / Why / Fix. Resolved items are not re-raised.

## Verification summary

- **Hours table recomputed.** G0 3x3+6=15; G0 to G1 12x2.5+14+24=68; G2 18x2.5+36=81; G2b 8x4+40=72; pilot 10x3.5+24=59; quarterly 32; reserve 64. The sum is 391, which matches "~390" and 7.5 h/week. Hours to G1 are 15+68=83, which matches the sheet. The weeks column sums to 51 (the "4" on the quarterly row is a count of reviews, not weeks). A3 is 117+36+32+(24-48)+64 = 273-297, so "~280" holds.
- **B12 arithmetic recomputed.** 250-60-40=150; -14 (280 h x 50)=136; -15 (60k/4)=121. Alternative: 60 (3% x 2m) + 18 (4% x 450k) + 20 (4% x 500k) = 98. Headroom is 23k. The 200k sensitivity (71k) is correct. The land-premium counterfactual (+80k) is correct. The 25k cap against 25-75k of margin gives 33-100%, which is correct.
- **Cost caps.** 2-4% = 10-20k, plus 1-3% = 5-15k, cap 5% = 25k. These agree between the sheet and B12. The 8% controls figure (40k) is within the medium-band cap and within one-third of 250k.
- **Front sheet.** The owner can approve or decline: the recommendation, what is not approved, cost basis and cap, hours, outcomes, dates, stop points and five actions are all present. Item 6 below sharpens it, but nothing blocks the decision.

## Findings

1. [MAJOR] The B12 example reaches "proceed" only on a pre-management margin (50% of revenue) that the appendix's own next line contradicts, so the example overstates how reachable the hurdle is.
   Problem: The example assumes a pre-management margin of 250k on 500k revenue. Break-even is 227k, which is 45% of revenue. The next paragraph of B12 sizes the cap against "5-15% net margins on 500k (assumed 25-75k)". The example's own self-run result, before owner time and set-up, is 150k (30%). At 25-75k, the self-run result is far below the 98k hurdle, so the hurdle is unreachable on those figures. The two paragraphs show the owner two different pictures of the same farm. In the first the pre-G1 cap is 17% of a year's margin; in the second it is 33-100%. The term "pre-management margin" is also undefined. B10 and the sheet call it "gross margin" and "margin", and B12 treats the two as equal. If it means gross margin (revenue less variable costs), the example omits hired labour, machinery running costs, depreciation and overheads, and 250k is too high.
   Why: R4-E1 required a demonstration that proceed is achievable "at plausible margins". The example achieves that only by an assumed 45-50% pre-management margin. An owner who reads it would conclude that a typical farm passes and that G1 is a formality. A landowner whose real margin is nearer the stated 5-15% is likely to restructure, and the sheet does not say so.
   Fix: (a) Define "pre-management margin" once: revenue less all operating costs except manager, deputy and controls, including hired labour, depreciation and rates. Use the same term on the sheet, in PLAN criterion 2, in B10 and in B12. (b) Reconcile the two paragraphs: either restate the example margin at a defensible level, or add one sentence: "break-even is 227k, 45% of revenue; most farms in the 5-15% net range will fail the hurdle and the default is restructure". (c) Show the cap against the example's 150k, or state which margin the 33-100% line uses.

2. [MAJOR] The hurdle rule says "best alternative", but the worked example tests only lease, the lowest-hurdle alternative, and the plan does not say how sale or a management company are treated. On the appendix's own placeholders the result flips.
   Problem: On the example's assumptions:
   - Sale: land 2m x 4% = 80k, plus 18k, = 98k income. This beats lease (78k), because 4% exceeds the assumed 3% lease yield.
   - Under the criterion as written, the land premium applies against a sale (4% x 2.5m = 100k), so the hurdle is about 198k against self-run at 121k. The rule as written therefore makes sale the best alternative and the hurdle unreachable.
   - Management company: the fee at 5-10% of revenue is 25-50k, owner hours 80-150 at 50/h are 4-7.5k, and controls are minimal. That gives about 190-220k of net income to the owner from the same 250k margin, against 121k for self-run. On B12's own placeholders it dominates self-run by a large margin, before any premium.
   - The example silently picks lease. It also omits the alternative's owner hours (20-40 h), which the criterion says to include. This is minor in dollars but not like for like.
   - Nothing says whether a landowner who intends to keep the land need consider sale. The intake does not ask whether the owner would sell.
   Why: "Failing the hurdle makes the best alternative the default" is the decision rule. As worded, G1 can return "proceed" (lease only), "exit" (sale) or "restructure" (management company) from the same numbers, and the example's "Proceed, with 23k headroom" is the one outcome that the appendix's own ranges contradict.
   Fix: (a) State the rule: the hurdle is computed against each alternative the owner declares acceptable (add "willing to sell land? y/n" to the intake), and the result is the highest of those hurdles or a small table of all of them. (b) Charge the land premium only when sale is a declared acceptable alternative. (c) Add one line to B12 for the management-company alternative with the 5-10% placeholder, and say plainly that proceed has to beat it, which is why most results will be "restructure". (d) Include the alternative's owner hours in the example.

3. [MINOR] The small-farm threshold is now consistent in kind but not in number, and the screen is not labelled as a necessary test only.
   Problem: The sheet screen uses "~8% controls". B10's small band (<250k) caps at ~7% and the medium band at ~8%. "Small farm" appears in the pre-G1 cost line and is undefined. The screen compares only against lease income, while the G1 hurdle also includes owner time, amortised set-up and the risk premium. On B12's numbers, a 200k margin passes the screen (200-60-40=100 > 60) and fails the hurdle (71 < 98).
   Why: The screen and B10 now agree in method (margin-based, one source of truth), which resolves R4-E2. But the owner may read a screen pass as a likely G1 pass.
   Fix: Say "screen at the band cap (7-8%)", define "small" as the <250k band, and add "passing the screen is necessary, not sufficient".

4. [MINOR] The pilot timing contradicts the year-1 hours table (carried over from R4 item 6; the v5 footnotes did not fix it).
   Problem: Section 3 puts the G3 pilot at ">= 8 wks after G2b ends". On the reference path G2 ends about 3 Jun 2027 and G2b about 29 Jul. The pilot would then start no earlier than about 23 Sep and run to about early Dec, mostly outside year 1 (ends 14 Oct 2027). The hours table instead places a 10-week, 59 h pilot straight after G2b (51 weeks, one unallocated).
   Why: Year-1 hours and "A1/A2 after G3" dates are both affected by a roughly 8-week gap. The total may be off by tens of hours in either direction.
   Fix: Either drop the 8-week gap for the reference path or add an 8-week gap row at routine hours and move the pilot out of year 1. Also relabel the quarterly row "4 reviews" so the weeks column reads as weeks.

5. [MINOR] Cost line on the sheet leaves two ambiguities.
   Problem: (a) "Lawyer and books-review lines quoted separately" does not say whether they sit inside the 25k cap. (b) The window memo's input, stock and sales spend is "outside the pre-G1 cap" (section 8), but the sheet does not tell the owner that approving Gate 0 commits the irreversible seed, fertiliser and restocking decisions by 29 Oct, nor give a size for that spend.
   Why: Stop point 3 ("spend reaches your cap") can fire at a different level from what the owner thinks he has capped.
   Fix: One sentence on the sheet: "Operating spend under the window memo (cap: lesser of your figure and last year's audited spend) is separate from, and not limited by, the pre-G1 cap; lawyer and books-review are inside/outside the cap."

6. [MINOR] The shadow price and the amortisation horizon still differ between sections.
   Problem: Section 4 amortises set-up over 3-5 years and B10 amortises entity and legal over 3 years. B12 uses 4 years for the residue and does not say how the 25k pre-G1 spend enters the 60k. The result is 15k per year (60k/4).
   Fix: State in B12 that the 60k includes the pre-G1 spend, or give the pre-G1 spend its own line.

## Not raised

The decision sheet gets the owner to a clear approve/decline: approve G0 and G1 only, with the cap and stop points. The v5 changes to hours, dates (G1 17 Dec / 29 Jan, manager start, A3 Q3 2028 or Q1 2029) and cost caps agree with one another. The only date contradiction is item 4.

VERDICT: 2 MAJOR remaining
