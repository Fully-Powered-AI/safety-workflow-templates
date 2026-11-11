# Temporary change register: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs for this run are the invented example in `public/example.md` (the settings, the change log and the item records, all invented). No client data was used. The run followed the instruction block in `member/template.md` and its output format. The model did not write the template. It read only the inputs of the example before producing the register, then compared its register with the example's.

## Inputs used

- Settings, change log (TC-101 to TC-110) and item records (TC-101 to TC-109, plus one row for TC-111) as given under "The inputs" in `public/example.md`.

## What came out

The register below is the run's output, set out in the template's format.

```
TEMPORARY CHANGE REGISTER: the Site, review as of 2026-12-07

For: the site manager. Prepared from the change log and item records supplied. Nothing here approves, extends or ends a change.

Counts: 7 open changes: 3 expired, 1 with no expiry date, 1 expiring within 30 days, 1 in date with items outstanding or not recorded, 1 in date with nothing outstanding. 2 ended changes: 1 with items still open, 1 with nothing open. Flags: approval not recorded 1; in place over 180 days 3; extended 2 or more times 1; no items recorded 0. Rows not read: 2.

1. Expired: 3

TC-103 Mould cooling time shortened from 20 to 15 minutes on Line 1. Process, Moulding hall. Owner production manager. Made 2026-06-01 (189 days ago). Approval: not recorded. Expired 2026-07-31 (129 days ago). Extended 0 times. Flags: approval not recorded; in place over 180 days.
Items: Compare part quality at 15-minute cooling (check): done 2026-06-26, evidence QA sheet 26 June. Update moulding procedure MP-07 (procedure): due 2026-06-15, 175 days overdue.
Decision: the site engineer chooses whether to restore, extend or reassess. Nothing is recorded as decided.

TC-101 Conveyor C3 run at reduced speed with a temporary clear guard panel fitted. Equipment, Packing hall. Owner maintenance supervisor. Made 2026-08-17 (112 days ago). Approval: site engineer on 2026-08-17. Expired 2026-10-31 (37 days ago). Extended 0 times. Flags: none.
Items: Fit permanent guard panel (check): due 2026-10-31, 37 days overdue. Update SOP-14 for reduced speed (procedure): done 2026-08-20, evidence signed SOP-14 rev C. Brief night shift on reduced speed (training): done 2026-08-24, evidence briefing roster 24 Aug.
Decision: the site engineer chooses whether to restore, extend or reassess. Nothing is recorded as decided.

TC-109 Compressor discharge pressure setpoint lowered. Process, Plant room. Owner maintenance supervisor. Made 2026-02-09 (301 days ago). Approval: site engineer on 2026-02-09. Expired 2026-12-04 (3 days ago). Extended 2 times. Flags: in place over 180 days; extended 2 or more times.
Items: Inspection of the pressure system by the competent person (check): done 2026-06-12, evidence report PS-26-3. Update compressed-air operating note (procedure): done 2026-03-02, evidence note rev 2.
Decision: the site engineer chooses whether to restore, extend or reassess. Nothing is recorded as decided.

2. No expiry date recorded: 1

TC-104 Chiller pump replaced with a different model. Equipment, Stores. Owner maintenance supervisor. Made 2026-03-23 (259 days ago). Approval: site engineer on 2026-03-23. No expiry date recorded. Extended 0 times. Flags: in place over 180 days.
Items: Update maintenance procedure and spare list (procedure): due 2026-04-30, 221 days overdue. Train maintenance team on the new pump (training): done 2026-05-06, evidence sign-in sheet 6 May.
Decision: the site engineer chooses whether to restore, extend or reassess. Nothing is recorded as decided.

3. Expiring within 30 days: 1

TC-102 Two pallet-stacking bays moved into the east walkway, leaving a marked route. Layout, East aisle. Owner warehouse supervisor. Made 2026-11-02 (35 days ago). Approval: site engineer on 2026-11-02. Expires 2026-12-14 (in 7 days). Extended 0 times. Flags: none.
Items: Measure clear walkway width (check): due 2026-12-04, 3 days overdue. Update fire-route plan (procedure): done 2026-12-02, evidence not supplied. Brief supervisors on the new route (training): due 2026-12-11, in 4 days.
Decision: the site engineer chooses whether to restore, extend or reassess. Nothing is recorded as decided.

4. In date, items outstanding or not recorded: 1

TC-106 Temporary cabin placed in the yard for visiting inspectors. Layout, Yard. Owner facilities coordinator. Made 2026-10-19 (49 days ago). Approval: site engineer on 2026-10-19. Expires 2027-01-31 (in 55 days). Extended 0 times. Flags: none.
Items: Test fire alarm link to the cabin (check): due 2026-12-20, in 13 days. Add cabin to the evacuation plan (procedure): done 2026-11-02, evidence plan rev 7.

5. In date, nothing outstanding: 1

TC-105 Additives weighed by hand while the dosing unit is repaired. Expires 2027-01-15. 2 of 2 items done with evidence.

6. Ended, items still open: 1

TC-107 Forklift charger moved to the loading bay. Ended. Owner warehouse supervisor.
Items: Confirm original charging bay floor marking restored (check): due 2026-12-04, 3 days overdue. Brief forklift drivers on return to the original bay (training): done 2026-12-03, evidence roster 3 Dec.

7. Ended, nothing open: 1

TC-108 Packing line 2 layout moved for a trial run. 1 of 1 items done with evidence.

8. Rows not read: 2

Change log, TC-110: expiry_date "after the audit" is not a date.
Item records, TC-111: no matching change in the change log.

Questions: 5
1. TC-103: approval not recorded (approved_by and approval_date are blank). The production manager, who owns the change, can answer.
2. TC-104: expiry date not recorded. The maintenance supervisor, who owns the change, can answer.
3. TC-102: "Update fire-route plan" is shown as done on 2026-12-02 with no evidence reference. The warehouse supervisor, who owns the change, can answer.
4. TC-110: row not read because the expiry date "after the audit" is not a date. The warehouse supervisor, who owns the change, can answer.
5. TC-111: the item "Re-test relief valve" matches no change in the log. The settings name nobody for the item records, so the site manager, who runs the register, can answer.

Every date and count traces to the change log and item records supplied, with the review date as the reference. The register changes no records and sends nothing.
```

