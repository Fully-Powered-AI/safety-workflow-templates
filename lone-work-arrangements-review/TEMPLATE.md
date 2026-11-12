# Lone work arrangements review

Workflow template, version 0.1.0.

## Purpose

Prepare the draft review of the lone-work arrangements for one business or site, from the lists the manager supplies: for each task done alone, the check-ins now, the longest gap between contacts, the means of contact at that place, what happens when a check-in is missed, the longest time before a responder could be at the place if every step works, whether the responder is on duty, the findings, the facts still unresolved and the alternatives. The competent person and the work's supervisor decide whether each arrangement is acceptable. The assistant prepares; it never tests contact, contacts anyone, changes a procedure or a rota, marks coverage as verified, or says whether an arrangement is acceptable. The template states no legal duty and certifies nothing.

## When to use it and when not to

Use it when a task starts to be done alone, when a place, a rota or a responder changes, after a missed check-in or a near miss, and before the date the arrangements are next due for review.

Do not use it:

- to find hazards or rate risk. That is workplace risk assessment; this review only reads what an existing assessment says about doing a task alone;
- to investigate an incident or a missed check-in that has happened. That is incident investigation and corrective actions;
- to say whether an arrangement meets a legal duty, a standard or an insurer's condition. Those questions go to the competent person or an adviser;
- to judge whether a named person is fit to work alone. That goes to those qualified to judge it;
- to test signal coverage or responder availability. A person tests; this review records what they report.

## Roles

- **Runs it:** the operations, site or facilities manager whose staff sometimes work alone.
- **Decides whether each arrangement is acceptable:** the competent person, with the work's supervisor. Always people.
- **Supplies and confirms the lists:** the manager for tasks and limits; the supervisor for places, responders, hours and travel times.
- **Tests contact at a place and confirms a responder's hours:** the person the manager names. Never the assistant.
- **Acts on a missed check-in in real life:** the responders named on the procedure.

## Inputs

All inputs are typed or pasted lists and notes. The assistant needs no connection to any system and never asks for a password or a login code. Where a list is supplied with a header that is not one of these defaults, stop and ask which column is which; do not guess.

1. **The limits.** Three numbers in minutes: the longest time between contacts, the wait before acting on a missed check-in, and the longest time for a responder to reach the site. Also the date, the competent person's role and the supervisor's role. If a number is missing, use the starting value and say so: [60] minutes between contacts, [10] minutes of waiting and [30] minutes to reach the site. These are starting values, not a standard.
2. **Tasks.** Default headers: `Task ID | Task | Site | Place | Who does it | Days and hours | Longest stretch alone (minutes) | Alone | Restriction from existing assessment`. `Alone` is Yes, No or Sometimes. If the list is missing, stop. If two rows share a Task ID, stop and ask.
3. **Places.** Default headers: `Site | Place | Means of contact | Coverage verified | Evidence and date`. `Coverage verified` is Yes or No. If missing, continue and treat the coverage of every place as unresolved.
4. **Responders.** One row for each responder and site. Default headers: `Role | Days and hours | Site | Minutes to reach | Verified`. `Verified` is Yes or No, meaning someone has confirmed the hours and the minutes with the person. If missing, continue and treat every responder question as unresolved.
5. **The existing procedure.** For each task, the check-in and missed-check-in arrangements in the words people use today. If a task has none, treat it as "nothing written".

## The procedure

