# R6 Adversarial Review (final verification): Economics / Management (PLAN.md v6 and appendices)

Lens: farm business economist. Numbered; Problem / Why / Fix. Resolved items are not re-raised.

## Verification of R5 MAJORs

- **E1 (definition and two examples): fixed.** OMBM is defined once (B10) and used on the sheet, in criterion 2 and in B12. The text says it is before interest and charges no land rent, and that "gross margin" is a different term. The 22% and 50% margins are labelled as examples, not as forecasts.
- **E2 (alternatives, intake, outcomes): mostly fixed.** The intake asks "would you sell" and which alternatives are acceptable. The land charge applies only if you would sell. Every option has its own formula and its own owner hours. The management-company haircut is explicit. The main paths now produce one outcome each. One branch is still open (item 1).

**Recomputation (all checked):**
- Example 1 (OMBM 110k):
  - Self-run: 110−60−40−14−15−20 = −39. Correct.
  - Management company: 99−35−30−5.75−20 = 8.25, shown as 8. Correct.
  - Lease: 78−1.5 = 76.5. Correct. Lease ranks first, so restructure to lease.
- Example 2 (OMBM 250k):
  - Self-run: 250−149 = 101. Correct.
  - Management company: 225−90.75 = 134.25. Correct.
  - Lease: 76.5. Management company ranks first. Without it, self-run beats lease by 24.5. Correct.
- **Break-even against lease:** OMBM = 76.5+149 = 225.5k, which is about 226k and 45.1% of revenue. Correct.
- **Cap shares:** 25k is 22.7% of 110k and 10% of 250k. Correct.
- **Inputs:** common inputs agree with the sheet and the hours table. Self-run 280 h, management company 115 h (inside 80–150) and lease 30 h (inside 20–40). Lease rent is 3% of 2m = 60k. The 4% return on 450k = 18k. Controls are 8% of 500k = 40k, and 60k/4 = 15k.
- **My own derived points (not in the plan):**
  - Management company against lease breaks even at OMBM of about 186k.
  - Management company against self-run breaks even at about 582k, which is more than 100% of revenue. On B12's placeholders a management company beats self-run at every credible margin.
  - The haircut that would flip Example 2 to self-run is about 23%, against the 10% default.
- **Example 1 and the one-third test:** at 8% controls, 40k is 36% of 110k, so Example 1 also fails criterion 2. That is consistent with "restructure" and needs no fix.

## Edge-case tests

- **Owner would not sell:** the sale option and the land charge both drop out. Land is held in every option and cancels, so the ranking is among the hold options. Works.
- **Owner would sell at 4% (land 2m):** every hold option loses 80k. Lease falls to −3.5 and self-run in Example 2 to 21, against sale at 98. The result is exit. Deterministic and sensible.
- **Management company unavailable or unacceptable:** it drops out, and Example 2 reverts to self-run, 24.5k above lease. Works.
- **Self-run first but fails stress, or has negative value, or is the only option:** not handled (item 1).

## Front sheet against B12

The sheet agrees with B12 and still lets the owner approve or decline.
- The G1 outcomes row names proceed, restructure and exit "by the ranking in section 4".
- The recommendation, cost cap, hours, dates and stop points are present.
- The overhead row points to the B12 examples.
- Items 3 and 4 below are refinements. Nothing blocks the decision.

## Findings

1. [MAJOR] The decision procedure is not complete: no outcome when self-run ranks first but fails the stress limit, and no floor on the winning option.
   Problem: B12 and section 4 say "Self-run first and within the stress limit: proceed". They are silent on self-run first but outside the stress limit. That is the likely case for a farm that clears lease only narrowly, as Example 2 does without a management company. The stress limit has no number or measure anywhere in the plan. "G1-signed limit" appears only under kill triggers, as a cumulative-loss limit. A further gap: the ranking has no minimum. If the owner declares only self-run acceptable, because he will not sell and no lessee or management company exists, self-run ranks first even at −39 (Example 1) and the rule returns "proceed". Ties and "all options negative" are also unhandled.
   Why: R5-E2 required deterministic outcomes, and the changelog claims them. Without this branch G1 can return no outcome in a plausible case, and a loss-making self-run can be approved on a technicality. The owner would then decide ad hoc at the gate, which is the discretion the rule was meant to remove.
   Fix: Add two sentences to B12 and section 4. (a) Define the stress limit as the worst stressed-year cash loss and the signed amount, for example "no more than X% of K, and cash above floor". (b) State the fall-through: an option that fails stress or has a value at or below zero is dropped and the next-ranked option applies. If none remains, the outcome is exit or lease at any price, and the owner is told that no acceptable option exists. Ties go to the lower-hours option.

2. [MINOR] The sheet does not say that a management company beats self-run on the placeholders, and the free screen does not test it.
   Problem: The screen compares only against lease income. A farm that passes it, such as Example 2 at 250k, still loses to a management company until OMBM reaches about 582k. The pre-G1 spend is 15–35k, with a cap of 25k. The sheet says only that lease or restructure is "the honest answer on many farms".
   Why: An owner whose goal is no involvement may spend the G1 money to learn what indicative management-company and lease quotes would show in the first week.
   Fix: Add to the days 1–3 screen: "obtain 1–2 indicative management-company, lease and grazing quotes and put them in the B12 formula". Add one sentence on the sheet: "On B12's placeholders a management company beats self-run unless its fee or haircut is much worse, so proceed mainly arises where none is available."

3. [MINOR] Contract grazing and manager-operator are ranked but have no formula, and the sale and would-sell inputs can contradict each other.
   Problem: Section 4 lists contract grazing, and B12 lists manager-operator in the restructure outcomes, but the formula list stops at four options. An owner could also say "would not sell the land" and mark "sale" acceptable.
   Fix: Add one line per missing option (for example, grazing fee less K at risk and hours) or state that they are valued like lease or management company. Add "sale is acceptable only if you would sell the land".

4. [MINOR] Pre-G1 spend is sunk at G1 and counted only against self-run, and the wording on the screen is loose.
   Problem: The 60k set-up figure includes the pre-G1 spend. By G1 that money is spent whichever option wins, yet B12 charges it only to self-run. This is about 6k a year and does not change either example. Separately, B10 says a farm passes "by the margin screen", while the sheet says the screen is "necessary, not sufficient".
   Fix: Say that pre-G1 spend is excluded from the ranking at G1 (or charged to all options equally), and change B10 to "the margin screen is a necessary test; the B12 hurdle decides".

VERDICT: 1 MAJOR remaining
