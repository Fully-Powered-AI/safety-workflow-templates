# Ergonomic review inputs: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs are the template's own invented example, in `public/example.md`: an invented 30-person home-goods fulfilment company, an invented task and invented people. No client data was used. The run used the six inputs in that file (referral brief, task steps, observation notes, measurements table, worker feedback, photograph list), as written, with no change to any input.

This is the third run. The first, earlier on 10 November 2026 with Claude Sonnet 5.5, was done by an assistant that did not write the template and read the published example output only after its own record was finished. An independent review of it found that the cycles-per-shift rule was only right for an observation of exactly one hour, that the example left out the paper dispenser's height, listed a shelf height the inputs do not mention and said nothing of a difference between the counted rate and the step times, and that the totals line had one person label for two people observed. The template was revised and a second run made by the assistant that revised it. Its published record was then failed by a second independent review, for these reasons: the line "WHERE THE INPUTS DISAGREE" read 2 although three disagreements followed and the header said 3, and the trial's commentary did not notice; the instruction block left out three rules the procedure states (a label weight is shown as read from a label, stop when the brief covers two tasks, the total is the sum of the step times); the missing-figure lines said "Carrying" where the notes say "lifts"; two open choices the second run recorded (whether taking a carton off a shelf is a lift, and whether a loosely stated distance is already given) were not settled in the template; and "why referred: both" read awkwardly. The first and second runs' outputs are not republished.

After the second review the template was revised again. The instruction block now carries the three omitted rules; the procedure and the block say that the movement word is the notes' own, that taking something off a shelf is reaching unless the notes call it a lift, and that a height or distance stated loosely is recorded as such and still listed as missing; the format reads "worker complaint and assessor referral" for why referred; and the count heading was corrected. The example's output was corrected to match.

This third run was done by the assistant that made those revisions, which had read the reviews and the example before it ran. It is therefore not an independent run, and it is expected to agree with the corrected example; its record is the example's output, checked line by line against the instruction block and output format (version 0.1.0) on the example's inputs. The record is given in full below.

After this run the template received wording-only edits that were not re-run: the format's totals line now reads "hour or hours observed" and "x [n] hours" to match the example, "Observed by" is on its own line in the format, and two rules already in the procedure (step times taken on one person and applied to another; whether a missing figure is measured, counted or observed) were added to the instruction block. The record below is unchanged.

## What came out

