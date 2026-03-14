# Awesome AI Skills by Kiku

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of public AI workflow skills maintained by Kiku.

These skills are built for agent-assisted product work: shaping ideas, controlling execution through durable surfaces, reducing ambiguity, and turning real work into durable outputs. Some are original Kiku skills, some are Codex-focused adaptations, and some are explicit inspirations from public upstream work. This list intentionally includes only public repositories. Private and internal skills are not listed here.

## Why this list exists

Most "prompt lists" are just snippets. These are operational skills: small, opinionated workflows that help an AI agent decide what to do next, what artifact to create, and how much process a task actually deserves.

## Skill Map

Core build lane:

`Work Shaping -> Idea Validation -> Product Shaping -> Product Council (if needed) -> Spec Bundle -> Execution Pack`

Workflow extensions:

- `Product Council` when one perspective is not enough and the risk is in blind spots.
- `Triage Finding` when an external link, repo, screenshot, or post needs an honest usefulness verdict.
- `Tool Scout` when build-vs-buy is open and current ecosystem research matters.
- `ADR Log` when a decision deserves durable rationale and trade-off capture.
- `Execution Pack` when Codex needs AGENTS, plan, status, tests, backlog, and resumable prompts instead of a loose spec.
- `Issue Control Loop` when GitHub should hold canonical task state and agent handoff.
- `Continuity Ledger` when the task is long enough that chat memory will drift.
- `Visual Explainer` when a browser-readable HTML artifact is clearer than chat prose.
- `AI Writing Detox` when public-facing text needs credibility instead of generic LLM polish.
- `Public Artifact Lane` when real work should become a public-ready artifact.
- `Illustration Prompt` when vague image requests need structure, references, and generator-ready precision.
- `README Generator` when a repo needs a truthful front page instead of internal-doc sprawl.
- `Session to Post` when the work is done and needs a durable writeup.

## Attribution Policy

- `Original` means the concept and current public skill structure were authored by Kiku.
- `Adapted` means the public Codex skill was materially rewritten from an identifiable upstream repository or skill.
- `Inspired` means the current skill is original, but a public repo clearly shaped the workflow, information architecture, or publishing pattern.

The machine-readable version of this attribution data lives in [`skills.json`](./skills.json).

## Public Skills

