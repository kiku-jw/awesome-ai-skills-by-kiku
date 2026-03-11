# Awesome AI Skills by Kiku

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of public AI workflow skills created by Kiku.

These skills are built for agent-assisted product work: shaping ideas, controlling execution through durable surfaces, reducing ambiguity, and turning real work into durable outputs. This list intentionally includes only public repositories. Private and internal skills are not listed here.

## Why this list exists

Most "prompt lists" are just snippets. These are operational skills: small, opinionated workflows that help an AI agent decide what to do next, what artifact to create, and how much process a task actually deserves.

## Skill Map

Core build lane:

`Work Shaping -> Idea Validation -> Product Shaping -> Product Council (if needed) -> Spec Bundle`

Workflow extensions:

- `Product Council` when one perspective is not enough and the risk is in blind spots.
- `Issue Control Loop` when GitHub should hold canonical task state and agent handoff.
- `Continuity Ledger` when the task is long enough that chat memory will drift.
- `README Generator` when a repo needs a truthful front page instead of internal-doc sprawl.
- `Session to Post` when the work is done and needs a durable writeup.

## Public Skills

| Skill | Focus | Best used when | Repo |
| --- | --- | --- | --- |
| Work Shaping | Process calibration before coding | You need to decide how much process, tracking, architecture, or review the task deserves | [work-shaping-skill](https://github.com/kiku-jw/work-shaping-skill) |
| Idea Validation | Turning ideas into honest validation briefs | The idea is still fuzzy and should not jump straight into a PRD or build | [idea-validation-skill](https://github.com/kiku-jw/idea-validation-skill) |
| Product Shaping | Choosing the smallest useful product framework | The idea has some signal, but the next product decision is still unclear | [product-shaping-skill](https://github.com/kiku-jw/product-shaping-skill) |
| Product Council | Stress-testing high-impact product decisions | The main risk is in blind spots, conflicting lenses, or a fuzzy go/no-go call | [product-council](https://github.com/kiku-jw/product-council) |
| Spec Bundle | Converting a loose spec into an implementation-ready bundle | A PRD is no longer enough and execution needs contracts, schema, tests, or architecture artifacts | [agent-spec-bundle](https://github.com/kiku-jw/agent-spec-bundle) |
| Issue Control Loop | Keeping one GitHub Issue canonical for humans and agents | Work needs durable issue state, deterministic handoff, or explicit machine-readable control | [issue-control-loop](https://github.com/kiku-jw/issue-control-loop) |
| Continuity Ledger | Keeping substantial work coherent across sessions | The work is long-running and chat memory is not a safe source of truth | [continuity-ledger-skill](https://github.com/kiku-jw/continuity-ledger-skill) |
| README Generator | Creating a human-first repo front page | A repo needs a clear README with real quick start, useful taxonomy, and less doc bloat | [readme-generator-skill](https://github.com/kiku-jw/readme-generator-skill) |
| Session to Post | Turning real coding work into a durable draft | A meaningful coding session is done and you want a build diary, post seed, or end-of-session writeup from the real artifacts | [session-to-post](https://github.com/kiku-jw/session-to-post) |

## Detailed Skill Notes

### [Work Shaping](https://github.com/kiku-jw/work-shaping-skill)

Choose the smallest honest amount of process before coding.

What it does:
- Classifies work as tiny or substantial.
- Decides whether chat is enough or the work deserves a GitHub issue.
- Chooses between no brief, a lightweight checklist, or a fuller execution brief.
- Makes architecture, review, and public-writing lanes explicit instead of accidental.

Good use cases:
- You are unsure whether a task is a one-shot fix or a multi-session effort.
- You want to decide if something should go into GitHub, a private note, or nowhere at all.
- You need to know whether a change deserves architecture work, a council pass, or just execution.

Typical prompts:
- `Is this a tiny task or substantial work?`
- `Should this go into GitHub or stay in chat?`
- `Do we need a checklist, an execution brief, or a full architecture pack?`

### [Idea Validation](https://github.com/kiku-jw/idea-validation-skill)

Turn a raw idea into a lean validation brief before it becomes a build order.

What it does:
- Forces buyer, pain, workaround, promised outcome, wedge, proof, and kill criteria into the open.
- Runs a contract-clean gate when an idea is adjacent to client work, sensitive data, or unclear rights.
- Pushes toward the fastest honest proof path, often manual service or a tiny demo.

Good use cases:
- You have an exciting idea but no named buyer or signal yet.
- You want to test demand before writing a PRD.
- You need to narrow a broad concept into one buyer, one pain, and one wedge.

Typical prompts:
- `Validate this idea before we build it.`
- `Who is the buyer and what painful recurring job are we removing?`
- `What is the smallest wedge and the fastest proof path?`

### [Product Shaping](https://github.com/kiku-jw/product-shaping-skill)

Use the smallest product framework that resolves the next real decision.

What it does:
- Selects the right framework for the current uncertainty: assumptions, experiments, opportunity-solution tree, strategy, value proposition, or pre-mortem.
- Avoids bloated PM rituals when a lighter framing would do.
- Routes the result into the right next lane instead of leaving it as a generic discussion.

Good use cases:
- The idea is validated enough to continue, but strategy or positioning is still fuzzy.
- There are too many assumptions and you need to prioritize what to test.
- You want a pre-mortem before committing to a direction.

Typical prompts:
- `Shape the product side without overdoing process.`
- `Which framework fits this decision best?`
- `Map the risky assumptions and tell me the next lane.`

### [Product Council](https://github.com/kiku-jw/product-council)

Stress-test a product decision with explicit lenses instead of fake personality roleplay.

What it does:
- runs a multi-lens council when one smart answer is not enough
- uses named roles with clear optimization targets, fears, and evidence preferences
- supports decision-shaped councils for wedge, GTM, roadmap, pricing, and go/no-go
- ends with consensus, disagreements, hidden assumptions, and one recommendation

Good use cases:
- A product decision is high-impact enough that blind spots matter.
- You want structured disagreement before committing to a direction.
- A normal strategy discussion feels too linear and is missing competing lenses.

Typical prompts:
- `Run a product council on this.`
- `Help me choose the wedge.`
- `Do a roadmap council.`

### [Spec Bundle](https://github.com/kiku-jw/agent-spec-bundle)

Build an implementation-ready spec bundle when a plain PRD is too soft.

What it does:
- Chooses the smallest bundle shape that will actually reduce ambiguity.
- Scaffolds artifacts such as `prd.md`, `contracts.md`, `schema.sql`, `test-plan.md`, and `epics.md`.
- Adds architecture artifacts like `blueprint.md`, `gate-matrix.md`, or ADRs only when risk and irreversibility justify them.

Good use cases:
- The team needs contracts, schema, and test coverage before coding can go cleanly.
- The build crosses subsystems or has a real local/cloud boundary.
- Review would be painful without clearer implementation artifacts.

Typical prompts:
- `Turn this PRD into an implementation-ready spec bundle.`
- `Add contracts, schema, and test plan.`
- `Give me the minimum bundle I can hand to an agent.`

### [Issue Control Loop](https://github.com/kiku-jw/issue-control-loop)

Turn one GitHub Issue into a clean human-agent control surface.

What it does:
- keeps the issue canonical instead of letting task state dissolve into chat
- makes machine state explicit via marker comments and deterministic parsing
- includes PRD intake and work-shaping primitives so the issue can become a clean handoff point
- keeps Projects as the board lens instead of duplicating canonical task meaning

Good use cases:
- You want GitHub Issue plus Project to become the real control layer for execution.
- A task needs a durable handoff between planning, coding, review, and operator oversight.
- You want explicit machine-readable state instead of vague workflow updates.

Typical prompts:
- `Turn this GitHub issue into a clean control loop.`
- `Use the issue as the canonical handoff surface.`
- `Parse this PRD and make it issue-ready.`

### [Continuity Ledger](https://github.com/kiku-jw/continuity-ledger-skill)

Keep substantial work coherent with a short factual `CONTINUITY.md`.

What it does:
- Creates a small durable bridge between sessions when chat memory is not enough.
- Tracks sources of truth, goals, constraints, decisions, evidence, and current state.
- Prevents long tasks from dissolving into fragmented context.

Good use cases:
- The task will span several sessions or branches.
- You expect context compaction or multiple tool loops.
- The work already has real artifacts and you need one stable bridge between them.

Typical prompts:
- `Keep continuity on this task.`
- `Update the ledger before we continue.`
- `Do not let this drift across sessions.`

### [README Generator](https://github.com/kiku-jw/readme-generator-skill)

Create or rewrite a repo README as a truthful public front page instead of an internal dump.

What it does:
- reads the repo before drafting instead of templating blindly
- identifies the repo type and chooses the smallest useful section set
- keeps quick start, usage, and value proposition on the first screen
- makes taxonomy explicit when a repo mixes tool, skill, library, app, or docs roles

Good use cases:
- The repo works, but the README is vague, stale, or overloaded.
- You want an open-source front page that explains value before implementation detail.
- The project contains multiple pieces and needs a clearer top-level framing.

Typical prompts:
- `Write a README for this repo.`
- `Rewrite this README to be clearer for outsiders.`
- `Refresh the quick start and usage sections.`

### [Session to Post](https://github.com/kiku-jw/session-to-post)

Turn a finished coding session into a durable draft instead of leaving the lessons trapped in chat and diffs.

What it does:
- turns a repo diff, saved patch, notes, or transcript into a readable development diary draft
- runs writer, critic, and editor passes so the result is shaped before you publish or file it away
- keeps the story anchored to decisions, failures, and pivots instead of file tours
- can hand the final artifact to another system with a post-save hook

Good use cases:
- The coding session is done and you want a build diary, public-safe post seed, or durable internal writeup.
- The real story lives across diff, notes, and transcript, and rewriting it manually would kill the momentum.
- You want end-of-session capture to be callable in plain language instead of only by remembering a CLI command.

Typical prompts:
- `Turn this session into a post draft.`
- `Write a build diary from this diff and notes.`
- `Make an end-of-session writeup from today's work.`

## How to use this list

- Start with Work Shaping if the real blocker is not code but the shape of the work.
- Use Idea Validation before writing a PRD for a raw product concept.
- Move to Product Shaping when there is signal, but the product decision is still fuzzy.
- Add Product Council when the decision is high-impact and you need explicit multi-lens disagreement before committing.
- Use Spec Bundle when implementation ambiguity becomes the main risk.
- Use Issue Control Loop when GitHub should become the durable human-agent control surface.
- Add Continuity Ledger when the task is long enough that durable memory matters.
- Use README Generator when the repo needs a clear public entry point more than deeper internal docs.
- Use Session to Post when the work is already real and you want a durable writeup from the session artifacts.

## Machine-readable index

The same public catalog also lives in [skills.json](./skills.json).

## License

[MIT](./LICENSE)
