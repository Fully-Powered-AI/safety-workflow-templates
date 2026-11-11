# Repeat incident pattern review: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (`claude-sonnet-5-5`)
- **Date:** 2026-11-10

The inputs are the invented example in [example.md](example.md) (an invented packaging and dispatch plant). No client data was used. The run was a single attempt by a model that did not write the template. One thing weakens it: the example file was read in one piece, so the published review was seen before this one was produced. The review below was still worked out from the inputs, with the day counts recomputed by script, but it is not a blind run and the likeness to the published review should be read with that in mind.

## Inputs used

The "The inputs" part of [example.md](example.md): the settings (period 1 November 2025 to 31 October 2026, today 2 November 2026, the four-step outcome order, small-group limit 3, the operations manager as investigation lead), the register of 13 incidents and the action list of 9 actions.

## What came out

```
REPEAT INCIDENT PATTERN REVIEW: 1 Nov 2025 to 31 Oct 2026

For: the operations manager. Prepared 2 Nov 2026 from the incident register and the action list supplied.

Inputs checked: 13 incidents supplied; 12 inside the period; 1 outside it (INC-101, 20 Oct 2025). Of those inside, 10 have a confirmed cause and 2 do not. 9 actions supplied; 9 linked to an incident inside the period. Small-group limit: 3. Outcome order: Near miss; First aid; Medical treatment; Lost time.
Confirmed cause categories as supplied: Pedestrian segregation 3; Housekeeping 3; Machine guarding 2; Maintenance 1; Training 1. Categories that look alike: none.

1. SAME CONFIRMED CAUSE AT THE SAME TASK OR EQUIPMENT
P1. Pedestrian segregation at Forklift at dock: 3 incidents, worst outcome Medical treatment, latest 22 Jul 2026 (103 days before today).
  Incidents: INC-102, 18 Nov 2025, Near miss, Dispatch; INC-106, 3 Mar 2026, Near miss, Dispatch; INC-111, 22 Jul 2026, Medical treatment, Dispatch. Days between: 105; 141.
  Confirmed causes as recorded: INC-102: No marked walkway between dock door 2 and the packing bench; INC-106: Pedestrian door at the dock opens onto the forklift route with no warning; INC-111: No stop line or mirror where the dock exit meets the walkway.
  Earlier actions: A-31, for INC-102, Paint a marked walkway from dock door 2 to the packing bench, Closed, completed 12 Dec 2025, no check result; A-49, for INC-106, Fit a warning light on the pedestrian door at the dock, Closed, completed 10 Apr 2026, no check result. (A-66 and A-67 belong to INC-111, the latest incident, so they are not earlier actions: A-66, Fit a convex mirror and a stop line at the dock exit, Open, not completed, no check result; A-67, Review the dock traffic plan with the team, Closed, completed 14 Oct 2026, no check result.)
  After an earlier action: 2 (INC-106, INC-111). INC-106 is dated after A-31 was completed on 12 Dec 2025; INC-111 is dated after A-31 and after A-49 was completed on 10 Apr 2026; none also after a check date (no check dates recorded).
  Gaps: A-66 open, 33 days past due. A-31, A-49 and A-67 completed with no check result. Every incident has an action.

P2. Machine guarding at Pallet wrapper: 2 incidents, shown by month because the group is below the small-group limit. Months: INC-104, Feb 2026; INC-109, May 2026. Months between: 3. Worst outcome: First aid. Actions: 1 recorded, 1 completed, 1 with a check result. After an earlier action: 1 (INC-109, also after that action's check date). Gaps: INC-109 has no action recorded.

2. SAME CONFIRMED CAUSE AT DIFFERENT TASKS OR EQUIPMENT
C1. Housekeeping at 3 tasks or equipment: 3 incidents, worst outcome First aid, latest 30 Jun 2026 (125 days before today).
  Incidents: INC-103, 2 Dec 2025, First aid, Packing, Packing bench; INC-107, 15 Apr 2026, First aid, Returns, Returns area; INC-110, 30 Jun 2026, Near miss, Goods in, Dock plate. Days between: 134; 76.
  Confirmed causes as recorded: INC-103: No end-of-shift clean-down step for the packing bench; INC-107: No end-of-shift clean-down step in the returns area; INC-110: Dock plate area not covered by any clean-down step.
  Earlier actions: A-38, for INC-103, Add an end-of-shift clean-down step to the packing checklist, Closed, completed 6 Feb 2026, no check result. (A-61, for INC-110, Open, not completed, is for the latest incident.)
  After an earlier action: 2 (INC-107, INC-110), dated after A-38 was completed on 6 Feb 2026, written for a different task; this review does not compare what the action covered.
  Gaps: INC-107 has no action recorded. A-61 open, 94 days past due. A-38 completed with no check result.

3. SAME TASK OR EQUIPMENT, DIFFERENT CONFIRMED CAUSES
T1. Forklift at dock: 5 confirmed incidents under 3 cause categories, worst outcome Medical treatment, latest 22 Jul 2026 (103 days before today). Days between, in date order: 98; 7; 64; 77.
  Pedestrian segregation: 3 (INC-102, INC-106, INC-111); in section 1 group P1.
  Maintenance: 1 (INC-105); 24 Feb 2026, Medical treatment, Brake wear not on the forklift service sheet. Action A-47, Add brake wear to the forklift service sheet, Closed, completed 27 Mar 2026, no check result. Not in section 1.
  Training: 1 (INC-108); 6 May 2026, First aid, Temporary driver started without the dock induction. Action A-55, Hold a dock induction for temporary drivers before their first shift, Closed, completed 4 Jun 2026, check result "Induction record seen for all four temporary drivers" on 10 Jun 2026. Not in section 1.
  Also at this task, cause not confirmed: INC-112.

4. NOT GROUPED
Cause not confirmed: INC-112, Sep 2026, Near miss, Dispatch, Forklift at dock, Under investigation. Shares the task with P1 and T1; no link is claimed. INC-113, Oct 2026, First aid, Packing, Pallet wrapper, Not investigated. Shares the equipment with P2; no link is claimed.
Confirmed, matching nothing: None.
Coverage: 10 confirmed incidents: 5 in section 1, 3 more in section 2, 2 more in section 3, 0 in none.

5. RECORD GAPS
Confirmed incidents with no action recorded: INC-107, INC-109.
Not-confirmed incidents with no action recorded: INC-112, INC-113.
Open actions past due: A-61, 94 days; A-66, 33 days.
Completed actions with no check result: A-31, A-38, A-47, A-49, A-67 (5 of 7 completed).
Status and dates that disagree: none.
Actions with no matching incident in scope: none.

6. QUESTIONS FOR THE TEAM
1. P1: INC-106 is dated after A-31 was completed (12 Dec 2025), and INC-111 after A-31 and A-49 (10 Apr 2026). Neither action has a check result. What was each action meant to change, and what check was planned?
2. P1: A-66 (mirror and stop line, for INC-111, Medical treatment) is 33 days past due. What is its current date, and what is in place at the dock exit meanwhile?
3. P2: INC-109 is dated after A-44 was completed and after its check date, and has no action recorded. Does its confirmed cause describe the same condition as INC-104's? (Cause wording is not shown for a group below the limit; it is in the register.)
4. C1: INC-103, INC-107 and INC-110 each record a missing clean-down step in a different place. A-38 covers the packing bench only, INC-107 has no action, and A-61 is 94 days past due. Which actions cover which places?
5. T1: five confirmed incidents at the forklift at dock fall under three categories (INC-102, INC-106, INC-111; INC-105; INC-108), with actions held by the warehouse lead (A-31, A-49, A-66), the maintenance lead (A-47) and the operations manager (A-55, A-67). Who reviews the dock's actions together?
6. Gaps: 5 of 7 completed actions have no check result (A-31, A-38, A-47, A-49, A-67). Which of them have a check planned, and when?
7. INC-112 (Under investigation) shares its task with P1 and T1. When is its cause expected to be confirmed?
8. INC-113 (Not investigated) shares its equipment with P2. When is its cause expected to be confirmed?
9. INC-101, dated 20 Oct 2025 (12 days before the period starts), has the same cause category and equipment as P2. Is it to be included in a review of P2?

This review compares records only. For the operations manager to decide which pattern, if any, needs a closer look. It investigates no single incident, finds no cause, assigns no blame, certifies nothing, and changes, sends and reports nothing.
```

