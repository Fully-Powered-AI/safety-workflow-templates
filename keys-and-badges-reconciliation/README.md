# Keys and badges reconciliation

Each quarter and after staff changes, the facilities or office manager sets the key and badge register beside the current staff and contractor list and the areas each role may enter. Items held by leavers, duplicates, unassigned items and access wider than the role come back as questions. Nothing is disabled.

*Workflow template · Health, safety and environment · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/keys-and-badges-reconciliation/)*

## The outcome

You know who can get into which rooms, on paper and in fact. Every key, fob and badge on your register is accounted for in one dated reconciliation, and the totals tie back to the register so nothing slips through the count.

The items that need a decision arrive sorted: badges and keys still held by people who have left (including a copy listed twice under one item number), items whose holder is no longer on any list, badges issued to nobody and keys marked lost, a second badge nobody disabled, two copies of one key, and a contractor whose badge opens a room their role does not need (in the invented example, the server room when the role only needs the plant room). Each comes with its facts, a plain question and the person whose call it is. People leaving in the next fortnight are listed too, so their items are collected on the last day rather than chased afterwards.

The register owner and the owner of each area decide. The AI assistant disables nothing, collects nothing, contacts no one, changes no record and reads no door logs.

## Who starts the work, and when

The facilities or office manager who keeps the register starts it each quarter, and again after a round of leavers, starters or role changes, or when a contractor's work ends. They supply the lists and read the draft. The owner of each restricted area, such as the IT lead for the server room or the finance manager for the records room, decides on access beyond a role. Whoever the deciders name carries the decisions out in the access system and the key cabinet.

## What they supply

- **The key and badge register:** each key, fob and badge, the number stamped on each key, the areas it opens, the holder, the date issued and its status.
- **The people list:** every member of staff and every contractor, with their role and any end date, including people who have left since the last check.
- **The role list:** the areas each role may open, as your company has agreed them.
- **The area list:** each area's code, name and owner.
- **Approved exceptions,** if you keep them: a holder allowed into an area beyond their role, who approved it and until when.
- **The review date,** and a leaving-soon window if you want something other than 14 days.

The template reads the column headers it expects and stops to ask when one does not match. No passwords, door codes or access-system logins belong in what you supply.

## What comes out

One dated reconciliation in a fixed order. A header with the counts and a tie-out line that accounts for every row of the register. Then five sections: items held by leavers, items whose holder is not on the people list, unassigned items, duplicates, and access wider than the role. Each item found carries a numbered finding and a neutral question.

Under them: the facts still missing, such as a role not on the role list; people leaving soon and what they hold; exceptions that applied; the decisions grouped by the person who makes them, each with a blank line for the decision, the name and the date; and anything the assistant declined to do. Where a section is empty it says "None."

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Health, safety and environment](https://fullypowered.ai/functions/health-safety-and-environment/), where physical security keeps restricted rooms, plant and stores closed to people who should not be there.
- [Executive and office support](https://fullypowered.ai/functions/executive-and-office-support/), where the office manager issues keys and badges and keeps the register.
- [Information security](https://fullypowered.ai/functions/information-security/), which owns the question of who can reach the server room and the records.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where client files and finance records sit behind doors that staff come and go through.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where workshops, stores and plant rooms each have their own keys and a steady flow of contractors.
- [Real estate](https://fullypowered.ai/industries/real-estate/), where property managers hold keys and fobs for buildings, plant and common areas.
- [Education](https://fullypowered.ai/industries/education/), where staff, supply staff and contractors carry keys to classrooms, offices and stores.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where keys handed out years ago are still in pockets nobody remembers.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new starters, new rooms and new contractors arrive faster than the register is kept.

It is a different piece of work from [the employee offboarding and handover checklist](https://fullypowered.ai/workflows/employee-offboarding-and-handover-checklist/), which follows one person's departure, and from [the learning system access review](https://fullypowered.ai/workflows/learning-system-access-review/), which checks software accounts rather than keys and badges.

## What has to change for your company

Write your own role list and agree it with each area owner before the first run; the template takes it as supplied and never decides what a role should open. Use your own area codes and name an owner for every area. Decide who decides on leavers' items, whether you record exceptions and who may approve them. Set your leaving-soon window and how old a people list may be. Map your register's columns to the default headers, or let the template stop and tell you which differ. It states no legal duty and certifies nothing: if an insurer or a standard sets rules for your keys and badges, your adviser confirms them. It runs in ChatGPT, Claude, Copilot or Gemini from the lists you supply, with no connection to your access control system.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 11 November 2026. It has not yet been tested in a client environment. It was tried on its invented example in three runs, the last on 12 November 2026; the record of the third is published with it. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past quarter your office manager already knows, plus cases written in advance, each with its expected result: a leaver still holding a badge, a holder matched by name only, a replacement badge never disabled, two different keys to one room, an exception that has ended, a renamed column. The register owner checks every finding against the register and the key cabinet before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 11 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 12 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Employee offboarding and handover checklist](https://fullypowered.ai/workflows/employee-offboarding-and-handover-checklist/)
- [Learning system access review](https://fullypowered.ai/workflows/learning-system-access-review/)
- [Contractor safety prequalification](https://fullypowered.ai/workflows/contractor-safety-prequalification/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
