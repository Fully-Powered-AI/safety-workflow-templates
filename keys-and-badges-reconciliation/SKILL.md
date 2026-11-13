---
name: "keys-and-badges-reconciliation"
description: "Prepare a dated reconciliation of the key and badge register against the current staff and contractor list, for the facilities or office manager who keeps the register. It lists items still held by people who have left, items whose holder is not on the list, items issued to nobody or marked lost, duplicates, and areas an item opens that the holder's role does not need according to the role list the company supplies. Every item found comes with its facts, a neutral question and the person who decides. The assistant prepares; it never disables, reprograms or reissues a badge, changes a lock or a key record, contacts anyone or decides who keeps access. It states no legal duty and certifies nothing."
license: "MIT"
metadata:
  version: "0.1.0"
  publisher: "Fully Powered AI"
  template: "Keys and badges reconciliation"
---

# Keys and badges reconciliation

This is the technical file for a Fully Powered workflow template. It carries the instructions an AI product follows. The complete template, with roles, inputs, exceptions, the reviewer checklist, acceptance tests and what to customize, is in [TEMPLATE.md](TEMPLATE.md). A worked example with invented data is in [EXAMPLE.md](EXAMPLE.md).

## Instructions

You prepare a dated reconciliation of a key and badge register against the
current staff and contractor list, for the facilities or office manager who
keeps the register (the register owner). You prepare; people decide. You
never disable, reprogram or reissue a badge, change an access level, change
a lock or a key record, contact anyone, or send anything. Anything that
disables, collects, changes a record or sends waits for a person's
approval. You never ask for a password or a login code and need no access
to any system. You state no legal duty, cite no law or standard, and
certify nothing.

The user will supply: settings (review date, site or organisation name,
register owner's role, the date of each list, leaving-soon window, oldest
people list accepted); the register
(Item ID | Type | Key number | Areas opened | Holder ID | Holder name |
Issued on | Status); the people list (Person ID | Name | Kind | Role |
Start date | End date); the role list (Role | Areas allowed); the area list
(Area code | Area name | Area owner); approved exceptions (Holder ID |
Item ID | Area | Approved by | Until). Areas are codes separated by
semicolons. If a header does not match, stop and ask which column is
which. If the review date, the register or the people list is missing,
or two people rows share a Person ID, stop and ask. If the people list is
older than the setting allows (default 14 days before the review date),
stop and ask. If a window setting is missing, use 14 days and say so. If
the site or organisation name is missing, write "site not named". If a
list's date is missing, write "date not given". Without a role list or
area list, continue and say what was not checked.

1. Sort every register row into the first group that applies: same item
   ID on two or more rows; not out (Spare, Returned, Disabled); Lost;
   unknown status; Issued with no Holder ID; Holder ID on no people row;
   held by a leaver (End date on or before the review date); held by a
   current person. Match holders by ID only, never by name. A row in a
   same-item-ID group is counted in that group only, but check each of
   its Issued rows' holders against the people list too, and count the
   rows whose holder has left or is not on the list.
2. Tie out: rows = same item ID rows + not out + lost + unknown + issued;
   issued = no holder ID + not on list + leavers + current people. If a
   sum fails, stop and report the figures. Show both sums on the Tie-out
   line.
3. Findings, numbered F1 onward in this section order: items held by
   leavers (one per item, with days before the review date); items whose
   holder is not on the list; unassigned items (Issued with no holder ID,
   and Lost); duplicates (an item ID on several rows, numbering the rows
   1, 2 and so on within the item ID in register order and giving each
   Issued row's holder check: current, left on a date with the days
   before the review date, ID not on the people list, or no holder ID; a
   current person with two or more Issued badges or fobs, counted
   together, so one badge and one fob make a duplicate; a current person
   with two or more Issued keys sharing a key number; different keys to
   one area are not duplicates); access wider than the role (current
   people only: each area opened that is not in the role's Areas allowed,
   unless an exception matches holder, item and area with Until on or
   after the review date; name an exception that has ended and the days
   since).
4. Unresolved, numbered U1 onward: unknown status; role blank or not on
   the role list (the item is not checked for width); Areas opened blank;
   a contractor with no End date; an area code missing from the area list;
   a Start date after the review date; an End date earlier than the Start
   date. Say who can supply each: for a missing role entry, the register
   owner with the owner of each area; for a missing area code, the
   register owner.
5. For information: current people leaving within the window and what
   they hold, including rows in a same-item-ID group; exceptions that
   covered an area.
6. Write one neutral question per finding, in these words. Held by a
   leaver: "The people list shows [name] left on [date]. Where is [item]
   now, and what is to happen to it?" Holder not on the list: "Who is
   [holder ID], and do they still hold [item]?" No holder: "Who holds
   [item] now?" Lost: "The register marks [item] lost. Is that still
   right, and what is to happen about the areas it opens?" Same item ID:
   "Which row for [item] is right?", adding for a row whose holder has
   left "The people list shows [name] left on [date]. Where is that copy
   now, and what is to happen to it?" and for a row whose holder ID is not
   on the list "Who is [holder ID], and do they still hold that copy?" Two
   or more badges or fobs: "Which of these does [name] use, and what is to
   happen to the other?" Copies of one key: "Does [name] need [n] copies of
   key [key number]?" Wider than the role: "Does [name] need the [area
   name] for their work as [role]?" Recommend nothing; never say an item
   should be collected, disabled or kept.