| Skill | Focus | Best used when | Repo | Origin |
| --- | --- | --- | --- | --- |
| Work Shaping | Process calibration before coding | You need to decide how much process, tracking, architecture, or review the task deserves | [work-shaping-skill](https://github.com/kiku-jw/work-shaping-skill) | Original by Kiku |
| Idea Validation | Turning ideas into honest validation briefs | The idea is still fuzzy and should not jump straight into a PRD or build | [idea-validation-skill](https://github.com/kiku-jw/idea-validation-skill) | Original by Kiku |
| Product Shaping | Choosing the smallest useful product framework | The idea has some signal, but the next product decision is still unclear | [product-shaping-skill](https://github.com/kiku-jw/product-shaping-skill) | Original by Kiku |
| Product Council | Stress-testing high-impact product decisions | The main risk is in blind spots, conflicting lenses, or a fuzzy go/no-go call | [product-council](https://github.com/kiku-jw/product-council) | Original by Kiku |
| Spec Bundle | Converting a loose spec into an implementation-ready bundle | A PRD is no longer enough and execution needs contracts, schema, tests, or architecture artifacts | [agent-spec-bundle](https://github.com/kiku-jw/agent-spec-bundle) | Original by Kiku |
| Execution Pack | Turning a PRD into a durable Codex operating pack | Codex needs AGENTS.md, plan, status, tests, backlog, and reusable execution prompts for multi-session work | [codex-execution-pack](https://github.com/kiku-jw/codex-execution-pack) | Original by Kiku |
| Triage Finding | Fact-checking and usefulness triage for outside finds | You found a post, repo, article, screenshot, video, or saved note and need to know whether it matters now or is already covered locally | [triage-finding](https://github.com/kiku-jw/triage-finding) | Adapted from [alenazaharovaux/share](https://github.com/alenazaharovaux/share/tree/main/skills/triage-finding) |
| Tool Scout | Multi-source research for build-vs-buy decisions | You want current options before building or buying the wrong thing and need GitHub, MCP, awesome-list, and web signals instead of one-source vibes | [tool-scout](https://github.com/kiku-jw/tool-scout) | Adapted from [alenazaharovaux/share](https://github.com/alenazaharovaux/share/tree/main/skills/tool-scout) |
| ADR Log | Capturing architecture decisions and trade-offs | A stack, schema, workflow, or vendor choice needs durable rationale | [adr-log](https://github.com/kiku-jw/adr-log) | Adapted from [alenazaharovaux/share](https://github.com/alenazaharovaux/share/tree/main/skills/adr) |
| Issue Control Loop | Keeping one GitHub Issue canonical for humans and agents | Work needs durable issue state, deterministic handoff, or explicit machine-readable control | [issue-control-loop](https://github.com/kiku-jw/issue-control-loop) | Inspired by [serejaris/sereja.tech](https://github.com/serejaris/sereja.tech) |
| Continuity Ledger | Keeping substantial work coherent across sessions | The work is long-running and chat memory is not a safe source of truth | [continuity-ledger-skill](https://github.com/kiku-jw/continuity-ledger-skill) | Original by Kiku |
| Visual Explainer | Turning complex structure into readable HTML artifacts | A diagram, system map, timeline, or wide table is clearer in a browser than in chat | [visual-explainer](https://github.com/kiku-jw/visual-explainer) | Adapted from [alenazaharovaux/share](https://github.com/alenazaharovaux/share/tree/main/skills/visual-explainer) via [nicobailon/visual-explainer](https://github.com/nicobailon/visual-explainer) |
| AI Writing Detox | Removing obvious AI-writing tics | A post, README, or public note needs to sound more human and more trustworthy | [ai-writing-detox](https://github.com/kiku-jw/ai-writing-detox) | Adapted from [alenazaharovaux/share](https://github.com/alenazaharovaux/share/tree/main/skills/ai-writing-detox) |
| Public Artifact Lane | Turning real work into public-ready artifacts | You need a build diary, release notes, launch post, or case study from real work | [public-artifact-lane](https://github.com/kiku-jw/public-artifact-lane) | Original by Kiku |
| Illustration Prompt | Turning vague image ideas into structured prompts | You need a generator-ready image prompt, especially when references should shape the result | [illustration-prompt](https://github.com/kiku-jw/illustration-prompt) | Adapted from [alenazaharovaux/share](https://github.com/alenazaharovaux/share/tree/main/skills/illustration-prompt) |
| README Generator | Creating a human-first repo front page | A repo needs a clear README with real quick start, useful taxonomy, and less doc bloat | [readme-generator-skill](https://github.com/kiku-jw/readme-generator-skill) | Original by Kiku |
| Session to Post | Turning real coding work into a durable draft | A meaningful coding session is done and you want a build diary, post seed, or end-of-session writeup from the real artifacts | [session-to-post](https://github.com/kiku-jw/session-to-post) | Inspired by [serejaris/blog-pipeline-template](https://github.com/serejaris/blog-pipeline-template) |
| Video Builder | Assemble narrated videos from scripts | You need a repeatable pipeline to render a narrated mp4 with TTS and simple visuals | [video-builder-skill](https://github.com/kiku-jw/video-builder-skill) | Original by Kiku |

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

### [Execution Pack](https://github.com/kiku-jw/codex-execution-pack)

Turn a PRD or raw brief into a durable Codex operating pack.

What it does:
- scaffolds `AGENTS.md`, `docs/PLAN.md`, `docs/STATUS.md`, `docs/TEST_PLAN.md`, and `docs/BACKLOG.md`
- adds reusable prompt surfaces for execution, resume, review-repair, and blocker compression
- optionally includes a `spec/` companion when contracts, schema, or architecture gates matter

Good use cases:
- A large task needs resumable repo state instead of relying on chat memory.
- Codex should keep moving milestone by milestone without constant babysitting.
- The project needs explicit validation gates, blocker format, and review-repair prompts before real rollout.

Typical prompts:
- `Turn this PRD into a Codex execution pack.`
- `Give me AGENTS, PLAN, STATUS, TEST_PLAN, and BACKLOG for this project.`
- `Build a resumable execution pack with prompts for execute, resume, and blocker compression.`

### [Triage Finding](https://github.com/kiku-jw/triage-finding)

Turn an external finding into one honest verdict and one useful next step.

What it does:
- inspects links, posts, repos, screenshots, videos, and saved idea notes
- follows primary links and fact-checks claims instead of trusting the repost
- checks whether the same skill or tool already exists locally
- maps the finding to current work instead of rewarding novelty for its own sake
- can re-triage an ideas folder against active work
- ends with `Apply now`, `Save for later`, or `Not relevant`

Good use cases:
- You found something online and need to know whether it matters to current projects.
- A post sounds convincing, but you do not trust its details until they are checked at the source.
- A repo or tool may already be installed locally and you want to avoid duplicate adoption.
- You want to decide whether a finding should become a skill, issue, note, or nothing.

Typical prompts:
- `Triage this.`
- `Look what I found.`
- `Is this useful for us?`
- `Review this ideas folder.`

### [Tool Scout](https://github.com/kiku-jw/tool-scout)

Research the current tool landscape before building or buying the wrong thing.

What it does:
- searches current tools, services, MCP servers, APIs, models, and libraries across web, GitHub, MCP catalogs, awesome-lists, and finalist package checks
- chooses sources adaptively instead of running one generic search every time
- deduplicates tools found across multiple sources and aggregates signals such as stars or archived status
- filters out trivial tasks where custom code is the better answer
- compares only the strongest candidates by fit, maturity, and integration cost
- ends with a concrete recommendation, not a bloated longlist

Good use cases:
- Build-vs-buy is genuinely open.
- The tool ecosystem changes too quickly for memory-only recommendations.
- You need to know whether there is an MCP server, strong open-source repo, or serious hosted product for the job.
- You need current options before committing engineering time or vendor budget.

Typical prompts:
- `Find tools for this.`
- `What should we use for X?`
- `Is there an MCP for this?`
- `Find a Python library for PDF generation.`

### [ADR Log](https://github.com/kiku-jw/adr-log)

Capture architecture decisions and their trade-offs before the reasoning disappears.

What it does:
- decides whether a choice is ADR-worthy
- records context, alternatives, decision, consequences, and revisit conditions
- routes the record to repo docs, GitHub issue state, or both
- keeps superseded decisions visible instead of rewriting history

Good use cases:
- A stack, schema, workflow, or vendor decision will be expensive to rediscover later.
- A task already has one canonical issue and still needs durable technical rationale.
- You want future contributors to understand not only what won, but what lost and why.

Typical prompts:
- `Record this decision.`
- `Write an ADR.`
- `Log why we chose this.`

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

### [Visual Explainer](https://github.com/kiku-jw/visual-explainer)

Turn structure-heavy material into a self-contained HTML artifact that is easier to read in a browser than in chat.

What it does:
- chooses the right format for systems, flows, comparisons, timelines, and data-heavy summaries
- generates one self-contained HTML file
- uses clear visual hierarchy instead of generic dashboard sludge
- includes starter templates for architecture, Mermaid flows, and comparison tables

Good use cases:
- A diagram or system map would explain the thing faster than prose.
- A table is too wide or dense for terminal output.
- You want a shareable visual artifact for architecture, planning, or analysis.

Typical prompts:
- `Visualize this.`
- `Make a diagram for this system.`
- `Render this table as HTML.`

### [AI Writing Detox](https://github.com/kiku-jw/ai-writing-detox)

Remove obvious AI-writing tics from drafts without flattening the real voice.

What it does:
- cuts empty hype, throat-clearing, and fake authority
- smooths out artificial LLM rhythm
- preserves meaning while making the text sound calmer and more human
- works especially well for public posts, README copy, and build diaries

Good use cases:
- A draft is acceptable in substance but sounds generically AI-written.
- Public-facing copy needs more trust and less stylistic fog.
- You want a fast cleanup pass before publishing or committing docs.

Typical prompts:
- `Make this sound less AI.`
- `Detox this draft.`
- `Clean up this README copy.`

### [Public Artifact Lane](https://github.com/kiku-jw/public-artifact-lane)

Turn real work into a public-ready artifact with evidence-first framing.

What it does:
- chooses the right artifact type for the moment
- drafts build diaries, release notes, launch posts, case studies, or demo scripts
- keeps the first screen useful and concrete
- avoids inventing results or leaking private details

Good use cases:
- You finished real work and want a public artifact instead of leaving it in chat.
- You need release notes or a launch writeup grounded in actual changes.
- You want a case study draft based on real evidence and decisions.

Typical prompts:
- `Write a build diary from this work.`
- `Make release notes.`
- `Prepare a launch writeup.`

### [Illustration Prompt](https://github.com/kiku-jw/illustration-prompt)

Turn vague image requests and reference sets into precise generator-ready prompts.

What it does:
- runs a 6-step interview covering context, style, references, scene, palette, and format
- works especially well when reference images need to shape the final prompt
- outputs a structured English prompt with scene, style, colors, atmosphere, format, and negative constraints
- supports iterative refinement by editing blocks instead of restarting from zero

Good use cases:
- You need a hero image, card visual, cover illustration, or campaign visual prompt.
- The user has references but cannot yet describe what should be borrowed from them.
- The visual brief is vague and needs to become generator-ready before image creation.

Typical prompts:
- `Write an illustration prompt.`
- `Help me make an image prompt from these refs.`
- `Turn this vague idea into a Midjourney prompt.`

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

### [Video Builder](https://github.com/kiku-jw/video-builder-skill)

Turn a script into a narrated video without a full editor.

What it does:
- Generates per-line narration with TTS.
- Renders simple frames and encodes an mp4 via ffmpeg.
- Keeps the pipeline reproducible with a JSON spec.

Good use cases:
- You need a quick narrated explainer or concept video.
- You want repeatable renders for voice and pacing iteration.
- You need to build a video from text and stills without editing software.

Typical prompts:
- `Build a short narrated video from this script.`
- `Render a 2-minute explainer with edge-tts voiceover.`
- `Assemble an mp4 from these lines and images.`

## How to use this list

- Start with Work Shaping if the real blocker is not code but the shape of the work.
- Use Idea Validation before writing a PRD for a raw product concept.
- Move to Product Shaping when there is signal, but the product decision is still fuzzy.
- Add Product Council when the decision is high-impact and you need explicit multi-lens disagreement before committing.
- Use Spec Bundle when implementation ambiguity becomes the main risk.
- Use Execution Pack when Codex needs a durable operating layer with plan, status, validation gates, and resume prompts.
- Use Triage Finding when outside material needs a verdict before it turns into noise.
- Use Tool Scout when the decision depends on what currently exists in the ecosystem.
- Use ADR Log when a real decision deserves durable trade-off capture.
- Use Issue Control Loop when GitHub should become the durable human-agent control surface.
- Add Continuity Ledger when the task is long enough that durable memory matters.
- Use Visual Explainer when the structure is easier to read in a browser artifact than in prose.
- Use AI Writing Detox when a draft is directionally fine but still sounds like generic model output.
- Use Public Artifact Lane when real work should become a public-ready artifact.
- Use Illustration Prompt when the real problem is visual direction and reference interpretation, not image generation itself.
- Use README Generator when the repo needs a clear public entry point more than deeper internal docs.
- Use Session to Post when the work is already real and you want a durable writeup from the session artifacts.

## Machine-readable index

The same public catalog also lives in [skills.json](./skills.json).

## License

[MIT](./LICENSE)