```
ERGONOMIC TASK OBSERVATION RECORD: Packing a boxed table lamp into a shipping
carton at pack station 3

Location: Warehouse, pack station 3
Why referred: worker complaint and assessor referral, as stated: packing team
raised aching shoulders at the team meeting on Thursday 5 November 2026;
assessor visit booked.
Prepared for: external ergonomics assessor, visit on Tuesday 17 November 2026.
People who do the task: packers (4 across two shifts). Shift and break pattern:
07:00 to 15:30; breaks of 15 minutes at 10:00 and 30 minutes at 13:00 (stated
by the supervisor).
Observed: Tuesday 10 November 2026, 07:30 to 08:30 (one hour); 2 packers.
Observed by: warehouse supervisor.
Sources: referral brief; task steps; observation notes of 10 November 2026;
measurements, 8 rows; worker feedback, 2 people asked; photographs and video,
3 files
Steps: 4. Measurements supplied: 8. Measurements missing: 9. Disagreements: 3.

STEP RECORD

S1. Take a flat carton from the stack on the shelf beside the bench, fold it
and tape the base
  Movements as described: reaches up to the shelf to the right of the bench
  and takes a carton; stands at the bench; folds the carton; tapes the base
  Time for this step in one cycle: about 25 seconds
  (stopwatch, packer A, typical of 5 cartons)
  Load: none described
  Heights and distances: shelf height and reach distance not given
  Measured: none
  Not measured: M1 shelf height; M2 reach distance to the carton stack
  Worker feedback on this step: shoulder ache worst when reaching up for
  cartons on the shelf (1 of 2 asked)

S2. Lift the lamp box from the trolley to the bench
  Movements as described: lifts one box from the trolley, which sits low; puts
  it on the bench about two steps away
  Time for this step in one cycle: about 3 seconds
  (stopwatch, packer A, typical of 5 cartons)
  Load: lamp box, 4.2 kg (printed on the box label, not weighed); the notes say
  about 3 kg (see D1)
  Heights and distances: bench height 92 cm (measured; the notes say the box is
  put on the bench); trolley height stated as "low", distance stated as "about
  two steps"
  Measured: box weight 4.2 kg (label); bench height 92 cm (tape measure)
  Not measured: M3 trolley height; M4 distance from the trolley to the bench
  Worker feedback on this step: none

S3. Wrap the lamp and place it in the carton with paper fill, close the lid and
tape it
  Movements as described: stands at the bench; wraps the lamp in paper with
  both hands; reaches right to the paper dispenser; places the lamp in the carton;
  closes the lid; tapes it
  Time for this step in one cycle: about 120 seconds
  (stopwatch, packer A, typical of 5 cartons)
  Load: none described
  Heights and distances: bench height 92 cm (measured); reach distance to the
  dispenser and its height not given
  Measured: bench height 92 cm (tape measure)
  Not measured: M5 reach distance to the paper dispenser; M6 height of the
  paper dispenser
  Worker feedback on this step: none

S4. Lift the packed carton onto the roller conveyor beside the bench
  Movements as described: lifts the packed carton off the bench; puts it on the
  conveyor on the packer's left, about one pace away; turns at the waist with
  feet kept in place
  Time for this step in one cycle: about 4 seconds
  (stopwatch, packer A, typical of 5 cartons)
  Load: packed carton, 6.4, 6.5 and 6.6 kg (bench scale), mean 6.5 kg
  Heights and distances: bench height 92 cm (measured; the notes say the carton
  is lifted off the bench); conveyor height 88 cm (measured); distance stated as
  "about one pace"
  Measured: packed carton weight 6.4, 6.5 and 6.6 kg (bench scale); bench height
  92 cm and conveyor height 88 cm (tape measure)
  Not measured: M7 distance from the bench to the conveyor; M8 extent of the
  turn at the waist
  Worker feedback on this step: twisting round to the conveyor feels awkward
  (1 of 2 asked)

TASK TOTALS (arithmetic on the supplied figures; cycles are estimated from the
observed period)
Working time stated per shift: 6.0 hours, 360 minutes (from the rota; excludes
breaks and other duties)
Packer A: 20 cycles in the observed hour (1.0 hour), estimated 120 cycles per
shift (20 cycles / 1.0 hour observed x 6.0 hours).
  Time per step per shift: S1 50.0 min; S2 6.0 min; S3 240.0 min; S4 8.0 min;
  total 304.0 min.
  Check against the stated working time: within (304.0 of 360 minutes).
  Weight lifted per shift: S2 120 x 4.2 kg = 504.0 kg; S4 120 x 6.5 kg =
  780.0 kg.
Packer B: 22 cycles in the observed hour (1.0 hour), estimated 132 cycles per
shift (22 cycles / 1.0 hour observed x 6.0 hours).
  Time per step per shift: S1 55.0 min; S2 6.6 min; S3 264.0 min; S4 8.8 min;
  total 334.4 min.
  Check against the stated working time: within (334.4 of 360 minutes).
  Step durations were timed on packer A and applied to packer B.
  Weight lifted per shift: S2 132 x 4.2 kg = 554.4 kg; S4 132 x 6.5 kg =
  858.0 kg.

WORKER FEEDBACK NOT TIED TO A STEP (as reported, by role; not assessed)
- Packers (2 of 2 asked): shoulders ache by late afternoon.
- Packers (2 of 2 asked): the 10:00 break is often skipped when orders are
  running late (see D2).

CHANGES SUGGESTED BY THE PEOPLE WHO DO THE TASK (recorded as said; not assessed)
- Packer (1 of 2 asked): the cartons on a lower shelf. Step 1.
- Packer (1 of 2 asked): the conveyor turned to face the bench. Step 4.

PHOTOGRAPHS AND VIDEO (listed, not interpreted)
- pack3_shelf.jpg: the carton shelf seen from the bench (as described by the
  supervisor)
- pack3_bench.jpg: the bench with the trolley beside it (as described by the
  supervisor)
- pack3_conveyor.jpg: the conveyor and the bench from above (as described by the
  supervisor)

WHERE THE INPUTS DISAGREE: 3
D1. Lamp box weight. The observation notes say "about 3 kg"; the measurements
give 4.2 kg, read from the box label. The totals use 4.2 kg. Has a box been
weighed? For: supervisor.
D2. Breaks. The brief and the notes say breaks are taken at 10:00 and 13:00 as on
the rota; both packers asked say the 10:00 break is often skipped when orders are
running late. The totals use the stated working time of 6.0 hours. How often is
the break skipped, and how does that change the time on the station? For:
supervisor.
D3. Cycle time. Packer A's step times add up to 152 seconds a cycle (25 + 3 +
120 + 4), but 20 cycles were counted in 60 minutes, which is 180 seconds a
cycle: 28 seconds a cycle are not accounted for. Packer B counted 22 cycles in 60
minutes, 164 seconds a cycle, against the same 152 seconds of step times (timed on
packer A): 12 seconds. The totals use the step times. What fills the
remaining seconds in each cycle? For: supervisor.

MEASUREMENTS STILL MISSING: 9
M1. Shelf height. Step 1. Reaching. For: supervisor (measure).
M2. Reach distance to the carton stack. Step 1. Reaching. For: supervisor
(measure).
M3. Trolley height, where the box is lifted from. Step 2. Lifting. For: supervisor
(measure).
M4. Distance from the trolley to the bench. Step 2. Lifting, stated as "about two
steps". For: supervisor (measure).
M5. Reach distance to the paper dispenser. Step 3. Reaching. For: supervisor
(measure).
M6. Height of the paper dispenser. Step 3. Reaching. For: supervisor (measure).
M7. Distance from the bench to the conveyor. Step 4. Lifting, stated as "about
one pace". For: supervisor (measure).
M8. Extent of the turn at the waist. Step 4. Turning. For: assessor (observe).
M9. Cycles counted over a full shift. Task. The cycles per shift above are
estimated from one observed hour. For: supervisor (count).

Personal details left out: a worker's name, with a detail of a health complaint
and a visit to a doctor (worker feedback)

NOT ASSESSED: This record scores no posture, rates no risk, compares no load with
any limit, gives no view on any person's health or fitness, and certifies nothing.
The ergonomics assessor judges the task.

HANDOVER, completed by people, not by the assistant
Checked by supervisor: ____________  Date: ____________
Received by assessor: ____________  Date: ____________

Draft for the supervisor's check and the assessor's use. Nothing has been sent,
assigned, changed or recorded, and no work has been stopped or started.
```
## What was observed

