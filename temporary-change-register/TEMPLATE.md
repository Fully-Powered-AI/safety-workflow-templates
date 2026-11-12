# Temporary change register

Workflow template, version 0.1.0.

## Purpose

Prepare the register of temporary changes for one site from the manager's own change log and item records: every change to equipment, layout or process that was made for a time, with its approval, its expiry date and how far past it, how many times it has been extended, the checks still outstanding, and the procedures and training it touches, each with its state. The changes are sorted so the ones past their date come first. The assistant prepares; it never approves, extends, restores or ends a change, never says a change is safe to continue, and never changes a record. A competent person, named in the settings, decides each flagged change.

## When to use it and when not to

Use it on the site's agreed review rhythm, before an audit or an inspector's visit, when site leadership changes, and after any period in which many quick fixes were made.

Do not use it:

- to plan routine upkeep of equipment on a calendar. That is the preventive maintenance plan, a separate piece of work;
- to decide whether a proposed change may be made, or to assess the hazards it creates. That belongs to the people and procedures the site has for assessing changes;
- to investigate why something went wrong after a change. That is an investigation, a separate piece of work;
- to say which changes the site's rules require to be assessed or reported. The competent person confirms that;
- when a change is unsafe now. Deal with it under the site's own arrangements first. A change is unsafe now only when the person says so or a file states it; an overdue item or an expired date does not by itself make it so.

## Roles

- **Runs it:** the site manager, operations manager or the person who keeps the change log.
- **Keeps the files current:** the role the register is prepared for, for the change log, and the owner named on each change, for its item records.
- **Decides each change (restore, extend or reassess):** the competent person the settings name, for example the site engineer. Always a person. If the settings name nobody, the register says "decider not named" and raises a question.
- **Owns each change:** the role in the `owner` column.
- **Answers the questions:** the role each question names. A question about a change is answered by that change's owner. A question about a row that was not read is answered by the owner in that row if it has one; if the owner is blank, or the row is an item with no matching change, or the decider is not named, by the role the register is prepared for. No other role is named unless a file or the settings give it.

## Inputs

1. **The change log,** one row per change, with these column headers: `change_id`, `description`, `type`, `area`, `date_made`, `owner`, `approved_by`, `approval_date`, `expiry_date`, `extension_count`, `status`. Dates are written YYYY-MM-DD. `type` is equipment, layout or process. `status` is open, extended or ended; extended is treated as open. If the status is extended and `extension_count` is 0 or blank, print the count as the log gives it ("Extended 0 times"), do not infer that an extension was made, and change nothing. Upper and lower case are ignored in `type` and `status`, so "Equipment" and "equipment" are the same. A blank `extension_count` counts as 0. A blank `expiry_date` means no expiry was recorded. A blank `approved_by` means no approval was recorded. If the log is missing, stop and ask.
2. **The item records,** one row per check, procedure update or briefing a change needs, with these column headers: `change_id`, `item`, `kind`, `due_date`, `done_date`, `evidence`. `kind` is check, procedure or training. A blank `done_date` means not done. `evidence` is a reference to the proof, such as a signed page, a roster or a report number. If the file is missing, write "no item records supplied" and carry on; every change then shows "no items recorded".
3. **The settings:** the site, the review date, the role the register is prepared for, the competent person who decides each change, the expiring-soon window in days, the in-place-too-long limit in days, and the extended-too-often limit. Defaults where a setting is missing, and say which were used: window 30 days, in place too long 180 days, extended too often 2 times. If the review date is missing, stop and ask; it is never taken from the assistant's own clock.

**Column headers.** If any file's headers do not match the ones above (renamed, missing or extra), stop and ask which column holds what. Never guess.

The assistant works from the files the person supplies. It needs no access to any system and never asks for a password or a login code. It refers to people by role; if a file names a person, it uses the role and notes that a name was left out.

## The procedure

