# Repeat incident pattern review

A safety lead with a year of incident records and earlier actions gets them compared in groups: confirmed causes, what was done before, and where incidents recur, with questions for the team. A competent person judges what the pattern means.

*Workflow template · Health, safety and environment · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflow templates/repeat-incident-pattern-review/)*

## The outcome

Each incident was investigated on its own, closed on its own and filed on its own. Nobody was asked to look across them. This workflow template does that one piece of work. It lays a year of records side by side and shows which confirmed causes keep coming back, at which task or piece of equipment, what was done after the earlier events, and whether the next event came after that action was finished.

The result is a short list of groups and a list of questions. It does not say what a pattern means. The investigation lead reads it, decides which group deserves a closer look and takes that to the team.

It investigates no single event, and it certifies nothing. For one incident, use [incident investigation and corrective actions](https://fullypowered.ai/workflows/incident-investigation-and-corrective-actions/).

## Who starts the work, and when

The investigation lead, or the safety, operations or site manager who owns the incident register, starts it when a pattern is suspected, before a safety review or planning round, or on a set rhythm such as once a year. It needs the register to be de-identified before it goes in.

## What they supply

- **The incident register for the period,** as a spreadsheet export: one row per incident with its date, outcome, area, task or equipment, and the confirmed cause category and wording where one has been agreed.
- **The action list:** the actions recorded after those incidents, with owners, due dates, completion dates and any check results.
- **Their settings:** the review period, today's date, the order of outcomes from least to most serious, and the smallest group to show in full.

## What comes out

One review, in a fixed order: the groups of incidents that share a confirmed cause and a task or piece of equipment; confirmed causes that appear across different tasks; tasks with several different causes; incidents left out because no cause is confirmed yet; the gaps in the records; and numbered questions for the team.

Each group lists its incidents, the days between them, the earlier actions and whether a later incident came after an action was completed. Groups too small to show without pointing at individuals are shown by month and category only.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Health, safety and environment](https://fullypowered.ai/functions/health-safety-and-environment/), where the register and the action list sit and where the next review begins.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where the layouts, routes and routines that a pattern points at are owned.
- [Quality management](https://fullypowered.ai/functions/quality-management/), which asks the same question of defects and complaints.
- [Construction](https://fullypowered.ai/industries/construction/), where the same hazards return on each new site.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where one machine or one changeover can sit behind several events.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where vehicles, docks and people on foot meet every day.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where years of incident records exist and nobody has time to read them together.

## What has to change for your company

Name who reads the review and who decides what happens next. Agree your cause categories before the first run and keep them stable, because the groups are only as good as the labels. Set your order of outcomes, the review period and the smallest group you are willing to show in full. De-identify the register before it is supplied, and decide where the review is kept and who may see it. It runs in ChatGPT, Claude, Copilot or Gemini, from the exports you supply; it needs no access to any system.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026, and the record of that run is published with it. The record lists the points where the instructions were ambiguous and the edits made afterward, which have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past year your safety lead already knows well, plus cases written in advance: two incidents that sound alike but have different confirmed causes, a column renamed in the export, a category spelled two ways, an action marked closed with no completion date. The safety lead checks every group against the register before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Incident investigation and corrective actions](https://fullypowered.ai/workflow templates/incident-investigation-and-corrective-actions/)
- [Workplace risk assessment](https://fullypowered.ai/workflow templates/workplace-risk-assessment/)
- [Training needs analysis](https://fullypowered.ai/workflow templates/training-needs-analysis/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
