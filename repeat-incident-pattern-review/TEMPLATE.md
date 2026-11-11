# Repeat incident pattern review

Capability template, version 0.1.0.

## Purpose

Compare a period of incident records, usually a year, and the actions recorded after them, and show where confirmed causes recur. The review groups incidents that share a confirmed cause category and a task or piece of equipment, shows the same confirmed cause across different tasks, shows tasks that have had several different causes, sets aside incidents whose cause is not yet confirmed, lists the gaps in the records and ends with numbered questions for the team. The assistant prepares; the investigation lead decides which pattern, if any, needs a closer look. The assistant investigates no single incident, finds no cause, blames no one, certifies nothing, and never changes a record, reports anything or sends anything.

## When to use it and when not to

Use it when a pattern is suspected, before a safety review or a planning round, or on a set rhythm such as once a year, when the register holds enough confirmed causes to compare (at least four confirmed incidents in the period).

Do not use it:

- to investigate one incident, find its causes or write its actions. Use the incident investigation and corrective actions capability for that;
- to decide whether an incident is reportable to an authority, whether a workplace is safe or compliant, or who is to blame;
- on a register that still carries names, contact details, ID numbers or medical details. De-identify it first;
- to rate or compare people, teams or contractors.

## Roles

- **Runs it:** the person who keeps the incident register, or whoever prepares it for the investigation lead.
- **Reads it and decides which pattern deserves a closer look:** the investigation lead, a qualified person the company names.
- **Confirms the causes in the register:** the investigation lead of each earlier incident. The assistant never recodes a cause.
- **Answers the questions:** the owners and managers the lead brings in.

## Inputs

1. **Incident register,** a spreadsheet export, one row per incident. Default column headers: `incident_ref, date, outcome, area, task_or_equipment, cause_status, cause_category, confirmed_cause`. Dates are written YYYY-MM-DD. `cause_status` is "Confirmed" when the investigation lead has agreed the cause; any other value, or a blank, counts as not confirmed. `cause_category` and `confirmed_cause` are used only for confirmed rows. If a header does not match, stop, show the expected and the found headers, and ask which column is which. Never guess.
2. **Action list,** a spreadsheet export, one row per action. Default column headers: `action_ref, incident_ref, action, owner_role, due_date, completed_date, check_result, check_date, status`. A blank `completed_date` means not completed, whatever the status says. If a header does not match, stop and ask, as above. If no action list is supplied, say "no action list supplied" and continue with the register only.
3. **Settings:**
   - the review period, start and end dates. If missing, stop and ask;
   - today's date. If missing, ask;
   - [your outcome order], lowest to highest. Default: Near miss; First aid; Medical treatment; Lost time. An outcome in the register that is not in the order: stop and ask where it goes;
   - [your small-group limit], default 3: a group with fewer incidents than this is shown with less detail (see the procedure);
   - the investigation lead's role.

The assistant works only from what the person supplies. It needs no access to any system and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Compare the headers of both lists with the defaults and stop on any mismatch. Stop if two incidents share a reference or two actions share a reference. Stop if a date is not in the stated form.
2. **Sort the register.** Rows dated inside the period, start and end included, are in scope. Rows outside are counted and listed with their dates and take no further part. Of those in scope, "Confirmed" rows are confirmed; the rest are not confirmed and are set aside for section 4.
3. **Keep names out.** If a name, an ID number, a phone number or an address appears in any column, do not repeat it. Replace it with the person's role, or leave it out, and tell the person which column held it and that the register should be cleaned before it is shared further.
4. **List the categories.** Count the confirmed incidents by `cause_category`, exactly as spelled. If two categories look alike (different wording or spelling, or one inside the other), do not merge them: print both and ask in the questions whether they are the same. Groups use the categories as supplied.
5. **Link the actions.** Attach each action to its incident by `incident_ref`. An action whose incident is not in the register, or is outside the period, is reported under record gaps and not used in any group.
6. **Section 1, same confirmed cause at the same task or equipment.** Group confirmed incidents with the same `cause_category` and the same `task_or_equipment`, as written. A group needs at least two incidents. Rank groups by number of incidents, then by number of incidents that came after an earlier action (step 8), then by the most recent date. Number them P1, P2. A confirmed row whose `cause_category` or `task_or_equipment` is blank cannot be grouped: list it under "Confirmed, matching nothing" in section 4 and name the blank field in section 5.
7. **Sections 2 and 3, the wider views.**
   - **Section 2:** a confirmed cause category that appears in two or more confirmed incidents at two or more different tasks or equipment. Number them C1, C2, ranked by number of incidents, then by the most recent date. An incident may appear in section 1 and here.
   - **Section 3:** a task or equipment with confirmed incidents under two or more different cause categories. Number them T1, T2, ranked the same way. Show each category with its incidents and its actions, and say which are already in a section 1 group.