1. **Check the inputs.** Confirm the headers of both files. Count the rows in each. If two change log rows share a `change_id`, stop and ask.
2. **Read the log rows.** A row is not read, and goes under "Rows not read" with its reason, if: `change_id` is blank; `date_made` is not a date; `expiry_date` is not blank and not a date; `status` is not open, extended or ended; `extension_count` is not a whole number; or `type` is not equipment, layout or process (ignoring case). A date that is not a date is never repaired or guessed, so "after the audit" and "end of Q1" are not read.
3. **Read the item rows.** An item row is not read if: `kind` is not check, procedure or training; `due_date` is blank or not a date; `done_date` is not blank and not a date, or is later than the review date; or its `change_id` is not a change in the log (reason: no matching change). An item row for a change whose log row was not read is also listed, with that reason.
4. **State each item.** In this order:
   - done with evidence: a `done_date` and an `evidence` reference;
   - done, evidence not supplied: a `done_date` and no `evidence`;
   - open and overdue: no `done_date` and a `due_date` before the review date, with the days overdue (review date minus due date);
   - due today, or due in n days: no `done_date` and a `due_date` on or after the review date.
   An item is outstanding if it is open or done with no evidence supplied. A done date after the due date is not a problem on its own; it is shown as written.
5. **Work out each change's dates.** Days ago for `date_made` is the review date minus the date. For an open change with an `expiry_date`: if the expiry is before the review date, it has expired, and the days ago is the review date minus the expiry; if it is the review date or later, the days until expiry is the expiry minus the review date, and an expiry on the review date is written "expires today" in place of "in 0 days". An ended change's expiry date is not examined, and an ended change is never called expired.
6. **Place each change in one section,** taking the first that fits:
   - open and expired: section 1;
   - open with no `expiry_date`: section 2;
   - open and expiring within the window (the review date through the review date plus the window, both days included): section 3;
   - open, in date, with an outstanding item or no item rows: section 4;
   - open, in date, every item done with evidence: section 5;
   - ended with an outstanding item: section 6;
   - ended, with no outstanding item, or with no item rows: section 7.
   Within a section, order changes by expiry date, earliest first; in section 2 by `date_made`, oldest first; in sections 6 and 7 by `change_id`. A change with no item rows says "no items recorded" under Items and carries that flag.
7. **Flag.** For each change put its flags on its line: approval not recorded (`approved_by` blank, any status); in place over [limit] days (open, and days since `date_made` greater than the limit); extended [limit] or more times (open, and `extension_count` at or above the limit); no items recorded. Count each kind once per change.
8. **Write the decision line** for each change in sections 1 to 3: the named decider chooses whether to restore, extend or reassess, and nothing is recorded as decided. Recommend none of the three. Sections 4 to 7 carry no decision line.
9. **Write the questions.** One numbered question for each missing or unreadable fact, in this order: approval not recorded; expiry date not recorded; evidence not supplied for a done item; a row not read; an item with no matching change; decider not named. Each question names the change or row, says what is missing, and says which role can answer, by the rule under Roles. Long-in-place and extended-too-often flags are shown on the change; they are not questions, because the facts are in the files. If there are none, write "None."
10. **Write the counts line.** It must agree with the sections: open changes by section; ended changes by section; the four flag counts; rows not read. A change whose log row was not read is in no section, so it is not counted in "[n] open changes" or "[n] ended changes"; it is counted once under rows not read.
11. **Return the draft** to the person it is prepared for. People decide the changes, update the log, close the items and chase the evidence.

## Exceptions and stop conditions

- **A change is unsafe now (the person says so, or a file states it):** stop. Do not infer it from overdue items or expired dates. Tell the person to deal with it under the site's own arrangements before anything else.
- **No change log, no review date, or column headers that do not match:** stop and ask.
- **Two changes with the same `change_id`:** stop and ask.
- **A date, a status or a type that cannot be read:** do not guess; list the row under "Rows not read" and ask.
- **An expired change:** never treat it as extended. It stays expired until the log shows otherwise.
- **Asked to extend an expiry, mark a change ended or restored, or say a change may continue:** decline; the named decider does that, and the log is changed by a person.
- **Asked to recommend restore, extend or reassess:** decline; list the facts and the decider.
- **Asked to approve a new change, assess its hazards, or say which changes the site's rules require to be assessed or reported:** decline; those belong to the site's competent people and procedures.
- **Asked to write a routine maintenance calendar:** decline and point to the preventive maintenance plan.
- **Asked to notify anyone, update the log, close an item or set a date:** decline and name the role that does it.
- **The files contain a password, a login code or a person's name in connection with a fault:** do not repeat it; refer to the role and tell the person to remove it from the source.

## Output format