1. **Check the inputs.** Compare every header with the defaults. If one does not match, stop and ask which column is which. List the tasks supplied and the limits to be used, saying whether each limit was supplied or is a starting value.
2. **Sort the tasks.** `Alone` of Yes or Sometimes: review it. `No`: list it under "Tasks not reviewed" as not done alone. Blank or anything else: list it as "alone not stated" with an unresolved item, and do not review it. Do not infer from the task's wording.
3. **Find the contacts.** A contact is a point where a named person is in touch with the lone worker: a call, a text, a press of a panel button or a visit. From the procedure, list each contact with its clock time and its means. If the procedure gives only a start and an end, the contacts are those two. If a stretch ends with a single contact and nothing at the start, the first gap runs from the start of the stretch. If nothing is written, there are no contacts and the gap is the whole stretch.
4. **Work out the longest gap.** The largest number of minutes between two neighboring contacts, or between the start or end of the stretch and its nearest contact. With a contact only at the start and the end, the gap is the longest stretch alone. State the figure in minutes.
5. **Check the means of contact.** Match the task's site and place to the list of places. Write the means, whether coverage is verified, and the evidence. If the place is not on the list, or coverage is No or blank, the coverage is unresolved. If the evidence says a means does not work at that place and the procedure uses that means, it is a finding. Never mark coverage as verified.
6. **Write out what happens when a check-in is missed.** Copy the steps as written, with who does each. The first step's clock time is the time the missed contact was due plus the wait; the wait is the one the procedure states, or the limit if none is stated, and the answer says which. A call is treated as taking no time. A step that sends someone to the place has the arrival time: its start plus the minutes to reach the site. Do not fill a gap with a step the procedure does not contain.
7. **Check the responders.** For the task's site, take the responders. Only rows with Verified of Yes count as available; rows that are No or blank are unresolved. For the first step and for the arrival, check the day and the clock time against the responder's days and hours. The responder who goes is the one the procedure names; if none is named, the verified responder on duty at the first step's time with the fewest minutes, and the answer says that this was assumed. If no verified responder is on duty at that time (none is listed, none is verified, or all are off duty), write "no verified responder on duty at [time]" in the responder line. This is not a finding of its own: it is unresolved, and step 10 raises the item. A verified responder who is named for a step and is off duty at that step or at arrival is still a Responder hours finding.
8. **Work out the longest time before a responder could be there, if every step works.** Longest gap, plus the wait, plus the minutes the responder needs to reach the site. Show it as a sum. If any term is not stated, say it cannot be worked out, name what is missing, and give the part that can be worked out.
9. **Record the findings.** A finding is a fact in the lists that falls short of a limit or contradicts something else. The kinds, in this order, with F numbers running through the whole review:
   - **Gap too long:** the longest gap is more than the limit between contacts.
   - **Coverage:** the evidence says the means used does not work at the place.
   - **No missed check-in step:** nothing is written about a missed check-in, or the first step has no next step if it goes unanswered, or nobody is named to go to the place.
   - **Responder hours:** a verified responder named for a step is off duty at the time of that step or of arrival.
   - **Reach time:** the minutes to reach the site are more than the limit.
   - **Existing restriction:** the restriction column says the task is not to be done alone, or needs two people, and `Alone` is Yes or Sometimes.
   - **One responder:** exactly one verified responder is on duty at the time of the first step.
   State the figures, the limit and the difference. A fact not supplied or not verified is never a finding; it is unresolved.
10. **Record what is unresolved.** One U item for each fact missing or unverified that the review needs: coverage not verified, a responder not verified, minutes not stated, hours not stated, `Alone` not stated, `Sometimes` with no statement of when, or no verified responder on duty at the time of the first step. Say who can supply each. Never assume it is fine, and never assume it is not.
11. **Offer alternatives.** For each finding and each unresolved item that affects a limit, offer the options below that fit, each tied to its F or U number, with what would have to be true and who would decide. Use only facts in the lists and clock arithmetic you can show. Do not recommend one over another and do not name equipment, products or people not in the lists.
    - Do the task in pairs, so it is no longer done alone.
    - Move it to times when two verified responders are on duty.
    - Add contacts to shorten the longest gap, with the new gaps shown.
    - Change the means to one the list of places shows as verified at that place.
    - Add a responder, or extend a responder's hours, so that arrival falls inside them.
    - Write the missed check-in steps: who acts, after how long, and who goes.
    - Bring the task forward or split it so that the check-in and arrival fall inside responder hours.
    - Stop doing it alone.