8. **Work out the facts of each group.** From the dates and actions, and nothing else:
   - the number of incidents, the worst outcome by [your outcome order], and the date of the latest incident with the days from today to it;
   - the days between each pair of incidents in date order;
   - the earlier actions: the actions linked to an incident that is dated earlier than the group's latest incident, each with its incident, status, completed date and check result, or "no check result". The actions linked to the latest incident are not earlier actions; list them on their own line, "Actions for the latest incident", in the same form, or "none";
   - **after an earlier action:** an incident counts when its date is later than the completed date of an action linked to an earlier incident in the same group. Name the incidents and the actions. If the check date of that action is also earlier than the incident's date, say so. In section 2 the action was written for a different task, so add that the review does not compare what the action covered;
   - gaps: incidents with no action recorded, open actions past their due date with the days, completed actions with no check result.
9. **Protect small groups.** A group with fewer incidents than the small-group limit is shown with its incidents by month only, with the worst outcome, the count of actions and the after-action facts. Leave out areas, exact dates (the date of an action, a completion or a check as well as of an incident), days between, and the confirmed-cause wording. The refs stay. Months between replace days between. The same rule applies to a category line in section 3 that holds fewer incidents than the limit: show the month and outcome of each incident, its action refs with status and whether a check result is recorded, and no exact date, area or cause wording. A section 3 task that has such a line shows months between its incidents instead of days between, because day counts would give the exact dates back.
10. **Say nothing about sameness beyond the record.** A group exists because recorded fields match, never because descriptions sound alike. Two incidents with different confirmed categories are never joined, and an incident whose cause is not confirmed is never placed in a group. In section 4, state the field it shares with a group and say that no link is claimed.
11. **Section 4, not grouped.** List the not-confirmed incidents in scope with ref, month, outcome, area, task or equipment and the status as written. List any confirmed incident that matches nothing. Then the coverage line: confirmed incidents counted once, in the first section that holds them.
12. **Section 5, record gaps.** Confirmed incidents with no action recorded; not-confirmed incidents with no action recorded; open actions past due, with days; completed actions with no check result, as a count out of the completed; actions whose status and completed date disagree (closed with no completed date, or open with one); actions with no matching incident.
13. **Section 6, questions for the team.** Number them. One for each group or view that the facts raise, one for the gaps that bear on a group (gaps on the same group may share a question), one for the not-confirmed incidents that share a field with a group, one for any look-alike categories, and, if an excluded incident outside the period shares the category and task of a group and falls within 30 days of the period, one that asks whether that incident is to be included in a review of the group. The number of questions is not fixed. Each question carries its facts and refs. A question asks; it does not recommend, rank urgency or say what the pattern means.
14. **Return the review** to the person who ran it, for the investigation lead. The assistant decides which pattern needs a closer look for no one.

## Exceptions and stop conditions

- **No register, or no period:** stop and ask.
- **A header does not match:** stop, show the expected and the found headers, and ask. Never guess which column is which.
- **Duplicate references, a date that is not YYYY-MM-DD, or an outcome not in the order:** stop and ask.
- **Fewer than four confirmed incidents in the period:** say so and stop. There is not enough to compare. List the incidents by ref and month.
- **The register holds names or personal details:** do not repeat them; see step 3.
- **A group rests on one category spelled two ways:** do not merge them; ask.
- **Asked to investigate one incident, name its causes or write its actions:** decline and point to the incident investigation and corrective actions capability.
- **Asked to say who is to blame, whether an incident is reportable, whether the site is safe or compliant, or which pattern matters most:** decline. The investigation lead decides.
- **Asked to change a record, close or assign an action, or send the review to anyone:** decline and name the role that does it.
- **Asked to treat two incidents as the same cause because they sound alike:** decline; only the investigation lead's confirmed categories group incidents.

## Output format

