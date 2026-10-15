# R4 Adversarial Review: Economics / Management (PLAN.md v4 and appendices)

Lens: farm business economist and consultant, judging v4 as a decision memo for a busy senior academic economist. Format: numbered; Problem / Why / Fix.

Word count: `wc -w` gives PLAN.md 2,200, but about 185 of those are table pipe characters. Real words are about 2,015, so the CHANGELOG's "about 2,100" is conservative and the body is essentially at the 2,000 target. The decision sheet is about 400 words and fits one page. Appendix A is 1,891 words, Appendix B 2,281 and the CHANGELOG 2,701 (not read by the owner).

## (a) Were the R3 MAJORs genuinely fixed?

- **R3-E1 hours table: fixed.** I recomputed every row.
  - G0: 3 x 3 + 6 = 15. G0 to G1: 12 x 2.5 + 14 + 24 = 68. G2: 18 x 2.5 + 36 = 81. G2b: 8 x 4 + 40 = 72. Pilot: 10 x 3.5 + 24 = 59. Quarterly 32. Crisis 64.
  - The sum is 391, matching "~390", and 391 / 52 = 7.5 h/week, matching the sheet.
  - The week counts agree with the dated path: G1 29 Jan plus 18 weeks is early June, which is the reference manager start.
  - A3: 2.25 x 52 = 117, plus 36, 32, 24-48 and 64 gives 273-297, consistent with "~280" and "~5 h/week".
  - Residuals are MINOR (item 6).
- **R3-E2 goal honesty: fixed.** The sheet opens by stating that "no involvement" is not achievable and that the goal becomes "no daily involvement". It gives about 5 h/week at A3 and Q3 2028 (plan on Q1 2029), says hours never reach zero, and lists lease, contract grazing and a management company with indicative hours (20-40, 40-80, 80-150) as first-class G1 options. Those hours are labelled "indicative", which is enough for a sheet (see item 8).
- **R3-E3 cost figures and cap rule: fixed.** The rule is now coherent: indicative 2-4% (plus 1-3% if there is no incumbent), a fixed owner-set cap (proposal 5%), and "quotes above it return to you". The worked example checks: 500k gives 10-20k, plus 5-15k, cap 25k. Steady-state overhead is stated as 7-10% plus manager and deputy pay. The residual is MINOR (item 4).
- **R3-E4 G1 hurdle: structurally fixed.** It now includes owner time at a declared shadow price, amortisation of set-up over 3-5 years, a like-for-like alternative and a defined capital basis. The control-cost test is coherent between PLAN criterion 2 and B10: band cap and one-third of pre-management gross margin, with the core never dropped and an expected-loss test for the rest. The default risk premium, applied to the capital basis the plan chose, is now the problem (item 1).

## (b) Findings

1. [MAJOR] The default risk premium (3-5% of invested capital, where capital includes land at market value) makes "proceed" nearly unreachable for any landowning farm.
   Problem: PLAN section 4, criterion 1 requires self-run net margin, after management, control cost, owner time and amortised set-up, to exceed the best alternative's income plus 3-5% of land, stock and machinery at market value. Farmland typically returns only about 2-4% of its value as lease rent, and a well-run operation earns perhaps 4-6% on total assets before paying a manager. Take land, stock and machinery worth 3m. The premium alone is 90-150k a year, on a farm whose gross revenue (the plan's own example scale) is around 500k. Even before the other deductions, self-run must beat lease by more than the farm's plausible entire net margin.
   - The land risk is the same in the self-run and lease cases, because the owner keeps the land either way. The incremental risk of self-running sits in the stock, machinery and working capital, not the land.
   - Land belongs in the base only when the alternative is sale.
   Why: G1 is presented as a genuine three-way decision (proceed, restructure or exit). With this default the outcome is close to fixed at "restructure", while the owner has already paid up to the pre-G1 cap. That is a misleading decision rule. Section 4 also stacks conservatisms: the premium, the owner's time, set-up amortisation, and the stress-loss limit.
   Fix: Define the premium on operating capital at risk (stock, machinery, working capital and the cash-flow trough), not on land. Charge land only against a sale alternative. Add one worked example at the 500k scale showing the hurdle arithmetic with lease income, so that the owner can see that proceed is achievable at plausible margins. Keep the 3-5% as an owner-adjustable default.

2. [MINOR] The day 1-3 feasibility screen tests only the control cost, not control plus manager pay, and its threshold disagrees with B10.
   Problem: The sheet says base revenue under about 250k probably fails the control-cost test. B10 says "under about 150-200k". A hired manager (not in the control-cost numerator) typically consumes 10-20% of revenue on a farm of this scale. Controls of 7-10% plus manager and deputy pay therefore exceed the pre-management margin on many farms well above 250k. The sheet does not tell the owner this.
   Why: A 300-500k farm passes the screen, spends up to 5% on pre-G1 work, and then fails at G1 for a reason that the accounts could have shown in three days.
   Fix: Make the screen "pre-management margin minus a local manager wage and 7-8% controls is above the lease income", using last year's accounts. Use one threshold in both files.

