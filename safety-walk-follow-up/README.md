# Safety walk follow-up

After a safety walk, the manager gets a follow-up brief that ties each concern workers raised to the commitment the manager made, its owner and due date, and the message to give back. Gaps arrive as questions, never as guesses.

*Workflow template · Health, safety and environment · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflow templates/safety-walk-follow-up/)*

## The outcome

People on the floor hear what happened to what they said. The manager walks away from the walk with every concern written down once, beside the commitment made for it, the person who owns it, the date it is due and a short message to give back to the people who raised it. A concern nobody has decided about is shown as exactly that, not left out.

The brief never turns a conversation into a promise. A concern that was discussed is not marked resolved, and a commitment is only what the manager said it is. Where an owner, a date, an owner's acceptance or a decision is missing, the brief asks the manager for it and holds the message until it is settled. The manager edits, approves and gives the messages; the AI assistant sends nothing and assigns nothing.

## Who starts the work, and when

The manager who walked the site starts it, the same day or the next, while the walk is fresh: a site, plant, warehouse or operations manager, or the safety coordinator who keeps the record. Run it again at each agreed check-in with the current status of each commitment, so overdue items and finished items that have not yet been reported back to the workers are easy to see.

## What they supply

- **The walk notes.** Each concern with a reference, the area, the role of the person who raised it and what was said. Roles, not names.
- **The commitments the manager has decided,** each with its reference, wording, owner, due date and whether the owner has accepted it. Concerns with no row stay open as decisions.
- **The give-back date,** when the manager will next speak to the people who raised the concerns, such as a shift briefing.
- **At a check-in:** the status of each commitment and the date its message was given.

## What comes out

One brief in a fixed order. A header with the walk and the counts, then every concern with its commitment, owner, due date, whether the owner accepted, a drafted message to give back and any flag. Then the decisions the manager still has to make, the commitments grouped by owner, and, at a check-in, what is overdue, what is reported done but not yet told to the workers, and what is ready for the manager to close.

A good brief can be checked against the walk notes line by line, and each worker's concern can be found in it in the words they used.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Health, safety and environment](https://fullypowered.ai/functions/health-safety-and-environment/), where promises made on the floor are the cheapest way to earn or lose trust.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where the person who runs the work also owns what is promised about it.
- [Construction](https://fullypowered.ai/industries/construction/), where a site walk produces a long list on a short timeline.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where concerns come from several shifts and lines and are easily lost between them.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where docks, yards and vehicles produce concerns that cross teams.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where walks happen on a rhythm and the follow-up lives in someone's notebook.

It is not a risk assessment. [Workplace risk assessment](https://fullypowered.ai/workflows/workplace-risk-assessment/) rates hazards and proposes controls. This workflow template keeps track of what the manager promised in response to what people said, and does not judge whether a promise is enough.

## What has to change for your company

Decide how you refer to roles so that no one is identified, and who counts as too few to be named even by role. Set the give-back occasion and who gives the messages. Decide who may be an owner and how an owner accepts. Agree the statuses your team uses, and who alone closes a concern. Add the wording you want at the close of each message, such as how to raise it again. It states no regulatory duty; your competent person confirms what applies where you operate. It runs in ChatGPT, Claude, Copilot or Gemini from notes and files you supply, and needs no connection to any of your systems.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026; the record is published with it. That run was by the model that revised the template after an earlier trial and an independent review, so it is not an independent check, and it was a first run: the check-in path has not been tried. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on one or two past walks your manager remembers well, plus hard cases written in advance, each with its expected behavior: a concern with no commitment, a commitment with no owner, an owner who has not accepted, a name in the notes, a safety device described as not working, a due date earlier than the give-back date. The manager checks every line against the notes before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Workplace risk assessment](https://fullypowered.ai/workflow templates/workplace-risk-assessment/)
- [Incident investigation and corrective actions](https://fullypowered.ai/workflow templates/incident-investigation-and-corrective-actions/)
- [Site safety induction pack](https://fullypowered.ai/workflow templates/site-safety-induction-pack/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