```
REPEAT INCIDENT PATTERN REVIEW: [period start] to [period end]

For: [investigation lead role]. Prepared [today] from the incident register and the action list supplied.

Inputs checked: [n] incidents supplied; [n] inside the period; [n] outside it ([ref, date; ...] or "none"). Of those inside, [n] have a confirmed cause and [n] do not. [n] actions supplied; [n] linked to an incident inside the period. Small-group limit: [n]. Outcome order: [lowest to highest].
Confirmed cause categories as supplied: [category n; ...]. Categories that look alike: [none, or the pairs, asked in the questions].

1. SAME CONFIRMED CAUSE AT THE SAME TASK OR EQUIPMENT
[For a group with at least the limit:]
P[n]. [Cause category] at [task or equipment]: [n] incidents, worst outcome [outcome], latest [date] ([n] days before today).
  Incidents: [ref, date, outcome, area]; ... Days between: [n]; ...
  Confirmed causes as recorded: [ref: wording]; ...
  Earlier actions: [action ref, for ref, action, status, completed date or "not completed", check result or "no check result"]; ... [or "none"]
  Actions for the latest incident: [same form, or "none"].
  After an earlier action: [n] ([refs]), each dated after [action ref] was completed on [date]; [refs, or "none"] also after its check date.
  Gaps: [incidents with no action; open actions past due, with days; completed actions with no check result; or "none"].
[For a group below the limit:]
P[n]. [Cause category] at [task or equipment]: [n] incidents, shown by month because the group is below the small-group limit. Months: [ref, month year]; ... Months between: [n]. Worst outcome: [outcome]. Actions: [n] recorded, [n] completed, [n] with a check result. After an earlier action: [n] ([refs]). Gaps: [...].
[If none: None.]

2. SAME CONFIRMED CAUSE AT DIFFERENT TASKS OR EQUIPMENT
C[n]. [Cause category] at [n] tasks or equipment: [n] incidents, worst outcome [outcome], latest [date] ([n] days before today).
  Incidents: [ref, date, outcome, area, task or equipment]; ... Days between: [n]; ...
  Confirmed causes as recorded: [ref: wording]; ...
  Earlier actions: [as in section 1].
  Actions for the latest incident: [as in section 1].
  After an earlier action: [n] ([refs]), dated after [action ref] was completed on [date], written for a different task; this review does not compare what the action covered.
  Gaps: [...].
[A group below the limit is shown by month, as in section 1. If none: None.]

3. SAME TASK OR EQUIPMENT, DIFFERENT CONFIRMED CAUSES
T[n]. [Task or equipment]: [n] confirmed incidents under [n] cause categories, worst outcome [outcome], latest [date] ([n] days before today). Days between, in date order: [n]; ... [If any category line below is below the small-group limit, give "Months between, in date order: [n]; ..." instead.]
  [Category]: [n] ([refs]); [in section 1 group P[n], or "not in section 1"]. [A category with fewer incidents than the small-group limit: month and outcome of each incident, action refs with status and whether a check result is recorded; no exact date, area or cause wording. A category at or above the limit: each incident's date, outcome and confirmed cause as recorded, and its actions.]
  Also at this task, cause not confirmed: [refs, or "none"].
[If none: None.]

4. NOT GROUPED
Cause not confirmed: [ref, month year, outcome, area, task or equipment, status as written. Shares [field] with [group]; no link is claimed.] [Or: None.]
Confirmed, matching nothing: [refs, or "None"].
Coverage: [n] confirmed incidents: [n] in section 1, [n] more in section 2, [n] more in section 3, [n] in none.

5. RECORD GAPS
Confirmed incidents with no action recorded: [refs, or none].
Not-confirmed incidents with no action recorded: [refs, or none].
Open actions past due: [action ref, days]; [or none].
Completed actions with no check result: [refs] ([n] of [n] completed).
Status and dates that disagree: [refs, or none].
Actions with no matching incident in scope: [refs, or none].

6. QUESTIONS FOR THE TEAM
1. [Question, with its facts and refs.]
...

This review compares records only. For [investigation lead role] to decide which pattern, if any, needs a closer look. It investigates no single incident, finds no cause, assigns no blame, certifies nothing, and changes, sends and reports nothing.
```

## Reviewer checklist

1. Every group's incidents share the stated category and task or equipment in the register, character for character. (Register keeper)
2. No not-confirmed incident sits in a group, and none is described as linked. (Investigation lead)
3. Every day count and the "after an earlier action" facts recompute from the dates. (Register keeper)
4. Groups below the small-group limit show no exact date, area, days between or cause wording. (Investigation lead)
5. Every record gap named is a real gap in the exports. (Register keeper)
6. The questions ask and recommend nothing; none states what the pattern means. (Investigation lead)
7. No name, ID number or contact detail from the register was repeated. (Register keeper)
8. The coverage line adds up to the confirmed incidents in the period. (Register keeper)

## Acceptance tests

Proposed tests. None has been run.

1. **Normal year.** A register with three incidents sharing a category and equipment, one action completed before the third. Expected: one group in section 1 with full detail, days between correct, the third incident shown as after an earlier action.
2. **Pair below the limit.** Two incidents sharing category and equipment, limit 3. Expected: shown by month, no exact dates, no area, no cause wording.
3. **Sounds alike, differs.** Two incidents at one task with different confirmed categories. Expected: not placed in section 1; appear in section 3 only.
4. **Cause not confirmed.** An incident at the same equipment as a group with status "Under investigation". Expected: in section 4 with the shared field, "no link is claimed", never in the group.
5. **Renamed column.** `task_or_equipment` exported as `equipment`. Expected: stops, shows both header lists, asks.
6. **Category spelled two ways.** "Guarding" and "Machine guarding". Expected: both printed, not merged, a question asks.
7. **Closed with no date.** An action with status Closed and a blank `completed_date`. Expected: listed under status and dates that disagree and not counted as completed.
8. **Asked to investigate one event.** Expected: declines and points to the incident investigation capability.
9. **Names in the register.** A person's name in `confirmed_cause`. Expected: not repeated; the column is named; the person is asked to clean the register.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the whole output format above. Do not paste the block alone: it relies on the format for the exact wording of the sections and the closing line.

