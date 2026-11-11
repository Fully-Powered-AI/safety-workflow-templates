# Repeat incident pattern review: an invented example

*Illustrative example with invented data.* The business, the incidents, the dates, the people's roles and every figure below are invented. The business is an invented packaging and dispatch plant, called the Plant here, with a packing hall, a returns area, a goods-in dock and a dispatch dock. Its operations manager keeps the incident register and asked for a review of the year to 31 October 2026. The register has already been de-identified.

The inputs come first, in full, so the template can be run on them. The review follows.

## The inputs

### 1. Settings (typed by the operations manager)

```
Review period: 2025-11-01 to 2026-10-31
Today: 2026-11-02
Outcome order, lowest to highest: Near miss; First aid; Medical treatment; Lost time
Small-group limit: 3
Investigation lead: the operations manager
```

### 2. Incident register

```
incident_ref,date,outcome,area,task_or_equipment,cause_status,cause_category,confirmed_cause
INC-101,2025-10-20,Near miss,Packing,Pallet wrapper,Confirmed,Machine guarding,Wrapper gate interlock defeated; no check that it was working
INC-102,2025-11-18,Near miss,Dispatch,Forklift at dock,Confirmed,Pedestrian segregation,No marked walkway between dock door 2 and the packing bench
INC-103,2025-12-02,First aid,Packing,Packing bench,Confirmed,Housekeeping,No end-of-shift clean-down step for the packing bench
INC-104,2026-02-09,First aid,Packing,Pallet wrapper,Confirmed,Machine guarding,Wrapper gate interlock could be defeated during jams
INC-105,2026-02-24,Medical treatment,Dispatch,Forklift at dock,Confirmed,Maintenance,Brake wear not on the forklift service sheet
INC-106,2026-03-03,Near miss,Dispatch,Forklift at dock,Confirmed,Pedestrian segregation,Pedestrian door at the dock opens onto the forklift route with no warning
INC-107,2026-04-15,First aid,Returns,Returns area,Confirmed,Housekeeping,No end-of-shift clean-down step in the returns area
INC-108,2026-05-06,First aid,Dispatch,Forklift at dock,Confirmed,Training,Temporary driver started without the dock induction
INC-109,2026-05-27,Near miss,Packing,Pallet wrapper,Confirmed,Machine guarding,Wrapper gate interlock defeated during a jam
INC-110,2026-06-30,Near miss,Goods in,Dock plate,Confirmed,Housekeeping,Dock plate area not covered by any clean-down step
INC-111,2026-07-22,Medical treatment,Dispatch,Forklift at dock,Confirmed,Pedestrian segregation,No stop line or mirror where the dock exit meets the walkway
INC-112,2026-09-10,Near miss,Dispatch,Forklift at dock,Under investigation,,
INC-113,2026-10-05,First aid,Packing,Pallet wrapper,Not investigated,,
```

### 3. Action list

```
action_ref,incident_ref,action,owner_role,due_date,completed_date,check_result,check_date,status
A-31,INC-102,Paint a marked walkway from dock door 2 to the packing bench,Warehouse lead,2025-12-15,2025-12-12,,,Closed
A-38,INC-103,Add an end-of-shift clean-down step to the packing checklist,Packing supervisor,2026-02-06,2026-02-06,,,Closed
A-44,INC-104,Fit an interlock on the wrapper gate and test it weekly,Maintenance lead,2026-03-20,2026-03-20,Tested weekly for four weeks; no bypass found,2026-04-20,Closed
A-47,INC-105,Add brake wear to the forklift service sheet,Maintenance lead,2026-03-31,2026-03-27,,,Closed
A-49,INC-106,Fit a warning light on the pedestrian door at the dock,Warehouse lead,2026-04-10,2026-04-10,,,Closed
A-55,INC-108,Hold a dock induction for temporary drivers before their first shift,Operations manager,2026-06-05,2026-06-04,Induction record seen for all four temporary drivers,2026-06-10,Closed
A-61,INC-110,Clear and mark the dock plate area at the end of each shift,Goods-in lead,2026-07-31,,,,Open
A-66,INC-111,Fit a convex mirror and a stop line at the dock exit,Warehouse lead,2026-09-30,,,,Open
A-67,INC-111,Review the dock traffic plan with the team,Operations manager,2026-10-15,2026-10-14,,,Closed
```

## The review

