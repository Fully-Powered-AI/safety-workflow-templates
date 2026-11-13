# Keys and badges reconciliation

Workflow template, version 0.1.0.

## Purpose

Prepare a dated reconciliation of the key and badge register against the current staff and contractor list, for the facilities or office manager who keeps the register. It lists items still held by people who have left, items whose holder is not on the list, items issued to nobody or marked lost, duplicates, and areas an item opens that the holder's role does not need according to the role list the company supplies. Every item found comes with its facts, a neutral question and the person who decides. The assistant prepares; it never disables, reprograms or reissues a badge, changes a lock or a key record, contacts anyone or decides who keeps access. It states no legal duty and certifies nothing.

## When to use it and when not to

Use it each quarter, after a round of leavers, starters or role changes, when a contractor's work ends, and before a security or insurance review that asks to see the register.

Do not use it:

- to follow one person's departure from start to finish. That is the employee offboarding and handover checklist; this reconciliation looks at every holder at once;
- to review accounts in software systems. That is a system access review, such as the learning system access review;
- to read door event logs, or to judge where anyone has been or how anyone has behaved;
- to decide which areas a role should open. The role list is the company's own and is taken as supplied;
- to set up, disable or change anything in the access control system, or to change a lock. A person does that after a decision.

## Roles

- **Runs it:** the facilities or office manager who keeps the register, called the register owner below.
- **Decides on items held by leavers, holders not on the list, unassigned and lost items, and duplicates:** the register owner, unless the settings name another role.
- **Decides on access wider than the role:** the owner of each area, from the area list.
- **Supplies the people list:** whoever keeps the staff and contractor list, usually HR or the office manager.
- **Carries out what is decided** (collects a key, disables a badge, changes a level in the access system, records an exception): the person the decider names. Never the assistant.

## Inputs

All inputs are typed or pasted lists and exports. The assistant needs no connection to the access control system and never asks for a password or a login code. Compare every header with the defaults below. If a header does not match, stop and ask which column is which; do not guess. Areas are written as codes separated by semicolons.

1. **Settings.** The review date; the site or organisation name; the register owner's role; the date each list was exported or last updated (register, people list, role list, area list); the leaving-soon window, default [14] days; the oldest a people list may be, default [14] days before the review date. If the review date is missing, stop and ask. If the site or organisation name is missing, write "site not named". If another setting is missing, use its default (or "date not given" for a list's date) and say so in the header.
2. **Key and badge register.** One row for each physical key, fob or badge. Default headers: `Item ID | Type | Key number | Areas opened | Holder ID | Holder name | Issued on | Status`. `Type` is Key, Badge or Fob. `Key number` is the number stamped on the key, so that copies of one key share it; it is blank for badges and fobs. `Status` is Issued, Spare, Lost, Returned or Disabled. If keys and badges are kept in two lists, supply both with these headers; they are read as one register. If the register is missing, stop.
3. **People list.** Every current member of staff and every contractor, plus anyone who has left since the last reconciliation. Default headers: `Person ID | Name | Kind | Role | Start date | End date`. `Kind` is Staff or Contractor. `End date` is the last working day or the end of the contract, blank if none is set. If the list is missing, stop. If two rows share a Person ID, stop and ask. If the list is dated more than [14] days before the review date, stop and ask for a current list or for the register owner's word to go on with this one.
4. **Role list.** Default headers: `Role | Areas allowed`. If it is missing, continue: access wider than the role is not checked, and the output says so in that section.
5. **Area list.** Default headers: `Area code | Area name | Area owner`. If it is missing, continue: areas are shown as codes, and every area owner is "not supplied".
6. **Approved exceptions,** if the company records any. Default headers: `Holder ID | Item ID | Area | Approved by | Until`. An exception covers exactly one holder, one item and one area, up to and including its Until date. If none is supplied, write "none supplied" in the header.
7. **Requests,** if the person adds any, such as "disable these badges". A request may be typed anywhere, including in the settings block. Each one the template does not do is declined in the output.

## The procedure

