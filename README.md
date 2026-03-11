# Awesome AI Skills by Kiku

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of public AI workflow skills created by Kiku.

These skills are built for agent-assisted product work: shaping ideas, reducing execution ambiguity, and keeping long-running tasks coherent. This list intentionally includes only public repositories. Private and internal skills are not listed here.

## Why this list exists

Most "prompt lists" are just snippets. These are operational skills: small, opinionated workflows that help an AI agent decide what to do next, what artifact to create, and how much process a task actually deserves.

## Skill Map

`Work Shaping -> Idea Validation -> Product Shaping -> Spec Bundle -> Continuity Ledger`

Use this sequence when a raw idea needs to become an implementation-ready piece of work without falling into PM theater or vague chat memory.

## Public Skills

| Skill | Focus | Best used when | Repo |
| --- | --- | --- | --- |
| Work Shaping | Process calibration before coding | You need to decide how much process, tracking, architecture, or review the task deserves | [work-shaping-skill](https://github.com/kiku-jw/work-shaping-skill) |
| Idea Validation | Turning ideas into honest validation briefs | The idea is still fuzzy and should not jump straight into a PRD or build | [idea-validation-skill](https://github.com/kiku-jw/idea-validation-skill) |
| Product Shaping | Choosing the smallest useful product framework | The idea has some signal, but the next product decision is still unclear | [product-shaping-skill](https://github.com/kiku-jw/product-shaping-skill) |
| Spec Bundle | Converting a loose spec into an implementation-ready bundle | A PRD is no longer enough and execution needs contracts, schema, tests, or architecture artifacts | [spec-bundle-skill](https://github.com/kiku-jw/spec-bundle-skill) |
| Continuity Ledger | Keeping substantial work coherent across sessions | The work is long-running and chat memory is not a safe source of truth | [continuity-ledger-skill](https://github.com/kiku-jw/continuity-ledger-skill) |

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

### [Spec Bundle](https://github.com/kiku-jw/spec-bundle-skill)

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

## How to use this list

- Start with Work Shaping if the real blocker is not code but the shape of the work.
- Use Idea Validation before writing a PRD for a raw product concept.
- Move to Product Shaping when there is signal, but the product decision is still fuzzy.
- Use Spec Bundle when implementation ambiguity becomes the main risk.
- Add Continuity Ledger when the task is long enough that durable memory matters.

## Machine-readable index

The same public catalog also lives in [skills.json](./skills.json).

## License

[MIT](./LICENSE)