```
You prepare a repeat incident pattern review for an investigation lead.
You compare records only. You investigate no single incident, find no
cause, blame no one and certify nothing. You never change a record, close
or assign an action, report anything or send anything; a person approves
and does all of that.

The user will supply: an incident register export, an action list export
(if none, say "no action list supplied" and go on with the register), the
review period, today's date, the order of outcomes, and the smallest group
to show in full (default 3). Expected register headers: incident_ref,
date, outcome, area, task_or_equipment, cause_status, cause_category,
confirmed_cause. Expected action headers: action_ref, incident_ref,
action, owner_role, due_date, completed_date, check_result, check_date,
status. If a header does not match, stop, show expected and found, and
ask. If the period, today's date or the register is missing, stop and ask.
Stop on duplicate references, dates not in YYYY-MM-DD, or an outcome not
in the order. With fewer than four confirmed incidents in the period,
stop, say there is not enough to compare and list the incidents by ref
and month. Never ask for a password or a login code.

1. Rows in the period (start and end included) are in scope; count the
   rest and list them with their dates. Only rows with cause_status
   "Confirmed" can be grouped; the others go to section 4. A Confirmed row
   with a blank cause_category or task_or_equipment is not grouped: list
   it as "Confirmed, matching nothing" and name the blank field in
   section 5.
2. Never repeat a name, ID number or contact detail; say which column
   held it and that the register should be cleaned.
3. Use cause categories exactly as spelled. If two look alike, print both
   and ask; never merge.
4. Section 1: confirmed incidents with the same cause_category and the
   same task_or_equipment, two or more; number P1, P2 by incident count,
   then incidents after an earlier action, then latest date. Section 2: a
   category at two or more different tasks; section 3: a task with two or
   more categories. Number C and T groups by incident count, then latest
   date. An action whose incident is not in scope goes to record gaps and
   into no group.
5. For each group: incident count, worst outcome, latest date and days
   from today, days between incidents, earlier actions, and gaps. Earlier
   actions are the actions linked to an incident dated earlier than the
   group's latest incident, each with status, completed date and check
   result (or "no check result"); list the actions of the latest incident
   separately as "Actions for the latest incident". An incident is "after
   an earlier action" when its date is later than that action's completed
   date; also say if it is later than the check date; in section 2 add that
   the action was written for a different task and the review does not
   compare what it covered. A blank completed_date means not completed,
   whatever the status says.
6. A group, or a section 3 category line, below the small-group limit is
   shown by month only, with worst outcome and action counts (or action
   refs with status), and no area, exact date, days between or cause
   wording; use months between. Exact dates of actions and checks are
   left out too. A section 3 task with such a line gets months between,
   not days between.
7. Group only on recorded fields. Descriptions that sound alike prove
   nothing. A not-confirmed incident is never placed in a group; say what
   field it shares and that no link is claimed.
8. Write dates as 18 Nov 2025 and months as Nov 2025. Print the coverage
   line: each confirmed incident counted once, in the first section that
   holds it.
9. List the record gaps, including actions marked closed with no
   completed date and actions with no matching incident. Then numbered
   questions with their facts and refs: one for each group or view, one
   for the gaps on a group, one for the not-confirmed incidents that share
   a field with a group, one for look-alike categories, and, if an
   excluded incident dated within 30 days outside the period has the same
   category and task as a group, one that asks whether it is to be
   included in a review of that group. Questions ask; they never
   recommend, rank urgency or say what the pattern means.
10. Use the output format exactly. Print "None." for an empty section.
    Recompute every count and day before you print it.

Decline to investigate one incident, name blame, say whether anything is
reportable or the site safe, or treat incidents as the same cause because
they sound alike. The investigation lead decides which pattern matters.
```

## What to customize

- Your cause categories, agreed with the investigation leads and kept stable.
- [your outcome order] and [your small-group limit].
- The review period and how often it runs.
- Who keeps the register, who reads the review and who decides.
- Where the review is kept and who may see it.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Not yet tested in a client environment. Incidents outside the period are listed with their exact dates, because the 30-day question needs them, even when one shares a category and equipment with a group below the small-group limit.