## What was observed

- **Every required part was produced.** Header, counts line, sections 1 to 8, questions and the trace line all came out. The counts line agrees with the sections (7 open and 2 ended changes; flags 1, 3, 1 and 0; 2 rows not read). Nothing in the run called for a stop: both files and the review date were supplied, the headers matched, no change_id was duplicated, and nothing in the inputs said a change was unsafe now.
- **Ordering and placement.** TC-103, TC-101 and TC-109 are in section 1 by expiry date, earliest first. TC-107 expired on 2026-12-03 but is ended, so it is not called expired and goes to section 6 because of its open check. TC-110 (expiry "after the audit") was not placed in a section.
- **Against the published example.** The example was later aligned to this run, so the two now read almost the same; see "Changed after the run recorded above" below for what was aligned and the few strings that still differ. As the run stood, the facts, dates, day counts, sections, flags, counts and decision lines match the example's register. The differences are small:
  - The example writes the area in lower case ("moulding hall", "east aisle"); this run kept the log's spelling ("Moulding hall", "East aisle"). The template does not say which.
  - The example's note on the TC-111 row adds the item name and due date in brackets; this run left them for the question.
  - The wording of the questions differs, and so does who can answer. The example names the production manager or the site engineer for question 1, the site engineer for questions 2 and 4, and "the person who keeps the item records" for question 5. This run named the owner of each change for questions 1 to 4, and the site manager for question 5.