## What was observed

- **All six sections and the closing line were produced,** in the order and form of the output format. Nothing in the instructions made the run stop: the headers matched, no reference was repeated, every date was in the stated form, every outcome was in the order, there were ten confirmed incidents, and the register held no names or personal details to leave out.
- **The counts and day counts were recomputed by script** (105 and 141 days; 134 and 76; 98, 7, 64 and 77; 103 and 125 days since the latest incidents; 33 and 94 days past due) and match the published example. Coverage adds up to 10.
- **Differences from the published example.** The group results, gaps and counts are the same. The wording and the questions differ:
  - The example lists A-66 and A-67 among P1's "earlier actions". They belong to INC-111, the latest incident in that group, so they are not earlier than anything in it. This run set them apart in brackets. The template does not say whether a group's "earlier actions" include the latest incident's own actions, so both readings are possible.
  - The example gives the exact date of A-44's check (20 April 2026) in the small group P2 and again in its question 3. The template says a group below the limit shows no exact date. The example breaks its own rule 9 and checklist item 4 there; this run left the date out.
  - The example has seven questions; this run has nine, because it wrote one for the check-result gap, one for each of the two unconfirmed incidents and a separate one for the dock's whole set of actions. The example's question 5 ("so that the three causes are not each handled by a different owner on a different timetable") and question 7 ("Should the review be run again with the period starting earlier?") lean toward saying what the pattern means or what to do, which checklist item 6 forbids. This run's questions ask for facts and dates only.
  - Section 3 in the example does not name "Not in section 1" for the two single-incident categories; this run did, as the output format says.
