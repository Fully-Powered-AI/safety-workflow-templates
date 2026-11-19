# AI workflow templates for site, operations and safety managers

FullyPowered Workflow Templates for health and safety teams turn the AI your company already pays for into a team that knows how the work is done: a site manager with the workplace risk assessment drafted for review, a safety lead with a year of incident records compared for patterns, a facilities manager with the key and badge register reconciled against current staff. 8 workflow templates, made to be customized and deployed. All plain Markdown, all free, MIT license.

We are FullyPowered AI. We build AI workflows for companies, and these are the templates we start from. We publish them because a good starting point should be open to everyone. Copy one. Change it. Make it yours.

> [!TIP]
> **Missing a template that is not listed here, or want these customized for your organization? Reach out to us.** These are templates, made to be customized and deployed. FullyPowered AI customizes and builds AI workflows, connects them to your business systems, installs them in your agents and puts them in the hands of the people who own the work. [See more examples for health and safety teams](https://fullypowered.ai/functions/health-safety-and-environment/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme) · [Have one built for your team](https://fullypowered.ai/pricing/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme). Not sure where to start? Email hello@fullypowered.ai and a person will answer.

**Who this is for**

- Owners and CEOs who want safety work prepared carefully and consistently across every site they run.
- Site, operations and safety managers who want something their team can run this week.
- The competent person who reviews each draft, signs it off and still makes every safety call.

**What these are for**

- **Your best way of doing it, for the whole team.** One piece of work, written down precisely enough that an assistant prepares it the same way every time.
- **Work you can check.** Every template says what it needs, what it produces, what it checked and what it could not.
- **A person decides.** Anything that sends, posts, pays or changes a record waits for someone to approve it.
- **Tied into your business systems.** A workflow can be designed to pull from the systems your company already runs, and even push data back into them, with guardrails and a person approving. [Browse the Connectors Directory](https://fullypowered.ai/connectors/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme).
- **Free, open and portable.** MIT-licensed plain instructions that run in the assistant or agent your team already uses: ChatGPT, Claude, Claude Code, Claude Cowork, Codex, Copilot, Gemini, Grok, Perplexity.

**Quick start**

1. **Turn your last safety walk notes into a follow-up brief.** Open ChatGPT, Claude, Copilot or Gemini. Copy the text below into a new chat, then add your own walk notes and what you decided. Remove any names first. Nothing is sent or changed, and you read the result before anyone else does.

   ```text
   You prepare the follow-up brief for one safety walk, for the manager who
   walked it. You prepare; I decide. Never make a commitment, name an
   owner, set a date, send a message, mark a concern resolved, or judge
   whether a commitment is enough. State no legal duty and say nothing
   about whether anything is safe. For each concern, link it to my
   commitment, owner, due date and whether the owner accepted. Keep the
   concern in the notes' words and replace any person's name with their
   role. Write a short message I could give back to the person who raised
   it. Where an owner, date or decision is missing, or a due date falls
   before the give-back date, flag it as a question for me and hold that
   message. Do not guess. My walk notes: [paste notes, one concern per
   line, with area and the raised-by role]. My commitments: [paste what you
   decided, with owner and due date]. Give-back date: [date]. Today:
   [date].
   ```

2. Read what comes back. It marks what it checked and what is left for you. What comes back:

   ```text
   SAFETY WALK FOLLOW-UP BRIEF: walk of Tuesday 3 November 2026

   For: Operations manager. Areas walked: Goods-in dock, Packing hall, Maintenance workshop. Prepared: Wednesday 4 November 2026, from 6 concerns and 5 commitment rows, and no status file. Give-back date: Friday 6 November 2026.
   Concerns: 6. Commitments stated: 4. Decided no action: 1. Awaiting decision: 1. Concerns flagged: 5.

   C1, Goods-in dock. Raised by: Night-shift forklift driver (the only driver on nights).
   Concern: The light at door 3 is out and the aisle is dark when the shift starts.
   Commitment: Replace the light at door 3.
   Owner: Maintenance lead. Due: Friday 6 November 2026. Owner accepted: yes.
   Message to give back: "You told us the light at door 3 is out and the aisle is dark when the shift starts. The Maintenance lead will replace the light at door 3 by Friday 6 November 2026. If it has not happened by then, tell the Operations manager."
   FLAG, needs attention now, role may identify the person: the concern describes a light as out and the aisle as dark, and the notes say there is one night-shift forklift driver. See decision 1.
   ```

3. Stop there. You will know if this is for you. When you want it fitted to your company, or built into your agents, [that is what we do](https://fullypowered.ai/pricing/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme).

A person starts every workflow, supplies the inputs and decides; the template only prepares and checks, states no legal duty, certifies nothing, and a competent person decides what is safe.

These are examples and a starting point, made to be changed to fit how your site works. Work that is not listed here can be built too, as one step or as many.

## The safety workflow templates here today

- **[Emergency drill brief](emergency-drill-brief/)**: Before a fire, evacuation or other drill, the site or office manager gets one brief: the scenario the responsible person has approved, who does what, what each observer records, and the questions for the debrief. It writes no emergency plan.
- **[Ergonomic review inputs](ergonomic-review-inputs/)**: For a supervisor preparing for an ergonomics assessor or a worker's complaint about a task: a task observation record of each step's movements, durations, loads and measurements as supplied, the measurements still missing, and what the people who do the task said.
- **[Keys and badges reconciliation](keys-and-badges-reconciliation/)**: Each quarter and after staff changes, the facilities or office manager sets the key and badge register beside the current staff and contractor list and the areas each role may enter. Items held by leavers, duplicates, unassigned items and access wider than the role come back as questions. Nothing is disabled.
- **[Lone work arrangements review](lone-work-arrangements-review/)**: For each task someone does alone, the manager gets the check-in method, the places where nobody could be reached, who responds when a check-in is missed and how soon, and alternatives. A competent person decides what is acceptable.
- **[Repeat incident pattern review](repeat-incident-pattern-review/)**: A safety lead with a year of incident records and earlier actions gets them compared in groups: confirmed causes, what was done before, and where incidents recur, with questions for the team. A competent person judges what the pattern means.
- **[Safety walk follow-up](safety-walk-follow-up/)**: After a safety walk, the manager gets a follow-up brief that ties each concern workers raised to the commitment the manager made, its owner and due date, and the message to give back. Gaps arrive as questions, never as guesses.
- **[Temporary change register](temporary-change-register/)**: For a site or operations manager with temporary changes to equipment, layout or process still in place: a register of every change with its expiry date, the checks still outstanding and the procedures and training it touches, ready for the competent person who decides what happens next.
- **[Workplace risk assessment](workplace-risk-assessment/)**: For one task or workplace, the site or operations manager gets each hazard, who could be harmed, the controls already in place, a likelihood-and-severity rating before and after, and further controls with an owner and a date, ready for a competent person to review and sign.

## How to use one

Open a folder and start with its README. Every folder stands alone, so copy the one you want and leave the rest. The templates are written for ChatGPT, Claude, Copilot and Gemini: paste the instruction block and the output format in as custom instructions, or load the folder in a product that reads `SKILL.md` packages.

To take the whole collection, press **Use this template** at the top of this page: it copies every folder into a repository in your own account, yours to change.

In every template a person starts the work, supplies the inputs and decides. The template prepares and checks. Anything that sends, posts, pays or changes a record waits for a person to approve it.

## What SKILL.md is

Each folder holds a file named `SKILL.md`. It is the technical file: the same instructions and output format as the template, in the packaged form that AI products which load instructions from a folder read. It is generated from `TEMPLATE.md`, so the two always agree. The workflow template is the whole folder; `SKILL.md` is one way of loading it. If your AI product does not read that format, use `TEMPLATE.md`.

## What "checked" means here

Each folder says exactly what was checked and when: who wrote it, that its sources and rights were reviewed, the date of its editorial review, and whether it has been tried on its example in a named AI product. Nothing is described as tested for a client unless it was. Test a template on your own past work before your team relies on it; each one comes with acceptance tests for that.

## More workflow templates

The [FullyPowered Workflows Directory](https://fullypowered.ai/workflows/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme) lists every workflow template across functions and industries, with search. A machine-readable list of this repository is in [index.json](index.json).

For the work these templates come from, by team and by task, see [AI workflow examples for health, safety and environment teams](https://fullypowered.ai/functions/health-safety-and-environment/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme).

## Licence and credits

MIT, in [LICENSE](LICENSE) and in every folder. Each folder's SOURCES.md names what the workflow template drew on. Published by [FullyPowered AI](https://fullypowered.ai/?utm_source=github&utm_medium=referral&utm_campaign=workflow-collections&utm_content=safety-readme&from=gh-safety-readme).