```
TEMPORARY CHANGE REGISTER: [site], review as of [date]

For: [role]. Prepared from the change log and item records supplied. Nothing here approves, extends or ends a change.

Counts: [n] open changes: [n] expired, [n] with no expiry date, [n] expiring within [window] days, [n] in date with items outstanding or not recorded, [n] in date with nothing outstanding. [n] ended changes: [n] with items still open, [n] with nothing open. Flags: approval not recorded [n]; in place over [limit] days [n]; extended [limit] or more times [n]; no items recorded [n]. Rows not read: [n].

1. Expired: [n]

[change_id] [description]. [Type], [area]. Owner [owner]. Made [date] ([n] days ago). Approval: [role on date, or "not recorded"]. Expired [date] ([n] days ago). Extended [n] times. Flags: [flags, or none].
Items: [item] ([kind]): [done date, evidence reference | done date, evidence not supplied | due date, n days overdue | due date, in n days | due today]. [next item]. [or "no items recorded"]
Decision: [decider] chooses whether to restore, extend or reassess. Nothing is recorded as decided.

2. No expiry date recorded: [n]

[same lines, with "No expiry date recorded." in place of the expiry line]

3. Expiring within [window] days: [n]

[same lines, with "Expires [date] (in [n] days)." in place of the expiry line, or "Expires today." when the expiry is the review date]

4. In date, items outstanding or not recorded: [n]

[same lines, with "Expires [date] (in [n] days)." and no Decision line]

5. In date, nothing outstanding: [n]

[change_id] [description]. Expires [date]. [n] of [n] items done with evidence.

6. Ended, items still open: [n]

[change_id] [description]. Ended. Owner [owner].
Items: [as above]

7. Ended, nothing open: [n]

[change_id] [description]. [n] of [n] items done with evidence, or "No items recorded."

8. Rows not read: [n]

[File, change_id]: [reason].

Questions: [n]
1. [Change or row]: [the missing fact]. [Role] can answer.

Every date and count traces to the change log and item records supplied, with [review date] as the reference. The register changes no records and sends nothing.
```

Notes on the format:

- **[site]** is the site setting. If the setting is a list, print its first entry only.
- **[Type]** is printed with a capital first letter. **[area]** is printed as the log gives it, with no change of case.
- **Approval.** Both `approved_by` and `approval_date` filled: "[role] on [date]". Only `approved_by` filled: "[role], date not recorded". Only `approval_date` filled: "not recorded (a date, [date], is given with no person)". Neither: "not recorded". The flag "approval not recorded" is for a blank `approved_by`; a blank `approval_date` alone gets no flag but does get the first question.
- **Rows not read** are printed exactly as "[File, change_id]: [reason]." with nothing added to the line.

Where a section is empty, print its heading with ": 0" and the word "None." under it. Where there are no questions, print "Questions: 0" and "None."

## Reviewer checklist

1. Every date is the date in the log, and every "days ago" and "in n days" figure is counted from the review date. (Site manager)
2. Each change is in the section its dates and items call for, and no ended change is called expired. (Site manager)
3. Every item shown as done has the done date and evidence the item records show, and any done item without evidence is marked so. (Owner of the change)
4. The counts line agrees with the sections. (Site manager)
5. No change is described as safe, approved, extended or restored, and no decision is recommended. (Competent person)
6. Every row that could not be read is listed with its reason, and nothing was repaired. (Site manager)
7. Every question names a role that can answer it. (Site manager)
8. The competent person has decided each change in sections 1 to 3, and the log has been updated by a person afterwards. (Competent person)

## Acceptance tests

Proposed tests. None has been run.

1. **Expired change.** Open, expiry 2026-10-31, review date 2026-12-07. Expected: section 1, "37 days ago", a decision line naming the decider.
2. **Ended change past its old expiry.** Status ended, expiry before the review date. Expected: never called expired; section 6 or 7 by its items.
3. **No expiry date.** Blank `expiry_date`. Expected: section 2 with "No expiry date recorded".
4. **Window edge.** Expiry exactly the review date plus the window. Expected: section 3. One day later: section 4 or 5.
5. **Expiry that is not a date.** "after the audit". Expected: under "Rows not read" and a question; not placed in a section.
6. **No approver.** Blank `approved_by`. Expected: "Approval: not recorded", the flag, and the first question.
7. **Done without evidence.** `done_date` set, `evidence` blank. Expected: shown as done, evidence not supplied; the change counts as having an outstanding item; a question.
8. **Item with no change.** Expected: under "Rows not read" with "no matching change"; a question.
9. **Renamed column.** `expires` in place of `expiry_date`. Expected: stops and asks which column holds what.
10. **Asked to extend an expiry.** Expected: declines and names the decider.
11. **Counts agree.** Add the section totals. Expected: the counts line matches.

## Instructions for the AI assistant

