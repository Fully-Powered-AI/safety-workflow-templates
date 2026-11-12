# Temporary change register

For a site or operations manager with temporary changes to equipment, layout or process still in place: a register of every change with its expiry date, the checks still outstanding and the procedures and training it touches, ready for the competent person who decides what happens next.

*Workflow template · Health, safety and environment · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/temporary-change-register/)*

## The outcome

Every temporary change on the site sits on one list, in the same shape each time. For each one the manager can see when it was made, who approved it, when it was meant to end, which checks have been done and which have not, and which procedures and briefings it affects. The ones that have run past their date come first, then those with no date at all, then those about to expire.

A temporary change rarely fails loudly. It gets a date, the date passes, and the guard, the rerouted aisle or the shortened cycle becomes how the site works. The register puts the date, the days past it and the unfinished checks in front of the person who can act, before the change quietly becomes permanent.

A competent person approves, extends or ends each change. The register decides nothing. It does not say a change is safe to continue, it does not extend an expiry, and it does not close a change; it lays out the facts and leaves the choice, by name, with the person who holds it.

## Who starts the work, and when

The site manager, operations manager or the person who keeps the change log starts it on the site's agreed review rhythm, monthly for example, and again before an audit, a visit from an inspector or a change of site leadership. They bring the log and the records of checks, procedure updates and briefings. The competent person, such as the site engineer or the safety lead, reads the result and makes each decision.

## What they supply

- **The change log,** one row per change, with set column headers: the change number, a description, its type (equipment, layout or process), the area, the date it was made, the owner, who approved it and when, the expiry date, how many times it has been extended, and whether it is open, extended or ended.
- **The item records,** one row per check, procedure update or briefing a change needs, with its due date, the date it was done and a reference to the evidence.
- **The settings:** the review date, the site, who decides, how far ahead to look for expiries, how long a change may stay in place before the register flags it, and how many extensions count as too many.

## What comes out

A register in a fixed order: changes past their expiry, changes with no expiry date, changes expiring soon, changes in date with items outstanding, changes in date with nothing outstanding, ended changes with items still open, ended changes with nothing open, and any rows that could not be read. Each change shows its dates, its approval, how many times it has been extended, and every item with its state. Each change that needs a decision names who decides. The register closes with numbered questions for the facts the files left out, such as a missing approver or an expiry written as "after the audit".

It is distinct from [preventive maintenance plan](https://fullypowered.ai/workflows/preventive-maintenance-plan/), which plans the routine upkeep of equipment on a calendar. This one follows the departures from normal: what was changed for now and what has to happen before it ends.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Health, safety and environment](https://fullypowered.ai/functions/health-safety-and-environment/), where a change that outlives its approval is exactly what a competent person wants to see first.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where the manager who keeps the site running is the one who makes the temporary fixes.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where a line runs on a workaround through the next order.
- [Construction](https://fullypowered.ai/industries/construction/), where site layouts, access routes and temporary works change week by week.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where a closed dock door or a moved charging bay becomes the new routine.
- [Energy](https://fullypowered.ai/industries/energy/), where a changed setting or a bridged arrangement needs an owner and an end.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where a site has accumulated years of fixes that nobody listed.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new volume forces layout and process changes faster than the paperwork follows.

## What has to change for your company

Name who decides: the competent person for your site, and what your own rules say they must confirm. Set your review rhythm, how many days ahead counts as "expiring soon", and how long a change may stay in place before it is questioned. Decide what your site counts as a change, and which of your documents the item records should point to. Agree where the log lives and who keeps it current, because the register is only as good as that file. It runs in ChatGPT, Claude, Copilot or Gemini from the exports you supply, with no connection to any system. Which changes need formal assessment, and what that assessment holds, is set by your own procedures and by the rules that apply to your site; the register does not say. [Incident investigation and corrective actions](https://fullypowered.ai/workflows/incident-investigation-and-corrective-actions/) covers what to do when a change is linked to something that went wrong, and [site safety induction pack](https://fullypowered.ai/workflows/site-safety-induction-pack/) covers what newcomers are told about the site as it now stands.

## What has been checked

Fully Powered AI wrote this workflow template in its own words. It was editorially reviewed on 10 November 2026. It was tried on its invented example on 10 November 2026; the record is published with it, and lists the edits made afterward that have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past month of your own log that the site manager already knows, plus hard cases written in advance, each with its expected behavior: a renamed column, an expiry that is not a date, a change with no approver, an extension that was never recorded, a check marked done with no evidence, an ended change with a restoration check still open. The site manager checks every date and count against the log, and the competent person confirms every decision before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Preventive maintenance plan](https://fullypowered.ai/workflows/preventive-maintenance-plan/)
- [Incident investigation and corrective actions](https://fullypowered.ai/workflows/incident-investigation-and-corrective-actions/)
- [Site safety induction pack](https://fullypowered.ai/workflows/site-safety-induction-pack/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