- **Facts in either output that are not in the inputs.** None in this run beyond arithmetic on the dates. In the example, "about eight months" (question 5) is not in the inputs but is derived from them (18 Nov 2025 to 22 Jul 2026).
- **Where the instructions were ambiguous, and a guess was needed:**
  - Whether a group's "earlier actions" include actions written for the latest incident in it (above).
  - The order in which C and T groups are numbered; only section 1 has a ranking rule.
  - The date style for the output; the input is YYYY-MM-DD and the format shows only "[date]", so "18 Nov 2025" was a choice. The example makes the same choice.
  - How many questions are required. Step 13 asks for "one for each gap that bears on a group", which could mean a dozen questions; this run grouped related gaps into one question.
  - Whether the small-group rule (no exact dates) also covers the one-incident category lines in section 3, which the format shows with a full date. This run showed the date, since the section 3 task as a whole had five incidents.
  - What to do with a row marked "Confirmed" whose category or task is blank. The template does not say; the example register has none.
  - "Not investigated" is not a value the template names; it counts as not confirmed because the rule says any other value does.
- **Shortcomings of the trial itself:** one run, one model, and not blind to the published review (see the top). It shows the instructions can be followed to a complete review on this input. It does not show how the template behaves on a messy real register, on the stop conditions (none was triggered), or in other products.

## Changed after the run recorded above, and not run again

The output and the observations above are as recorded. They describe the template and the example as they stood at the run. After an independent review, these changes were made to the published files on 10 November 2026, and the template was not run again on the example:

- **The example's small group.** The dates were taken out of P2 and out of question 3, so the example now follows the small-group rule it had broken, as the run did.
- **"Earlier actions."** The template now defines them: the actions linked to an incident dated earlier than the group's latest incident. The actions of the latest incident are listed on their own line, "Actions for the latest incident", in the output format, the pasted instructions and the example. The example no longer lists A-66, A-67 or A-61 as earlier actions, as the run did not.
- **The example's questions.** Question 5 now asks who reviews the dock's actions together; question 4 asks which actions cover the three places and who owns each; question 7 asks whether INC-101 is to be included in a review of P2. The template now words the 30-day question that way. None of the questions steers toward a remedy.
- **Section 3.** A category line with fewer incidents than the small-group limit now follows the small-group rule: month and outcome, action refs with status, no exact date or cause wording. The example's lines for INC-105 and INC-108 were shortened to match. The run had shown their dates; that part of the template now differs from what was run.
- **Ambiguities the run found.** The template and the pasted instructions now say how C and T groups are numbered (incident count, then latest date), the date style (18 Nov 2025; Nov 2025), that the number of questions is not fixed and gaps on one group may share a question, and that a Confirmed row with a blank category or task is listed as matching nothing and named in the record gaps.
- **The pasted instructions** now begin with the line "Paste this block as custom instructions, followed by the output format above." and carry the rules that were only in the procedure: the coverage line, actions with no matching incident, months between, the 30-day question, the "no action list supplied" case and the stop when today's date is missing.
- **The example's layout.** The review is now in a plain block with plain headings and two-space indents, as the output format has it, and the added line "Every incident has an action." was removed from P1.

- **Later minor edits (after a second review).** Section 3 now shows months between, not days between, for a task that has a category line below the small-group limit (the example's T1 now reads "Months between, in date order: 3; 1; 2; 2"), so day counts cannot give back the exact dates the small-group rule leaves out. The pasted instructions now carry the section 2 wording about an action written for a different task, and the line before the block says to paste it with the whole output format. Out-of-period incidents keep their exact dates, noted in the template's version notes. The example's question 4 now quotes the text of A-38 instead of saying what it covered. The recorded run above shows T1 with days between, as it was run; these edits were not run again.

These changes have not been tried. The example's published review was edited by hand to match the changed template, not produced by a new run.