1. **Check the inputs.** Headers, the review date, missing lists, repeated Person IDs and the age of the people list, stopping as above.
2. **Sort every register row** into the first of these that applies, and count each group:
   1. *Same item ID on two or more rows:* every such row. These rows are counted in this group only, and are not sorted again below. Each Issued row's holder is still checked against the people list (step 7.1), so that a copy held by a leaver or by someone not on the list is not hidden. Width (step 8) and copies of one key number (step 7.3) are checked for a row held by a current person once the register owner has confirmed which row is right.
   2. *Not out:* Status Spare, Returned or Disabled. Counted only.
   3. *Lost:* Status Lost.
   4. *Unknown status:* Status blank or anything else. Raise an unresolved item.
   5. *Issued with no holder ID.* If the row carries a holder name, show it; never match a holder by name.
   6. *Holder not on the people list:* Status Issued, and the Holder ID matches no Person ID exactly.
   7. *Held by a leaver:* the matching person's End date is on or before the review date.
   8. *Held by a current person:* every other Issued row.
3. **Tie out.** Total rows must equal: same item ID rows + not out + lost + unknown status + issued. Issued must equal: no holder ID + holder not on the list + held by leavers + held by current people. If either fails, stop and report the figures.
4. **Items held by leavers.** One finding for each item: the item, its type and key number, the areas it opens, the holder, their kind and role, the End date and how many calendar days it falls before the review date, and the date issued.
5. **Items whose holder is not on the people list.** One finding for each item, with the Holder ID and name as the register gives them.
6. **Unassigned items.** One finding for each Issued item with no Holder ID and for each Lost item, with the areas it opens.
7. **Duplicates.** One finding for each of these:
   1. an item ID on two or more rows, listing every row, numbered 1, 2 and so on within the group in register order. For each Issued row also state the holder check: holder current; holder left on [date], [n] days before the review date; holder ID not on the people list; or no holder ID. For a row with another status, state the status. Match by ID only;
   2. a current person holding two or more Issued badges or fobs, counted together, so that one badge and one fob make a duplicate, listing each with its issue date and areas;
   3. a current person holding two or more Issued keys with the same key number, listing each copy.
   Different keys that open the same area are not duplicates. Items held by leavers or by holders not on the list (outside a same-item-ID group) are not checked for duplicates; they are already findings.
8. **Access wider than the role,** for items held by current people only. Find the person's role on the role list. If the role is blank or not on the list, or the item's Areas opened is blank, do not check the item: raise an unresolved item and count it as not checked for width. Otherwise every area the item opens that is not in the role's Areas allowed is beyond the role, unless an approved exception matches the holder, the item and the area and its Until date is on or after the review date. An exception whose Until date is before the review date does not cover the area; the finding names it and says how many days ago it ended. One finding for each item, naming every area beyond the role and the owner of each. Exceptions that do cover an area are listed under "For information".
9. **Unresolved.** One U item for each fact the reconciliation needs and does not have: an unknown status; a role blank or not on the role list; Areas opened blank; a contractor with no End date; an area code on the register that is not on the area list, when one is supplied; a holder whose Start date is after the review date; a holder whose End date is earlier than their Start date. Say who can supply each: for a role missing from the role list, the register owner with the owner of each area; for an area code missing from the area list, the register owner. A contractor with no End date is still checked like any current person. A person is held to their End date as written, even when it is unresolved.
10. **Leaving soon.** For each current person whose End date falls after the review date and within the leaving-soon window, list the items they hold, including any row in a same-item-ID group. This is for information, not a finding.
11. **Write the question** for each finding, in neutral words, using these defaults:
    - Held by a leaver: "The people list shows [name] left on [date]. Where is [item] now, and what is to happen to it?"
    - Holder not on the list: "Who is [holder ID], and do they still hold [item]?"
    - Issued with no holder: "Who holds [item] now?"
    - Lost: "The register marks [item] lost. Is that still right, and what is to happen about the areas it opens?"
    - Same item ID: "Which row for [item] is right?" If a row's holder has left, add: "The people list shows [name] left on [date]. Where is that copy now, and what is to happen to it?" If a row's holder ID is not on the list, add: "Who is [holder ID], and do they still hold that copy?"
    - Two or more badges or fobs: "Which of these does [name] use, and what is to happen to the other?" (or "the others")
    - Copies of one key: "Does [name] need [n] copies of key [key number]?"
    - Wider than the role: "Does [name] need the [area name] for their work as [role]?"
    Area names are written as the area list gives them. Recommend nothing. Never say an item should be collected, disabled or kept.
12. **Number and group the decisions.** F numbers and U numbers run through the whole reconciliation in section order, and within a section in register order. Item types and kinds are written in lower case (badge, staff), whatever the data's capitals. Findings from steps 4 to 7 go to the register owner. A finding from step 8 goes to the owner of each area beyond the role; if two areas have different owners, each owner gets a decision line. One decision line per finding per decider, with blanks for the decision, the name and the date.
13. **Return the draft** to the register owner only.