3. [MINOR] Possible double counting in the hurdle: set-up costs appear both in control cost and in the amortised set-up.
   Problem: Criterion 1 deducts "management and control cost" and also "one-off set-up amortised over 3-5 years (entity, legal, SOPs, tools, ... consultant backstop ...)". B10 already puts entity/legal (amortised over 3 years), tools and the consultant backstop into control cost.
   Why: It overstates costs against self-run, which compounds item 1.
   Fix: Add one clause: "set-up items already in B10 are counted once", and align the amortisation horizon (3 in B10, 3-5 in section 4).

4. [MINOR] The cap sits inside the plausible range when no incumbent exists, and it is never related to the farm's margin.
   Problem: With no incumbent the indicative range is 3-7% (15-35k at 500k), and the proposed cap is 5% (25k). The mid-case therefore touches the cap and stop point (3) fires on an ordinary outcome, which is the loop R3-E3 warned about. The cap is also not shown against a year's net margin. On a 500k farm with a 5-15% margin, 25k is 33-100% of a year's profit at risk before any decision.
   Fix: State, in one clause, that cap exhaustion is expected where there is no incumbent and that the owner re-approves on quotes. Show the cap as a share of margin in the worked example, so that the owner sees the size of the bet.

5. [MINOR] The sheet gives the owner a cost-and-hours picture for the whole programme but not for the thing being approved.
   Problem: The recommendation is "approve G0 and G1 only". The sheet gives about 390 h for the whole first year but not the hours to G1, which the table puts at 15 + 68 = about 83 h through 29 Jan. It gives steady-state overhead only as percentages. A single line of dollars at the example scale (500k: controls 35-50k plus manager and deputy pay) would show the scale of the commitment he is declining or entering.
   Why: The sheet is otherwise good. He can approve or decline, but he has to infer the G1-only commitment.
   Fix: Add "To G1: about 83 h, spend up to the cap (25k at 500k)" and one illustrative steady-state dollar line.

6. [MINOR] Small arithmetic and definition loose ends in section 5.
   Problem:
   - The weeks column sums to 51, not 52. It is cosmetic, but a one-week gap should be shown.
   - "G3 pilot >=8 wks after G2b" is ambiguous. If it means after G2b ends, the pilot (10 weeks) runs past 14 Oct and the year-1 total changes.
   - "Range 330-450" has no stated derivation (about +/-15%).
   - Whether the 30-45 min/week approval queue is inside the routine hours is not stated.
   - A3 is defined as a quarterly review, yet the A3 hours include 36 h of monthly review.
   Fix: One footnote line each, or a note "monthly digest, not a review".

7. [MINOR] The invented numbers are flagged globally but not on the figures that carry the decision.
   Problem: Line 3 says every number is a default to be calibrated, and the pre-G1 cost and the lease hours are marked "indicative". The 250k screen, the 3-5% premium, the 5% cap proposal and the per-row weekly hours (which generate the 390 h) have no source and no "assumed" tag. Section 4 tags model inputs measured / benchmark / assumed, but the sheet does not apply that tag to its own figures.
   Fix: Add "(assumed, no source)" next to the hours rows and the premium, or one sentence on the sheet: "figures marked ~ are my assumptions pending quotes and accounts."

8. [MINOR] The lease and management-company comparison is stated in hours, not in income.
   Problem: The sheet gives indicative owner hours for the three non-self-run options but no indication of net income levels or where they sit against self-run (lease rent as a % of land value, management company fee as a % of revenue).
   Fix: Give a one-line indicative range for each, flagged as placeholder, so the owner can see roughly why G1 would favour one of them.

## (c) Consistency check

- Hours: table, sheet (390 h, 7.5 h/week) and A3 (~280 h) agree. The 150% kill trigger pegs to the section 5 schedule.
- Dates: G1 29 Jan, G2 18 weeks, manager Jun 2027, A3 Q3 2028 / Q1 2029 agree between the sheet, the season table and the hours table.
- Cost: sheet example arithmetic is correct. The control band caps (7 / 8 / 8-10%) agree with the sheet's "7-10%", and the one-third margin test appears in both PLAN and B10.
- Inconsistent: the 250k versus 150-200k small-farm threshold (item 2).

## (d) Can the owner approve or not approve from the front sheet?

Yes. The sheet states the recommendation (G0 and G1 only), what is not approved, the cost basis and cap rule, hours, outcomes, dates, stop points and five actions. Items 2, 4, 5 and 8 would sharpen it, but none of them blocks the decision. The one thing that could mislead the G1 outcome itself is item 1.

VERDICT: 1 MAJOR remaining