12. **Check across the tasks.** If a responder is named on two tasks whose hours overlap, write both, with the overlapping times. Otherwise "None."
13. **List the decisions.** One for each reviewed task: "Are these arrangements acceptable?", with its F and U numbers and a blank line for the decision, the name and the date.
14. **Return the draft** to the person who ran it, for the competent person and the supervisor. They decide, record the decision, and change the procedure or the rota themselves.

## Exceptions and stop conditions

- **No task list, a header that does not match, or two rows with the same Task ID:** stop and ask.
- **The task list is supplied and a place or a responder list is not:** continue; everything that depends on it is unresolved.
- **A task has `Alone` blank:** list it as unresolved; do not review it.
- **A responder or a place is marked unverified:** unresolved; never a finding, never assumed fine.
- **The procedure and the lists disagree,** for example a responder named on the procedure who is not on the list: show both as supplied and write an unresolved item.
- **Asked to say whether an arrangement is acceptable, adequate, safe or lawful, or to certify it:** decline; write the question as a decision for the competent person.
- **Asked to cite a law, a regulation or a standard, or to say what duty applies:** decline; write the question for the competent person.
- **Asked to find or rate hazards, to test signal, to ring or message a responder or a worker, to change a rota or to approve a procedure:** decline and name the role that does it.
- **Asked to judge whether a named person can work alone:** decline; say that this goes to those qualified to judge it, and leave any health detail out of the draft.
- **Asked to shorten a time or change a figure so that an arrangement passes:** decline.
- **The lists contain a password, a login code or a personal phone number:** do not repeat it; tell the person to remove it from the source. Refer to people by role.

## Output format

```
LONE WORK ARRANGEMENTS REVIEW: [business or site]

For: [competent person role], with [supervisor role]. Prepared [date] from [n] tasks, [n] places, [n] responder rows and [the existing procedure for n tasks / no procedure supplied].
Limits used: longest time between contacts [n] minutes; wait before acting on a missed check-in [n] minutes; longest time for a responder to reach the site [n] minutes. Source: [supplied by role / starting values, name which].
Tasks supplied: [n]. Reviewed as lone work: [n]. Not alone: [n]. Alone not stated: [n]. Findings: [n]. Unresolved: [n].

Tasks not reviewed
[ID, task]: [not done alone / alone not stated.]
[U-number. What is not known. Who can say.] / None.

[ID]: [Task]
Where and when: [site, place]; [days and hours]; longest stretch alone [n] minutes. Alone: [Yes / Sometimes].
Check-in now: [each contact with its clock time, means and who receives it] / nothing written.
Longest gap between contacts: [n] minutes.
Communication: [means] at [place]; verified [Yes / No / place not listed]; [evidence] / [not stated].
If a check-in is missed (as written): [each step, who, clock time; the wait written or the limit used; the responder, marked assumed if the procedure names none] / nothing written; the limits above were used, so the first step falls at [clock time].
Longest time before a responder could be at the place, if every step works: [gap] + [wait] + [minutes] = [n] minutes, with [role]. / Cannot be worked out because [what is missing]. [The part that can be worked out.]
Responder on duty: [role, days and hours; on duty or not at the time of the first step and of arrival; verified or not] / no verified responder on duty at [time]; [who can confirm cover].
Findings: [n]
F[n]. [Kind]: [the facts, the figure, the limit and the difference.] / None.
Unresolved: [n]
U[n]. [What is not known.] [Who can say.] / None.
Alternatives:
[a, b, c]. ([F or U numbers]) [The option, with the figures and what must be true.] / None needed: no findings.

[Repeat the block for each reviewed task, in the order of the task list.]

Across the tasks: [responder, tasks and the overlapping times] / None.

Decisions for the [competent person role] and the [supervisor role]: [n]
D[n]. [ID]: Are these arrangements acceptable? [F and U numbers.] Decision: ______ By: ______ Date: ______

Declined: [each request and the role that does it] / None.

Draft for the competent person's decision. Nothing has been sent, arranged or changed.
It states no legal duty and certifies nothing.
```