```
You prepare the temporary change register for a site from the change log
and item records the person supplies. You never approve, extend, restore
or end a change, never say a change is safe to continue, never recommend
a decision, and never change a record or send anything. A named competent
person decides each change.

The user will supply: the change log with the headers change_id,
description, type, area, date_made, owner, approved_by, approval_date,
expiry_date, extension_count, status; the item records with the headers
change_id, item, kind, due_date, done_date, evidence; and the settings
(site, review date, who decides, expiring-soon window, in-place-too-long
limit, extended-too-often limit). If the change log or the review date is
missing, stop and ask. If any header does not match, stop and ask which
column holds what. If the item records are missing, write "no item records
supplied" and carry on; every change then shows "no items recorded". Dates
are YYYY-MM-DD. Take the review date from the settings, never from your
own clock. Defaults if unset: window 30 days, in place too long 180 days,
extended too often 2 times; say which were used. Refer to people by role; if a file names a person, use the role and
say a name was left out. If a change is unsafe now, stop and tell the person
to deal with it under the site's own arrangements first. A change is unsafe
now only if the person says so or a file states it; never infer it from
overdue items or expired dates.

1. Stop and ask if two change log rows share a change_id. Leave a row out
   and list it under "Rows not read" with its reason if a required date,
   status, type or count cannot be read (ignore upper and lower case in
   type and status), or an item row has no matching change, a bad kind, no
   due date, or a done date after the review date. An item row whose change
   was not read is also listed. Never repair or guess a date.
2. State each item as done with evidence, done with evidence not supplied,
   overdue by n days (review date minus due date), due in n days or due
   today. Outstanding means open or done with no evidence.
3. Status extended is treated as open. A blank extension_count counts as
   0 (if the status is extended and the count is 0 or blank, print the count
   as given and infer nothing); a blank approved_by means no approval was
   recorded. For an open change, expired means expiry before the review
   date; count days from the review date; an expiry on the review date is
   written "expires today". An ended change is never called expired.
4. Place each change in the first section that fits: 1 open and expired;
   2 open with no expiry date; 3 open expiring within the window (the review
   date and the last day of the window both count); 4 open, in date, with
   an outstanding item or no item rows; 5 open, in date, all items done
   with evidence; 6 ended with an outstanding item;
   7 ended otherwise. Order sections 1, 3, 4 and 5 by expiry date,
   earliest first; section 2 by date_made, oldest first; sections 6 and 7
   by change_id.
5. Flag: approval not recorded (any status); in place over the limit and
   extended the limit or more times (open changes only); no items
   recorded.
6. For sections 1 to 3 write: the decider chooses whether to restore,
   extend or reassess, and nothing is recorded as decided.
7. Ask one numbered question for each missing or unreadable fact, in this
   order: approval not recorded; expiry date not recorded; evidence not
   supplied for a done item; a row not read; an item with no matching
   change; decider not named. Name the role that can answer: the change's
   owner; for a row not read with a blank owner, an item with no matching
   change, or no decider named, the role the register is prepared for.
   Name no other role. A long time in place or too many extensions is
   flagged, not asked.
8. Write the counts line so that it agrees with the sections. A change
   whose row was not read is in no section and is not counted as open or
   ended; it is counted under rows not read.
9. Use the output format exactly. Print the site as the first entry of
   the site setting, the type with a capital first letter and the area as
   the log gives it. Print approval as "role on date"; with only the role,
   "role, date not recorded"; with only a date, "not recorded (a date,
   [date], is given with no person)"; with neither, "not recorded". In
   each of the last three cases ask the approval question. Print each row
   not read as "[File, change_id]: [reason]." Print an empty section as
   ": 0" with "None." under it. End with the trace line: "Every date and
   count traces to the change log and item records supplied, with the
   review date as the reference. The register changes no records and sends
   nothing."

Decline requests to extend an expiry, end or restore a change, recommend
a decision, assess hazards, say what the site's rules require, or notify
anyone. Name the person or role who does that instead.
```

## What to customize

- Who decides, and what your own rules say they must confirm.
- The review rhythm, the expiring-soon window, the in-place-too-long limit and the extended-too-often limit.
- What your site counts as a change, and the types it uses.
- The kinds of item you track, and what counts as evidence for each.
- The columns your log already has, mapped to the headers above.
- Who receives the register, and where decisions are recorded.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Tried on its invented example on 10 November 2026; the record is published with it, and lists the edits made afterward that have not been run again. Not yet tested in a client environment.
