# Ergonomic review inputs

For a supervisor preparing for an ergonomics assessor or a worker's complaint about a task: a task observation record of each step's movements, durations, loads and measurements as supplied, the measurements still missing, and what the people who do the task said.

*Capability template · Health, safety and environment · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/ergonomic-review-inputs/)*

## The outcome

When a task is referred for an ergonomic assessment, the assessor's first questions are always the same: what exactly do people do, for how long, how often, handling what, and what has been measured? This capability puts the answers on one record, written from what the supervisor actually saw and measured, so the assessor spends the visit assessing instead of collecting.

Each step of the task gets its own entry: the movements in the supervisor's own words, how long the step takes in one cycle (one complete run through all the steps of the task), the weights, heights and distances that were given, and the figures that were not. The record adds up what can be added up, such as time spent per step over a shift, and says plainly where a number is an estimate from a short observation. What the people who do the task said sits beside it, separate from what was observed, with the places the two disagree.

The record judges nothing. It scores no posture, rates no risk, compares no load with any limit, gives no view on anyone's health or fitness and certifies nothing. The ergonomics assessor decides what the task means and what should change.

## Who starts the work, and when

The supervisor or manager responsible for the task starts it: when an assessor is booked, when a worker or a team raises a complaint about a task, or when a task is about to change and someone wants it recorded first. They watch the task, time and weigh what they can, ask the people who do it, and run the capability the same day.

The ergonomics assessor, from inside the business or an outside adviser, receives the record and does the assessing.

## What they supply

- **A short referral brief.** The task, the location, who does it and how many, why it was referred, when it was observed, who observed it, who the assessor is, the shift and break pattern, and the working time on the task per shift.
- **The steps of the task,** in the order they are done.
- **Observation notes.** What was seen at each step, in plain words: the movements, how long things took, what was handled, where, and how often.
- **Measurements,** if any, as a table with stated column headers: weights, heights, distances, forces and times, with who took them and how.
- **Worker feedback,** if any: what the people who do the task said, by role, and what they suggested.
- **A list of photographs or video,** if any, with a line on what each one shows.

## What comes out

One task observation record in a fixed order. A header with the task, the reason for referral and what was observed. Then a record for each step: the movements as described, the time for the step in one cycle, the load, the heights and distances, the measurements supplied, the measurements not supplied and what the people who do the task said about that step.

Then the totals that follow from the figures supplied, the feedback and suggestions that belong to no single step, the photographs listed but not interpreted, the places where the inputs disagree, every measurement still missing and who could supply it, a line stating what the record does not do, and a blank handover block. A good record can be checked against the supervisor's notes line by line, and every figure in it traces to something that was supplied.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Health, safety and environment](https://fullypowered.ai/functions/health-safety-and-environment/), where task referrals, complaints and assessments are tracked and the assessor's findings are owned.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where repeated handling at benches, lines and packing stations is the everyday subject of ergonomic reviews.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where loading, picking and putting away make lifting and carrying the core of the work.
- [Construction](https://fullypowered.ai/industries/construction/), where tasks change with every site and the working position changes with them.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where long-standing tasks are done the way they always have been until someone complains.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), where higher volumes change how often and how long a task is done.

It stays distinct from [workplace risk assessment](https://fullypowered.ai/capabilities/workplace-risk-assessment/), which rates hazards and proposes controls. This capability only records the task for the person who will judge it. [Incident investigation and corrective actions](https://fullypowered.ai/capabilities/incident-investigation-and-corrective-actions/) is the right place when an injury has already happened.

## What has to change for your company

Decide who counts as the assessor and how they prefer to receive a record. Keep or change the column headers of the measurement table, and the list of figures the record asks for with each kind of movement. Decide how long an observation should run before you rely on it, and who may take measurements and with what. Decide where records are kept, who sees worker feedback, and how the people who raised a concern hear what happened next. It runs in ChatGPT, Claude, Copilot or Gemini from the notes and files you supply, with no connection to any system. Anything about a person's health goes to those qualified to handle it, not into this record.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 10 November 2026. It was tried on its invented example in Claude on 10 November 2026 in three runs: the template and its example were revised after an independent review of the first, and again after a second review, and the record of the third is published with it. The first run was made by an assistant that did not write the template; the second and third runs were made by the assistant that revised it, so they do not replace an independent one. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three tasks your assessor has already looked at, plus cases written in advance: a measurement table with a renamed column, a weight that differs between the notes and the table, a task with no timings, a worker's name and health detail in the feedback, a request to say whether a load is acceptable. The assessor checks every figure against the notes before anyone relies on the record. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete capability template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the capability drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related capabilities

- [Workplace risk assessment](https://fullypowered.ai/capabilities/workplace-risk-assessment/)
- [Incident investigation and corrective actions](https://fullypowered.ai/capabilities/incident-investigation-and-corrective-actions/)
- [Site safety induction pack](https://fullypowered.ai/capabilities/site-safety-induction-pack/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
