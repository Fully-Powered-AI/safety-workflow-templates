# Emergency drill brief: one trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in `public/example.md` (the five input blocks under "The inputs"). No client data was used. This record is of the third run. The first run, on the first version of the template, is not kept (the second run's record is also replaced by this one): it found that the example's decisions were not in the order the template's own rule gives, that the run sheet left out the "By" part of some steps, and several places where the instructions were open. The template and the example were then edited, and this run followed the edited instruction block and output format. This is one run, not a test for a client, and not a test in any other product.

Two things to know about how fair the trial is. The run was not blind: the example file was read in one go, so the example's published output was seen before the brief below was written, and the earlier run's record was in view too. And the run was made by the assistant that made the edits, not by an independent reviewer. The template was edited a second time after the second run, on a reviewer's points: the output format's "Not covered" section gained a sentence naming three things the brief does not check, a few rules from the procedure were added to the instruction block, and the example's decisions were made fuller. The earlier record was in view when this run was made, and this run's brief is the earlier one with the new sentence in "Not covered"; the rest was checked line by line against the example's inputs and the edited instruction block. This run therefore shows that the template can be followed to the same result. It does not show that a model that had not seen the answer would reach it. Treat the comparison below with that in mind.

## What came out

**EMERGENCY DRILL BRIEF: fire evacuation, Unit 4, Company A (workshop and first-floor office)**

Date: Wednesday 18 November 2026, 10:30 to 11:00. Prepared: Tuesday 10 November 2026, from the drill details, the arrangements list (7), the roles list (4), the previous findings (3).
Approver: Site manager. Drill lead: Operations coordinator.
Scenario: approved by the Site manager on Monday 9 November 2026 (as supplied).
Announced in advance to: Site manager, drill lead, the two observers. Not announced to: everyone else.
Expected at roll call: 34 (workshop 26, office 7, visitors 1).
Counts: arrangements 7; roles 4; previous findings 3; observation points 7. Flags: 4.

**The question this drill answers**

Does everyone reach the assembly point, and is everyone counted, within our targets when exit D2 cannot be used? Source: supplied.

**The scenario**

A fire is reported in the glue store at the back of the workshop. Exit D2 is unusable. The office must leave by the internal stair. A visitor is signed in.
Pretended: the fire in the glue store, and exit D2 being unusable.
Real: the alarm sounds, people leave and assemble; nothing is lit and nothing is moved.
Stop the drill if: a real emergency happens, anyone is hurt, or the drill lead calls it off.

**Run sheet**

1. 10:15. The drill lead puts a "blocked" sign across D2; the door stays closed. By: Drill lead. Arrangement: A03.
2. 10:30. The alarm is sounded from the call point by the front desk. By: Drill lead. Arrangement: A01.
3. From the alarm. The workshop leaves by D1. By: Workshop fire warden (R01). Arrangement: A02.
4. From the alarm. The office leaves by the internal stair, then out through D1. By: Office fire warden (R02). Arrangement: A04.
5. 10:35. Everyone is at the assembly point, the visitor car park by the gate (target: 5 minutes after the alarm). By: everyone on site. Arrangement: A05.
6. 10:38. Roll call complete (target: 8 minutes after the alarm). Each fire warden counts their own area; the visitor log is taken to the assembly point. By: R01, R02 and the Visitor log holder (R03). Arrangement: A06.
7. After the roll call. The all clear is given in person; nobody re-enters until then. By: Site manager (R04). Arrangement: A07.

**Gaps in the arrangements list**

- Help for people who cannot use the stairs or need assistance to leave: no arrangement on the list. FLAG, arrangement not supplied. See decision 1.

**Roles for the drill**

- R01 Workshop fire warden. Duty: clears the workshop and counts people at the assembly point. Holder: Shift supervisor. Deputy: Machine operator lead. On the day: neither reported away.
- R02 Office fire warden. Duty: clears the office and counts people at the assembly point. Holder: Accounts clerk. Deputy: Receptionist. On the day: holder away (Monday 16 to Friday 20 November 2026); the deputy is named and not reported away. FLAG, holder away. See decision 2.
- R03 Visitor log. Duty: takes the visitor log to the assembly point. Holder: Receptionist. Deputy: Operations coordinator. On the day: neither reported away.
- R04 Site manager. Duty: gives the all clear. Holder: Site manager. Deputy: none. On the day: not reported away.

**Observers**

- Maintenance technician: workshop and assembly point. Holds no duty in the roles list.
- Receptionist: office. Holds a duty: holder of R03, and deputy of R02, which the Receptionist would cover on the day because the R02 holder is away. FLAG, observer holds duties. See decision 3.

**What to observe**

- O01 Alarm (A01). Watch for: whether the continuous bell is heard in the workshop and in the office. Record: heard yes or no at each observer's position, and how many people say they did not hear it. Observers: Maintenance technician (workshop), Receptionist (office). Previous finding: F03.
- O02 Exit (A02), workshop front exit D1. Watch for: the workshop leaving by D1. Record: the time the first and the last person pass D1, and whether a queue forms (yes or no). Observer: Maintenance technician.
- O03 Exit (A03), workshop rear exit D2. Watch for: the door staying closed with the sign across it, and whether anyone goes to it. Record: the floor zone in front of D2 (from F02) clear or not clear at 10:15, and the number of people who go to D2. Observer: Maintenance technician. Previous finding: F02.
- O04 Route (A04), office to the internal stair and out through D1. Watch for: the office leaving by that route. Record: the time the last person leaves the office. Observer: Receptionist.
- O05 Assembly point (A05), visitor car park by the gate. Watch for: people arriving. Record: the time the last person arrives, against the 10:35 target. Observer: Maintenance technician.
- O06 Roll call (A06). Watch for: each fire warden counting their own area and the visitor log arriving. Record: whether the visitor log is at the assembly point when the roll call starts, the time the roll call completes against 10:38, and the total counted against 34 expected. Observer: Maintenance technician. Previous finding: F01.
- O07 All clear (A07). Watch for: the all clear given in person. Record: the time it is given, and the number of people who re-enter before it. Observer: Maintenance technician (area taken from the run sheet).