- **Facts in the example's output that are not in the inputs.** "Whoever entered the row" (question 4) and "the person who keeps the item records" (question 5) name roles the inputs never give. The example's question 1 also names the site engineer as someone who can say who approved the change, which the inputs do not show. In this run's output, question 5 names the site manager, the person the settings say the register is prepared for, because no one is named for the item records. Every other fact in this run's output traces to the inputs. The one added phrase is "who owns the change", which the template supports.
- **Ambiguities and shortcomings in the template**, met while following it:
  1. The settings in the example do not name anyone as keeper of the change log, although the Roles section says the settings do. So the role to answer a question about an item with no matching change is not defined. The template also gives no rule for choosing who answers when a question concerns a row that was not read.
  2. The instruction block is shorter than the procedure and leaves out rules the procedure has. It does not say that sections 2, 6 and 7 are ordered differently from the others. It does not say to stop on duplicate change_ids. It does not give the order of the questions. It does not say how to flag a done date later than the review date, or an item row whose change was not read. A run from the block alone would have to guess these.
  3. The template does not say whether the counts line includes open changes that were not read. This run counted only changes it could place in a section (7 open), as the example does, but the template never says so.
  4. The type is written "equipment, layout or process" and the log has "Equipment", "Layout", "Process". This run matched them ignoring case. The template does not say that case is ignored, and "never guess" could be read the other way.
  5. How to recognise a change that is "unsafe now" is not defined. This run took it to mean only what the person says, so TC-101 (a permanent guard still not fitted 37 days past expiry) was not treated as a stop. A different reading might stop here.
  6. The format says "Approval: [role on date, or 'not recorded']", but does not say what to print when `approved_by` is filled and `approval_date` is blank, or the reverse.
  7. The format has the area after the type with no case rule (see above), and does not say what to print in the header for the site when the setting is a list ("the Site, moulding hall, packing hall, warehouse and yard"). This run printed "the Site", as the example does.
- **Not tested here.** The acceptance tests were not run; only the one example was. Nothing in this trial shows how the template behaves on a real site's files or in any other AI product.

## Changed after the run recorded above, and not run again

The output and the observations above are as recorded and describe the template and the example as they stood at the run. After an independent review of the template, on 10 November 2026:

- **Corrections to the observations.** The observation about the instruction block says it does not say how to flag a done date later than the review date. That was inaccurate: step 1 of the block covers it by listing the row under "Rows not read". The gap was in the other rules named beside it.
- **Roles and answerers.** The template no longer says the settings name a keeper of the change log. It now has a rule for who answers a question: the change's owner; for a row not read with a blank owner, an item with no matching change, or no decider named, the role the register is prepared for. The example's questions 1, 2, 4 and 5 now name those roles, as this run did.
- **Case and spelling.** The template now ignores case in type and status, prints the type with a capital first letter, and prints the area as the log gives it. The example now keeps the log's spelling of the area, as the run did.
- **Rows not read.** The example no longer adds the item name and due date in brackets to the TC-111 line, as the run did.
- **Counts, header, approval and unsafe now.** The template now says that a change whose row was not read is not counted as open or ended, that a list in the site setting prints its first entry, how to print approval when only one of the approver and the date is filled, and that "unsafe now" means the person says so or a file states it. The run did what these rules now say, except that the approval case with one field filled did not arise in the example.
- **The instruction block** now carries the rules that were only in the procedure: stop on a duplicate change_id, extended is treated as open, a blank extension count is 0, a blank approver means not recorded, the order within each section, the order of the questions, an item row whose change was not read, and referring to people by role.

- **Small wording changes after the review, also not run again.** Question 5 in the example now says the site manager is the person "for whom the register is prepared", which is how the settings put it, in place of "who runs the register". In the example inputs, TC-104 is now in the "Plant room" instead of "Stores", and the TC-111 item is "Re-test emergency stop" instead of "Re-test relief valve". The register above is left as the run produced it, so it still shows "Stores", the relief-valve item and "who runs the register"; apart from those three strings the example's register and this one are the same.
- **Template rules added, not run.** An expiry on the review date is now written "expires today"; the instruction block now says what to do when the item records are missing, that the expiring-soon window includes the review date and its last day, that the in-place and extended flags apply to open changes only, and that days overdue is the review date minus the due date; and a status of extended with a count of 0 or blank is printed as the log gives it. None of these cases arose in this run.

None of these was run again. A block-only run has not been tried.
