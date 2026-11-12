# Lone work arrangements review

For each task someone does alone, the manager gets the check-in method, the places where nobody could be reached, who responds when a check-in is missed and how soon, and alternatives. A competent person decides what is acceptable.

*Workflow template · Health, safety and environment · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/lone-work-arrangements-review/)*

## The outcome

Every task your people do alone is read against the same questions. How often does anyone hear from the person? Can the means of contact actually work at that spot, and has anyone checked? If a check-in does not come, who acts first, how long do they wait, who goes to the place, and are they on duty and close enough when it happens?

The answers arrive as a short review for each task, with the minutes worked out in view. Where the arrangements fall short, the review says exactly where and offers alternatives drawn from the facts you supplied, such as a second check-in, a different time of day or a pair. What nobody has verified stays marked as unresolved; it is never assumed fine.

A competent person and the supervisor read it and decide whether each arrangement is acceptable. The AI assistant decides nothing, tests nothing, contacts no one and changes no procedure.

## Who starts the work, and when

The operations, site or facilities manager whose staff sometimes work alone starts it. Run it when a new task starts being done alone, when a place or a rota changes, after a missed check-in or a near miss, and on the date the arrangements are next due for review. The competent person and the work's supervisor read the draft before anyone treats an arrangement as accepted.

## What they supply

- **A list of tasks,** each with its site, place, days and hours, longest stretch alone, whether it is done alone, and anything the existing risk assessment says about doing it alone.
- **A list of places,** with the means of contact available at each, whether coverage there has been checked, and when and by whom.
- **A list of responders,** with their days and hours, the minutes each needs to reach each site, and whether that has been confirmed with them.
- **The existing procedure,** in the words your people use today, for each task.
- **Your limits:** the longest time you allow between contacts, how long to wait before acting on a missed check-in, and the longest time for a responder to reach the site. Starting values come with the template.

## What comes out

One draft review in a fixed order. A header with the limits used and the counts. The tasks not reviewed and why. Then, for each task done alone: where and when, the check-ins now, the longest gap between contacts, the means of contact at that place, what happens when a check-in is missed, the longest time before a responder could be at the place if every step works, who is on duty, the findings, the facts still unresolved and the alternatives.

It ends with any responder named on two tasks at the same time, the decisions for the competent person and the supervisor, each with a blank decision line, and anything the assistant declined to do.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Health, safety and environment](https://fullypowered.ai/functions/health-safety-and-environment/), which names the competent people and owns the procedures this review reads.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where the rota decides who is alone, when and for how long.
- [Construction](https://fullypowered.ai/industries/construction/), where a person may be on a remote part of a site, a roof or a closed-off floor.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where yards, depots and early or late shifts leave one person on a site.
- [Real estate](https://fullypowered.ai/industries/real-estate/), where caretakers, cleaners and maintenance staff open and close buildings alone.
- [Energy](https://fullypowered.ai/industries/energy/), where plant rooms, substations and field sites are far from the nearest colleague.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where arrangements agreed years ago may no longer match the rota or the building.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new sites and new shifts leave more people on their own.

## What has to change for your company

Set your own limits for the longest gap between contacts, the wait before acting and the time a responder may take to arrive; the starting values are not a standard. Name your competent person and the supervisor for each kind of work, and decide which tasks are never done alone, whatever the review finds. Decide who tests contact at a place and how often, how a responder's hours and travel times are confirmed, and where decisions are recorded. The template states no legal duty and certifies nothing: the duties that apply where you operate are for your competent person to confirm. It does not find or rate hazards; that is [workplace risk assessment](https://fullypowered.ai/workflows/workplace-risk-assessment/), and this review reads what that assessment says about doing a task alone. After a missed check-in or an injury, [incident investigation and corrective actions](https://fullypowered.ai/workflows/incident-investigation-and-corrective-actions/) takes over. It runs in ChatGPT, Claude, Copilot or Gemini from the lists you supply, with no connection to any system.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026, and the record of that run is published with it. The record lists the points where the instructions were ambiguous and the edits made afterward, which have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three tasks your competent person already knows well, plus hard cases written in advance, each with its expected behavior: a coverage entry marked unverified, a responder whose hours end before the chain runs, a task marked as alone that the risk assessment says needs two people, a renamed column, a request to say whether the arrangement is lawful. The competent person checks every figure and every finding against the lists before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Workplace risk assessment](../workplace-risk-assessment/)
- [Incident investigation and corrective actions](https://fullypowered.ai/workflows/incident-investigation-and-corrective-actions/)
- [Site safety induction pack](https://fullypowered.ai/workflows/site-safety-induction-pack/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