**Findings from earlier drills**

- F01 (2 March 2026). Roll call for the office took 9 minutes because the visitor log was left at reception. Action: visitor log kept in a grab folder by the front desk. Status: done. To look at on this drill: O06, to see whether the fix holds.
- F02 (2 March 2026). Exit D2 was blocked by pallets. Action: floor zone marked in front of D2 and checked weekly. Status: open. To look at on this drill: O03, as still open.
- F03 (2 March 2026). Two people on the first floor did not hear the alarm. Action: check the bell volume in the meeting room. Status: not stated. To look at on this drill: O01. FLAG, status not stated. See decision 4.

**Debrief questions** (Wednesday 18 November 2026, 14:00)

1. O01. Who did not hear the alarm, and where were they?
2. O02. Did the workshop use D1? When did the first and last person pass it, and did a queue form?
3. O03. Was the floor zone in front of D2 clear at 10:15? How many people went to D2, and what did they do next?
4. O04. When did the last person leave the office?
5. O05. When did the last person reach the assembly point, against the 10:35 target?
6. O06. Was the visitor log at the assembly point when the roll call started? Was the roll call complete by 10:38, and did the count match the 34 expected?
7. O07. When was the all clear given, and how many people re-entered before it?
8. What happened that nobody planned for?
9. What did people tell you they found confusing?
10. Which observations need an action, who owns each, and by when? The Site manager decides.

**Decisions for the Site manager: 4**

1. Gaps, arrangement not supplied. The arrangements list has no arrangement for people who cannot use the stairs or need assistance to leave. The brief cannot set an observation point for something that is not written. Is there an arrangement to add to the list, and should it be observed?
2. R02, holder away. The Accounts clerk, holder of the Office fire warden role, is away on the drill date. The deputy, the Receptionist, is named and not reported away. Does the Receptionist cover R02 in this drill, or is someone else named?
3. Observers, observer holds duties. The Receptionist is the observer for the office and also holds R03 and is deputy for R02. The office is observed only by the Receptionist. Who observes the office if the Receptionist is carrying the visitor log or counting the office?
4. F03, status not stated. The earlier finding about the bell volume has an action and no status. O01 will look at it. Has the bell volume in the meeting room been checked?

**Not covered**

This brief does not direct a live emergency, does not show that a rescue can be carried out, is not an emergency plan and does not say what any law or regulator requires. It does not check how much one observer carries, whether two observation points fall at the same moment in different places, or whether an absence is inside the expected numbers; the Site manager looks at those when approving. It records what to watch and ask; the Site manager decides what the drill showed.

Draft for the Site manager's approval. Nothing has been announced, sent or run.

## What was observed

Every part of the output format was produced, and no stop condition was met: the five required drill details, the arrangements list and the headers were all present, no ID was repeated, a scenario was supplied and marked approved, the scenario asks for nothing real, and the expected total (26 + 7 + 1 = 34) agrees with its parts. Every time on the run sheet is a supplied time (10:15, 10:30) or the 10:30 start plus a supplied target (10:35, 10:38). The counts in the header match the body: 4 flags, 4 decisions, 7 observation points. The decisions run in the order of the brief: gaps, roles, observers, earlier findings.

### Differences from the published example

- **Wording only.** Some run-sheet steps, the observation points, the debrief questions and the decision texts are worded differently, and the decision texts are a little fuller in this run. No flag, count, time or decision differs. The "Not covered" section is identical to the example's.
- **Observer for the roll call and the all clear.** Both the example and this run give O06 and O07 to the Maintenance technician, and both mark O07 as taking its area from the run sheet, as the edited template now asks. This was a guess in the first run.

### Facts not in the inputs

None found in this run's output. The D2 floor zone in O03 comes from finding F02's action, and is marked "(from F02)", as the edited template allows. Every figure in the example's output traces to an input as well.

### What the edits closed, and what this run did not test

Closed since the first run: the order of the decisions is written into the instruction block; each run-sheet step ends "By", with "everyone on site" for a step everyone does; observation points record a count in place of a description; a finding's action may supply a watch item; a point with no stated area takes the area of the step before it; an observer who holds and covers duties is one flag; the gaps section holds only flags or "none"; the instruction block now carries the rules about quoting targets and counts and about the order of the decisions.

Left to the responsible person, and now said so in the template and in every brief's "Not covered" section rather than guessed: how much one observer carries and whether two points happen at once in different places (the Maintenance technician holds five points, and nothing was flagged); whether an absence is among the expected numbers (the Accounts clerk is away, and the inputs do not say whether the 7 expected in the office includes that person); and whether the 10:15 set-up could tip off people who were not told.

### Shortcomings

- Nothing here shows how the template behaves when inputs are missing, wrong or contradictory. The other fourteen acceptance tests in the template were not run.
- The run was not blind and not independent. A different model or session, without the published output in view, may produce a different brief.
- This is one run by one model.