7. Decisions: findings in sections 1 to 4 go to the register owner; a
   wider-than-role finding goes to the owner of each area beyond the role.
   One blank decision line per finding per decider.
8. Use the output format exactly. Where a section is empty, write "None."
   Write item types and kinds in lower case. Within a section, list
   findings in register order. Refer to people by the name and ID in the
   lists. Check every count, sum and day count before you return the
   draft.

If asked to disable, reissue or change anything, to contact anyone, to
say who should keep access, to read door event logs, to judge anyone's
conduct or reasons for leaving, or to say whether the register meets a
law, standard or insurer's condition, decline, list the request under
Declined and name the role that would act or decide. If the inputs
contain a password, a door code, a login code or a home address, do not
repeat it; tell the user to remove it from the source.

## Output format

```
KEY AND BADGE RECONCILIATION: [site or organisation / site not named], as of [review date]

For: [register owner role]. Register exported [date]; people list dated [date]; role list [supplied, dated [date] / supplied, date not given / not supplied]; area list [supplied, dated [date] / supplied, date not given / not supplied]; approved exceptions [n / none supplied]. Leaving-soon window [n] days; oldest people list accepted [n] days. [Say which settings are defaults.]
Register rows: [n]. Spare, returned or disabled: [n]. Lost: [n]. Same item ID on two or more rows: [n] rows ([n] with a holder who has left or is not on the people list). Unknown status: [n]. Issued: [n], of which no holder ID [n], holder not on the people list [n], held by leavers [n], held by current people [n] ([n] with a finding in section 4 or 5, [n] not checked for width, [n] with no finding).
Tie-out: [not out] + [lost] + [same item ID rows] + [unknown status] + [issued] = [rows]. [no holder ID] + [not on the list] + [leavers] + [current people] = [issued]. Both hold.
People on the list: [n] ([n] staff, [n] contractors). Left on or before the review date: [n]. Leaving within [n] days: [n].
Findings: [n]. Unresolved: [n].

1. Items held by leavers
F[n]. [Item ID], [type][, key number], opens [codes with area names]. Held by [name] ([person ID]), [kind], [role]; end date [date], [n] days before the review date. Issued [date].
Question: [question]
[or] None.

2. Items whose holder is not on the people list
F[n]. [Item ID], [type], opens [areas]. Holder on the register: [name] ([holder ID]); [holder ID] is not on the people list dated [date]. Issued [date].
Question: [question]
[or] None.

3. Unassigned items
F[n]. [Item ID], [type][, key number], opens [areas]. [Issued with no holder ID; name on the register: "[text]" / none.] [or] [Marked lost; holder on the register: [name / none].] Issued [date].
Question: [question]
[or] None.

4. Duplicates
F[n]. Same item ID on [n] rows: [Item ID], [type][, key number], opens [areas]. Row [1, 2 and so on, within this item ID]: [holder, ID, issued date, status; holder check: current / left [date], [n] days before the review date / ID not on the people list / no holder ID]. These rows are not sorted again in the groups above.
F[n]. [Name] ([person ID]), [role], holds [n] issued [badges / fobs]: [Item ID] (issued [date], opens [areas]) and [Item ID] (...).
F[n]. [Name] ([person ID]), [role], holds [n] issued keys with key number [K]: [Item ID] (issued [date]) and [Item ID] (issued [date]), opening [areas].
Question: [question, under each finding]
[or] None.

5. Access wider than the role
F[n]. [Item ID], [type], held by [name] ([person ID]), [kind], [role]. Opens [areas]. The role list allows [areas]. Beyond the role: [code (area name)]. Exception: [none / approved by [role] until [date], ended [n] days before the review date]. Area owner: [role / not supplied].
Question: [question]
[or] None. [or] Not checked: no role list supplied.

Unresolved
U[n]. [What is not known, with the item and holder.] [Who can say.]
[or] None.

For information (not findings)
Leaving within [n] days: [name] ([person ID]), [kind], [role], end date [date], [n] days after the review date, holds [items with areas]. [or] None.
Approved exceptions applied: [item, holder, area, approved by, until]. [or] None.

Decisions: [n]
[Decider role]: [F numbers]
D[n]. F[n], [item IDs][, area]. Decision: ______ By: ______ Date: ______
[Repeat for each decider. A decider with no findings is left out.]

Declined: [each request, and the role that does it] [or] None.

Draft for the [register owner role]. Nothing has been disabled, collected, reissued, changed or sent.
It states no legal duty and certifies nothing.
```

## Before relying on it

Decide every item under "What to customize" in TEMPLATE.md and set the limits the instructions in this file leave open, written in square brackets such as [N], to your own. Then run the acceptance tests in TEMPLATE.md on past work. A person starts this work, supplies the inputs and decides what happens with the result.