```
REPEAT INCIDENT PATTERN REVIEW: 1 Nov 2025 to 31 Oct 2026

For: the operations manager. Prepared 2 Nov 2026 from the incident register and the action list supplied.

Inputs checked: 13 incidents supplied; 12 inside the period; 1 outside it (INC-101, 20 Oct 2025). Of those inside, 10 have a confirmed cause and 2 do not. 9 actions supplied; 9 linked to an incident inside the period. Small-group limit: 3. Outcome order: Near miss; First aid; Medical treatment; Lost time.
Confirmed cause categories as supplied: Pedestrian segregation 3; Housekeeping 3; Machine guarding 2; Maintenance 1; Training 1. Categories that look alike: none.

1. SAME CONFIRMED CAUSE AT THE SAME TASK OR EQUIPMENT

P1. Pedestrian segregation at Forklift at dock: 3 incidents, worst outcome Medical treatment, latest 22 Jul 2026 (103 days before today).
  Incidents: INC-102, 18 Nov 2025, Near miss, Dispatch; INC-106, 3 Mar 2026, Near miss, Dispatch; INC-111, 22 Jul 2026, Medical treatment, Dispatch. Days between: 105; 141.
  Confirmed causes as recorded: INC-102: No marked walkway between dock door 2 and the packing bench; INC-106: Pedestrian door at the dock opens onto the forklift route with no warning; INC-111: No stop line or mirror where the dock exit meets the walkway.
  Earlier actions: A-31, for INC-102, Paint a marked walkway from dock door 2 to the packing bench, Closed, completed 12 Dec 2025, no check result; A-49, for INC-106, Fit a warning light on the pedestrian door at the dock, Closed, completed 10 Apr 2026, no check result.
  Actions for the latest incident: A-66, for INC-111, Fit a convex mirror and a stop line at the dock exit, Open, not completed, no check result; A-67, for INC-111, Review the dock traffic plan with the team, Closed, completed 14 Oct 2026, no check result.
  After an earlier action: 2 (INC-106, INC-111). INC-106 is dated after A-31 was completed on 12 Dec 2025; INC-111 is dated after A-31 and after A-49 was completed on 10 Apr 2026; none also after a check date.
  Gaps: A-66 is open, 33 days past due. A-31, A-49 and A-67 were completed with no check result.

P2. Machine guarding at Pallet wrapper: 2 incidents, shown by month because the group is below the small-group limit. Months: INC-104, Feb 2026; INC-109, May 2026. Months between: 3. Worst outcome: First aid. Actions: 1 recorded, 1 completed, 1 with a check result. After an earlier action: 1 (INC-109, also after that action's check date). Gaps: INC-109 has no action recorded.

2. SAME CONFIRMED CAUSE AT DIFFERENT TASKS OR EQUIPMENT

C1. Housekeeping at 3 tasks or equipment: 3 incidents, worst outcome First aid, latest 30 Jun 2026 (125 days before today).
  Incidents: INC-103, 2 Dec 2025, First aid, Packing, Packing bench; INC-107, 15 Apr 2026, First aid, Returns, Returns area; INC-110, 30 Jun 2026, Near miss, Goods in, Dock plate. Days between: 134; 76.
  Confirmed causes as recorded: INC-103: No end-of-shift clean-down step for the packing bench; INC-107: No end-of-shift clean-down step in the returns area; INC-110: Dock plate area not covered by any clean-down step.
  Earlier actions: A-38, for INC-103, Add an end-of-shift clean-down step to the packing checklist, Closed, completed 6 Feb 2026, no check result.
  Actions for the latest incident: A-61, for INC-110, Clear and mark the dock plate area at the end of each shift, Open, not completed, no check result.
  After an earlier action: 2 (INC-107, INC-110), dated after A-38 was completed on 6 Feb 2026, written for a different task; this review does not compare what the action covered.
  Gaps: INC-107 has no action recorded. A-61 is open, 94 days past due. A-38 was completed with no check result.

3. SAME TASK OR EQUIPMENT, DIFFERENT CONFIRMED CAUSES

T1. Forklift at dock: 5 confirmed incidents under 3 cause categories, worst outcome Medical treatment, latest 22 Jul 2026 (103 days before today). Months between, in date order: 3; 1; 2; 2.
  Pedestrian segregation: 3 (INC-102, INC-106, INC-111); in section 1 group P1.
  Maintenance: 1 (INC-105); not in section 1. Feb 2026, Medical treatment. Action A-47, Closed, no check result.
  Training: 1 (INC-108); not in section 1. May 2026, First aid. Action A-55, Closed, check result recorded.
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

1. INC-106 and INC-111 are dated after A-31 was completed, and INC-111 after A-49 as well. Neither action has a check result. What was each meant to change at the dock, and what check was planned?
2. A-66 is 33 days past due and belongs to INC-111, the group's most serious outcome (Medical treatment). Who owns its date, and is anything in place at the dock exit in the meantime?
3. INC-109 is dated after A-44 was completed and after its check date, and has no action recorded. Does the confirmed cause for INC-109 describe the same condition as the one for INC-104? Cause wording is not shown for a group below the limit; it is in the register.
4. The confirmed causes for INC-103, INC-107 and INC-110 each name a missing clean-down step in a different place. A-38 is recorded as "Add an end-of-shift clean-down step to the packing checklist", INC-107 has no action, and A-61 is 94 days past due. Which actions cover the packing bench, the returns area and the dock plate, and who owns each?
5. The dock has had five confirmed incidents in about eight months under three cause categories, with actions held by the warehouse lead (A-31, A-49, A-66), the maintenance lead (A-47) and the operations manager (A-55, A-67). Who reviews the dock's actions together?
6. When are the causes of INC-112 and INC-113 expected to be confirmed, so the next review can place them? INC-112 is at the same task as five confirmed incidents and INC-113 at the same equipment as two.
7. INC-101, dated 20 Oct 2025, is 12 days before the period and has the same cause category and equipment as P2. Is it to be included in a review of P2?

This review compares records only. For the operations manager to decide which pattern, if any, needs a closer look. It investigates no single incident, finds no cause, assigns no blame, certifies nothing, and changes, sends and reports nothing.
```
