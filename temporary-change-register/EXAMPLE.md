# Temporary change register: an invented example

*Illustrative example with invented data.* The site, the changes, the dates and the evidence references below are all invented. The site is an invented 90-person plastics moulding and packing site, called the Site here. The site manager runs the review; the site engineer is its competent person and decides each change. People are referred to by role.

The inputs come first, in full, so the template can be run on them. The register follows.

## The inputs

### 1. Settings (typed by the site manager)

```
Site: the Site, moulding hall, packing hall, warehouse and yard
Review date: Monday 2026-12-07
Prepared for: the site manager
Decides each change: the site engineer
Expiring soon means: expiry within 30 days of the review date
In place too long: more than 180 days
Extended too often: 2 or more extensions
```

### 2. Change log (export)

```
change_id,description,type,area,date_made,owner,approved_by,approval_date,expiry_date,extension_count,status
TC-101,"Conveyor C3 run at reduced speed with a temporary clear guard panel fitted",Equipment,Packing hall,2026-08-17,maintenance supervisor,site engineer,2026-08-17,2026-10-31,0,open
TC-102,"Two pallet-stacking bays moved into the east walkway, leaving a marked route",Layout,East aisle,2026-11-02,warehouse supervisor,site engineer,2026-11-02,2026-12-14,0,open
TC-103,"Mould cooling time shortened from 20 to 15 minutes on Line 1",Process,Moulding hall,2026-06-01,production manager,,,2026-07-31,0,open
TC-104,"Chiller pump replaced with a different model",Equipment,Plant room,2026-03-23,maintenance supervisor,site engineer,2026-03-23,,0,open
TC-105,"Additives weighed by hand while the dosing unit is repaired",Process,Moulding hall,2026-11-23,production manager,site engineer,2026-11-23,2027-01-15,0,open
TC-106,"Temporary cabin placed in the yard for visiting inspectors",Layout,Yard,2026-10-19,facilities coordinator,site engineer,2026-10-19,2027-01-31,0,open
TC-107,"Forklift charger moved to the loading bay",Equipment,Warehouse,2026-10-05,warehouse supervisor,site engineer,2026-10-05,2026-12-03,0,ended
TC-108,"Packing line 2 layout moved for a trial run",Layout,Packing hall,2026-09-14,production manager,site engineer,2026-09-14,2026-11-15,0,ended
TC-109,"Compressor discharge pressure setpoint lowered",Process,Plant room,2026-02-09,maintenance supervisor,site engineer,2026-02-09,2026-12-04,2,open
TC-110,"Loading dock door 4 closed and traffic redirected to door 5",Layout,Dock,2026-11-16,warehouse supervisor,site engineer,2026-11-16,after the audit,0,open
```

### 3. Item records (export)

```
change_id,item,kind,due_date,done_date,evidence
TC-101,Fit permanent guard panel,check,2026-10-31,,
TC-101,Update SOP-14 for reduced speed,procedure,2026-08-24,2026-08-20,signed SOP-14 rev C
TC-101,Brief night shift on reduced speed,training,2026-08-31,2026-08-24,briefing roster 24 Aug
TC-102,Measure clear walkway width,check,2026-12-04,,
TC-102,Update fire-route plan,procedure,2026-12-11,2026-12-02,
TC-102,Brief supervisors on the new route,training,2026-12-11,,
TC-103,Compare part quality at 15-minute cooling,check,2026-06-30,2026-06-26,QA sheet 26 June
TC-103,Update moulding procedure MP-07,procedure,2026-06-15,,
TC-104,Update maintenance procedure and spare list,procedure,2026-04-30,,
TC-104,Train maintenance team on the new pump,training,2026-04-30,2026-05-06,sign-in sheet 6 May
TC-105,Check dust extraction at the weighing station,check,2026-11-27,2026-11-24,check sheet 24 Nov
TC-105,Brief operators on manual weighing steps,training,2026-11-27,2026-11-24,roster 24 Nov
TC-106,Test fire alarm link to the cabin,check,2026-12-20,,
TC-106,Add cabin to the evacuation plan,procedure,2026-11-02,2026-11-02,plan rev 7
TC-107,Confirm original charging bay floor marking restored,check,2026-12-04,,
TC-107,Brief forklift drivers on return to the original bay,training,2026-12-04,2026-12-03,roster 3 Dec
TC-108,Confirm original line layout restored,check,2026-11-15,2026-11-14,photo 14 Nov
TC-109,Inspection of the pressure system by the competent person,check,2026-06-30,2026-06-12,report PS-26-3
TC-109,Update compressed-air operating note,procedure,2026-03-01,2026-03-02,note rev 2
TC-111,Re-test emergency stop,check,2026-12-01,,
```

## The register

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

TC-104 Chiller pump replaced with a different model. Equipment, Plant room. Owner maintenance supervisor. Made 2026-03-23 (259 days ago). Approval: site engineer on 2026-03-23. No expiry date recorded. Extended 0 times. Flags: in place over 180 days.
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
5. TC-111: the item "Re-test emergency stop" matches no change in the log. The settings name nobody for the item records, so the site manager, for whom the register is prepared, can answer.

Every date and count traces to the change log and item records supplied, with the review date as the reference. The register changes no records and sends nothing.