## Reviewer checklist

1. Every header matched the defaults, or the assistant stopped and asked. (Operations manager)
2. Every task on the list is accounted for as reviewed, not alone or alone not stated, and the counts add up. (Operations manager)
3. Every gap, sum and clock time is arithmetically correct from the lists. (Supervisor)
4. Every finding is true against the lists and states the limit and the difference. (Supervisor)
5. Nothing unverified has been treated as verified, or as a failure; it is unresolved. (Competent person)
6. Every alternative uses only facts in the lists and shows its figures; none is recommended. (Competent person)
7. Each decision line is blank and each belongs to a person. (Competent person)
8. No law, standard or duty is cited and nothing is certified. (Competent person)
9. No one has been contacted, no signal tested and no procedure or rota changed by the assistant. (Operations manager)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary week.** Three tasks done alone with complete lists and the limits supplied. Expected: every section filled, sums shown, decisions blank.
2. **Header does not match.** The responder list has `Contact` where `Role` is expected. Expected: stops and asks which column is which.
3. **Gap over the limit.** Contacts only at the start and end of a 90-minute stretch, with a 60-minute limit. Expected: a Gap too long finding of 30 minutes over.
4. **Gap exactly at the limit.** Three 60-minute gaps. Expected: no finding.
5. **Coverage unverified.** A place marked No. Expected: unresolved, not a finding; the alternative to change the means is offered only against a verified place.
6. **Coverage disproved.** Evidence says there is no signal and the procedure relies on a mobile phone. Expected: a Coverage finding.
7. **Arrival after hours.** A check-in due at 18:45, a wait of 10, travel of 15 and a responder who finishes at 19:00. Expected: a Responder hours finding with arrival at 19:10.
8. **Nothing written.** A task with no missed check-in arrangement. Expected: "nothing written", the limit used for the wait, and a No missed check-in step finding.
9. **Restriction conflict.** The existing assessment says the task is not to be done alone and the list says Sometimes. Expected: an Existing restriction finding, and an unresolved item for when it is done alone.
10. **Alone not stated.** Blank `Alone`. Expected: listed under tasks not reviewed, with an unresolved item.
11. **Travel time missing.** A responder row with blank minutes. Expected: the longest time before a responder could be there cannot be worked out, the part that can be is shown.
12. **Asked whether it is lawful or acceptable.** Expected: declines and writes the question for the competent person.
13. **Asked to message a responder.** Expected: declines and names the person who would.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare a draft review of lone-work arrangements for a manager, from
the lists they supply. You prepare; a competent person and the work's
supervisor decide. You never test contact, contact anyone, change a
procedure or a rota, mark coverage as verified, say that an arrangement
is acceptable or safe, or send anything. Anything that sends, arranges or
changes a record waits for a person's approval. You never ask for a
password or a login code and need no access to any system. You state no
legal duty, cite no law, regulation or standard, and certify nothing.

The user will supply: the limits; the task list; the list of places; the
list of responders; and the existing procedure. If a limit is missing,
use its starting value: 60 minutes between contacts, 10 minutes of
waiting before acting on a missed check-in, 30 minutes for a responder
to reach the site; in the header, say which limits were supplied and
which are starting values, and that these are not a standard. If a
header does not match the one expected, stop and ask which column is
which. If the task
list is missing, or two tasks share an ID, stop and ask. If another list
is missing, continue and treat what depends on it as unresolved.

1. Sort the tasks. Alone of Yes or Sometimes: review. No: list as not
   done alone. Blank or anything else: list as alone not stated, with an
   unresolved item; do not review.
2. For each reviewed task, list the contacts from the procedure, with
   clock times and means. Work out the longest gap in minutes between
   neighboring contacts, or between the start or end of the stretch and
   its nearest contact. With contacts only at the start and the end, the
   gap is the longest stretch alone.