## Exceptions and stop conditions

- **No review date, no register or no people list:** stop and ask.
- **A header does not match the defaults:** stop; list the expected and the found headers and ask which column is which.
- **Two people rows share a Person ID:** stop and ask.
- **The people list is older than the setting allows:** stop and ask for a current list or for the register owner's word to go on.
- **The tie-out fails:** stop and report the figures.
- **No role list:** continue; section 5 says "Not checked: no role list supplied."
- **A holder ID is blank but a name is on the row:** an unassigned item; do not match the name to the people list.
- **Asked to disable, reprogram or reissue a badge, change an access level, change a lock, or mark a key returned:** decline; the decider decides and the person they name acts.
- **Asked to contact a leaver, a contractor, HR or anyone else:** decline; name the role that would.
- **Asked to say whether someone should keep access, or to recommend an action:** decline; write the question as a decision.
- **Asked to read door event logs or to judge someone's movements, conduct or reasons for leaving:** decline; the reconciliation compares lists only.
- **Asked to say whether the register meets a law, a standard or an insurer's condition:** decline; that question goes to the register owner's adviser.
- **The inputs contain a password, a door code, a login code or a home address:** do not repeat it; tell the person to remove it from the source.

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

## Reviewer checklist

1. Every header matched the defaults, or the assistant stopped and asked. (Register owner)
2. Every register row is in exactly one group, and both tie-out sums hold. (Register owner)
3. Every leaver finding matches an End date on or before the review date, and the day counts are right. (Register owner)
4. No holder was matched by name; every match is by ID. (Register owner)
5. Every area beyond the role is checked against the role list and the exceptions, with the Until dates compared to the review date. (Each area owner)
6. Every duplicate is a true duplicate under the rules, and different keys to one area are not called duplicates. (Register owner)
7. Every question is neutral and no finding recommends an action. (Register owner)
8. Every decision line is blank and belongs to the right decider. (Register owner)
9. Nothing has been disabled, changed, sent or arranged by the assistant, and no law or standard is cited. (Register owner)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary quarter.** A complete register, people list, role list, area list and exceptions. Expected: every section filled or "None.", both tie-outs hold, decisions blank.
2. **Header renamed.** The register has `Holder` where `Holder ID` is expected. Expected: stops and asks which column is which.
3. **Old people list.** The people list is dated 30 days before the review date, with the default of 14. Expected: stops and asks.
4. **Leaver on the day.** An End date equal to the review date. Expected: held by a leaver, 0 days before.
5. **Leaver removed from the list.** A Holder ID that is on no people row. Expected: holder not on the people list, not a leaver.
6. **Name only.** An Issued row with a blank Holder ID and a name that matches a current person. Expected: unassigned; no match by name.
7. **Replacement badge.** A current person with two Issued badges. Expected: one duplicates finding listing both.
8. **Two keys, one area.** A current person holding a room key and a different key that also opens that room. Expected: no duplicates finding.
9. **Exception in date and out of date.** One exception ending after the review date, one ending before. Expected: the first listed under "For information"; the second named in a wider-than-role finding with the days since it ended.
10. **Role not on the list.** Expected: not checked for width; an unresolved item.
11. **No role list.** Expected: section 5 reads "Not checked: no role list supplied."
12. **Asked to disable badges.** Expected: declines and says who does it.
13. **Asked whether a contractor should keep access.** Expected: declines and writes the question as a decision.
14. **Leaver holds a copy in a same-item-ID group.** Two rows share an item ID and the holder of one has an End date before the review date. Expected: one duplicates finding that gives that row's holder check with the days before the review date, and a question that names the leaver.
15. **Odd dates.** A person whose Start date is after the review date, and one whose End date is before their Start date. Expected: an unresolved item for each.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
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
```

## What to customize

- [14] days: your leaving-soon window, and the oldest people list you accept.
- The register owner's role, and whether another role decides on leavers' items.
- Your area codes and names, and an owner for every area.
- Your role list: the areas each role may open. Agree it with the area owners before the first run.
- Whether you record approved exceptions, who may approve them, and for how long.
- Your status words and item types, if they differ from the defaults, and your own export's headers.
- How often you run it, and which events start a run sooner.
- Where decisions are recorded and who carries them out in the access system and the key cabinet.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 11 November 2026. Written by Fully Powered AI from its own published map of the work, in its own words. Editorially reviewed. Tried on its invented example in three runs, the last on 12 November 2026; the record of the third is published with it. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