Whether the required parts were produced. Yes. Every section of the output format appears, the "None." rule needed no use, every product was recomputed, and the personal detail was left out and its kind recorded. No stop condition applied. The count lines were checked against the lists they head: Steps 4, Measurements supplied 8, Measurements missing 9 (M1 to M9) and Disagreements 3 (D1 to D3), and the "WHERE THE INPUTS DISAGREE" heading reads 3.

Arithmetic, rechecked: 20 cycles / 1.0 hour x 6.0 hours = 120 and 22 / 1.0 x 6.0 = 132 cycles per shift. Packer A: 120 x 25 / 60 = 50.0, 120 x 3 / 60 = 6.0, 120 x 120 / 60 = 240.0 and 120 x 4 / 60 = 8.0 minutes, total 304.0. Packer B: 55.0, 6.6, 264.0 and 8.8 minutes, total 334.4. Weights: 120 x 4.2 = 504.0, 120 x 6.5 = 780.0, 132 x 4.2 = 554.4 and 132 x 6.5 = 858.0 kg. Counted rate: 3600 / 20 = 180 seconds against 152 for the step times, 28 seconds; 3600 / 22 = 163.6, rounded to 164, against 152, 12 seconds. These inputs observe for exactly one hour, so this run does not exercise the rate rule on a different length; acceptance test 13 covers that and has not been run.

The choices the earlier run found open are now settled in the template, and this run followed the settled rules: a loosely stated distance ("about two steps", "about one pace") is recorded as stated loosely and is still listed as missing; taking a flat carton off a shelf is reaching, not lifting, because the notes do not call it a lift; and the movement word in a missing-figure line is the notes' own, so M4 and M7 read "Lifting" (the notes say the box and the carton are lifted) and not "Carrying", a word the notes never use. A weight read from a label is shown as read from a label ("printed on the box label, not weighed"), and the total of the step times is the sum of the step times.

Against the reviewer checklist, the record met items 1, 2, 3, 5, 6, 7, 9 and 10. Items 4 and 8 depend on the assessor's judgement of the list of missing figures and of the disagreements, which the model cannot settle itself.

This was a further run by the same model that revised the template, on one invented example. It shows the template produces a complete, checkable record from these inputs; it does not show how it performs in a client's own setting or in other products, and it is not an independent run.