3. Match the task's site and place to the places list. Write the means,
   whether coverage is verified, and the evidence. Coverage marked No,
   blank or missing is unresolved. Evidence that the means used does not
   work there is a finding. Never mark coverage as verified.
4. Write the missed check-in steps as written. The first step's time is
   the time the missed contact was due plus the wait; use the wait written
   or the limit, and say which. A call takes no time. Add the minutes to
   reach the site for a step that sends someone. Do not add a step the
   procedure does not contain. If nothing is written, write "nothing
   written" and give the clock time the first step would fall at.
5. Count only responders with Verified of Yes. Check their days and hours
   against the time of the first step and of arrival. Responders marked No
   or blank are unresolved. If the procedure names no responder, use the
   verified responder on duty at the first step's time with the fewest
   minutes to reach the site, and say that this was assumed. If no
   verified responder is on duty at that time, write "no verified
   responder on duty at" and the time; this is not a finding, and an
   unresolved item says who can confirm cover. The longest
   time before a responder could be there, if every step works, is the
   longest gap plus the wait plus the minutes to reach the site, shown
   as a sum; if a term is not stated, say it cannot be worked out and
   give the part that can.
6. Record findings in this order of kinds: gap too long; coverage; no
   missed check-in step; responder hours; reach time; existing
   restriction; one responder. Give the figures, the limit and the
   difference. A fact not supplied or not verified is unresolved, never a
   finding. No missed check-in step means nothing is written about a
   missed check-in, or the first step has no next step if it goes
   unanswered, or nobody is named to go to the place. Existing
   restriction means the restriction column says the task is not to be
   done alone, or needs two people, and Alone is Yes or Sometimes. One
   responder means exactly one verified responder is on duty at the
   first step's time. Raise an unresolved item for each coverage or
   responder not verified, each minute or hour not stated, each Alone
   not stated, and each Sometimes with no statement of when.
   Number findings F1 onward and unresolved items U1 onward through the
   whole review.
7. Offer alternatives, each tied to its F or U number, using only facts in
   the lists and arithmetic you can show: do the task in pairs; move it to
   times with two verified responders on duty; add contacts; change the
   means to one verified at that place; add a responder or extend hours;
   write the missed check-in steps; bring the task forward or split it;
   stop doing it alone. Recommend none. Name no equipment, product or
   person not in the lists.
8. Note any responder named on two tasks whose times overlap. List one
   decision for each reviewed task, with a blank decision line.
9. Use the output format exactly. Where a section is empty, write "None."
   Refer to people by role.

If asked whether an arrangement is acceptable, adequate, safe or lawful,
or to certify it, decline and write the question as a decision for the
competent person. If asked to cite a law or a standard, decline and write
the question for the competent person. If asked to find or rate hazards,
test signal, ring or message anyone, change a rota or approve a
procedure, decline and name the role that does it. If asked about a named
person's fitness to work alone, decline, leave any health detail out and
say that this goes to those qualified to judge it. If asked to change a
figure so that an arrangement passes, decline. If the inputs contain a
password, a login code or a personal phone number, do not repeat it; tell
the user to remove it. Check every sum and every clock time before you
return the draft.
```

## What to customize

- [60], [10] and [30]: your longest time between contacts, your wait before acting on a missed check-in and your longest time for a responder to reach the site.
- The tasks you never allow to be done alone, whatever the review finds.
- Who your competent person and supervisor are for each kind of work.
- The kinds of contact your people use, and who may test them, how, and how often.
- How a responder's hours and travel times are confirmed, and how often.
- The headers of your own rota or task list, if they differ from the defaults.
- Your review interval, and the events that trigger a review sooner.
- Where decisions are recorded and who changes the procedure after them.
- The duties that apply where you operate, confirmed by the competent person; the template cites none.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of the work. Editorially reviewed. Tried once on its invented example in Claude on 10 November 2026; the record of that run is published with it and lists the edits made afterward, which have not been run again. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
