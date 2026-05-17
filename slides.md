---
marp: true
theme: default
paginate: true
backgroundColor: "#000000"
color: "#FFFFFF"
style: |
  :root {
    --teal:    #2DD4BF;
    --teal-2:  #5EEAD4;
    --teal-3:  #14B8A6;
    --teal-d:  #0D9488;
    --mute:    #94A3B8;
    --line:    #134E4A;
    --panel:   #0A0F0F;
  }
  section {
    background: #000000;
    color: #FFFFFF;
    font-family: 'Inter', 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
    font-size: 22px;
    line-height: 1.45;
    padding: 56px 72px;
  }
  h1 {
    color: var(--teal);
    font-size: 54px;
    line-height: 1.1;
    margin: 0 0 18px 0;
    letter-spacing: -0.5px;
    border: none;
  }
  h2 {
    color: var(--teal-2);
    font-size: 36px;
    line-height: 1.15;
    margin: 0 0 14px 0;
    letter-spacing: -0.3px;
  }
  h3 {
    color: var(--teal-2);
    font-size: 24px;
    margin: 0 0 8px 0;
  }
  h4 {
    color: var(--teal-3);
    font-size: 20px;
    margin: 0 0 6px 0;
    text-transform: uppercase;
    letter-spacing: 1.2px;
  }
  p, li { color: #FFFFFF; font-size: 22px; }
  strong { color: var(--teal-2); font-weight: 600; }
  em { color: var(--mute); font-style: normal; }
  a, a:visited { color: var(--teal-2); }
  blockquote {
    border-left: 4px solid var(--teal);
    color: #FFFFFF;
    padding: 8px 18px;
    margin: 18px 0;
    font-size: 24px;
    font-style: normal;
    background: rgba(45, 212, 191, 0.05);
  }
  code, pre { font-family: 'JetBrains Mono', 'Fira Code', Consolas, monospace; font-size: 19px; }
  pre {
    background: var(--panel);
    border: 1px solid var(--line);
    border-radius: 8px;
    padding: 16px 18px;
    color: var(--teal-2);
  }
  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 20px;
  }
  th {
    color: var(--teal);
    text-align: left;
    border-bottom: 2px solid var(--teal-d);
    padding: 10px 12px;
    font-size: 20px;
  }
  td {
    color: #FFFFFF;
    border-bottom: 1px solid #1f2937;
    padding: 10px 12px;
    vertical-align: top;
  }
  ul, ol { margin: 0 0 10px 0; padding-left: 22px; }
  ul li, ol li { margin-bottom: 8px; }
  hr { border: 0; border-top: 1px solid var(--teal-d); margin: 20px 0; }
  section::after { color: var(--teal-d); font-size: 16px; }

  /* Layout helpers */
  .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 28px; }
  .grid-3 { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 22px; }
  .grid-4 { display: grid; grid-template-columns: 1fr 1fr 1fr 1fr; gap: 18px; }
  .grid-13 { display: grid; grid-template-columns: 1fr 3fr; gap: 32px; }
  .grid-31 { display: grid; grid-template-columns: 3fr 1fr; gap: 32px; }

  .card {
    background: var(--panel);
    border: 1px solid var(--line);
    border-left: 4px solid var(--teal);
    border-radius: 8px;
    padding: 18px 20px;
  }
  .card-soft {
    background: rgba(45,212,191,0.04);
    border: 1px solid var(--line);
    border-radius: 8px;
    padding: 18px 20px;
  }
  .pill {
    display: inline-block;
    color: var(--teal);
    border: 1px solid var(--teal-d);
    border-radius: 999px;
    padding: 4px 12px;
    font-size: 18px;
    margin-right: 6px;
  }
  .kbd {
    display: inline-block;
    background: var(--panel);
    border: 1px solid var(--line);
    border-radius: 4px;
    padding: 2px 8px;
    color: var(--teal-2);
    font-family: 'JetBrains Mono', monospace;
    font-size: 19px;
  }
  .big { font-size: 88px; color: var(--teal); line-height: 1; letter-spacing: -2px; font-weight: 700; }
  .huge { font-size: 120px; color: var(--teal); line-height: 1; letter-spacing: -3px; font-weight: 700; }
  .label { color: var(--teal-3); text-transform: uppercase; letter-spacing: 2px; font-size: 18px; }
  .muted { color: var(--mute); }
  .center { text-align: center; }

  section.lead {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 64px 80px;
  }
  section.lead h1 { font-size: 72px; }
  section.divider {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    padding: 80px;
  }
  section.divider .label { color: var(--teal); font-size: 22px; }
  section.divider h1 { font-size: 84px; line-height: 1; }
  section.quote {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 80px 120px;
  }
  section.quote p { font-size: 36px; line-height: 1.3; color: #FFFFFF; }
  section.quote .attrib { color: var(--teal-2); font-size: 22px; margin-top: 24px; }
---

<!-- _class: lead -->

<span class="label">Keynote · 2026</span>

# Humans at the Heart

## Building Software in the Age of Agents

<br>

<span class="pill">Agentic SDLC</span>
<span class="pill">Human-in-the-Loop</span>
<span class="pill">Rule Zero</span>

<br>

**[Speaker Name]** · *[Title · Organisation]*

---

<!-- _class: quote -->

> Last night, while you were sleeping, an agent opened a pull request against your main branch, ran the tests, and tagged you for review.

<div class="attrib">It compiled. It passed CI. It even wrote the changelog.<br>The only question left is — <strong>whose name appears next to that commit?</strong></div>

---

<!-- _class: divider -->

<span class="label">The shift</span>

# The question
# has changed.

---

## Three years ago we asked:

<div class="grid-2">

<div class="card-soft">

<h4>Then</h4>

<h2 style="color:#FFFFFF">"Can AI help me code?"</h2>

<br>

A productivity question.
A tooling question.
A *me-and-my-editor* question.

</div>

<div class="card">

<h4>Now</h4>

<h2>"What happens when agents ship code without me?"</h2>

<br>

A governance question.
An accountability question.
A *me-and-my-team-and-the-world* question.

</div>

</div>

---

## This isn't a "Responsible AI" talk.

<br>

**It's a talk about how we ship software now.**

<br>

- Autonomous coding agents are *already* opening pull requests against production repos.
- Multi-agent workflows are *already* triaging issues, writing tests, generating release notes — every night, on schedule.
- The Model Context Protocol has turned every API into something an agent can drive.

<br>

> The interesting work isn't *whether* to adopt this.
> It's *how* to stay in command of it.

---

## About me

<div class="grid-2">

<div class="card-soft">

<h4>Speaker</h4>

**[Name]**
*[Title · Organisation]*

- Building and breaking AI-assisted dev workflows since the first wave
- Worked alongside teams shipping with coding agents in production
- I care about engineering that future humans will thank us for

</div>

<div class="card-soft">

<h4>What I've watched up close in 2025–2026</h4>

- Teams 10x their throughput — and 10x their incidents
- Audit logs where nobody could explain who approved what
- And teams that got this *beautifully* right

</div>

</div>

---

## The journey today

<div class="grid-2">

<div>

<h4>Part 1 · The Three Waves</h4>

From pair → peer → fleet.
How the operating model of software has quietly inverted.

<br>

<h4>Part 2 · Rule Zero</h4>

You own the code.
You appear in the audit log.
Accountability is the price of autonomy.

<br>

<h4>Part 3 · The AI-Native SDLC</h4>

What actually changes in your day, your repo, your pipeline.

</div>

<div>

<h4>Part 4 · Human-in-the-Loop as a Control System</h4>

Approval gates, sandboxes, traces, evals — the control plane for safe autonomy.

<br>

<h4>Part 5 · Trustworthy Agentic AI</h4>

Explainability, reliability, inclusivity — redrawn for agents.

<br>

<h4>Part 6 · The Fleet</h4>

Your new job: conductor, not typist.

</div>

</div>

---

<!-- _class: divider -->

<span class="label">Part 1</span>

# Three Waves
# of AI-Assisted
# Development

---

## The arc, at a glance

<div class="grid-3">

<div class="card">

<span class="label">Wave 1 · 2021–2023</span>

<h2 style="font-size:30px">Pair Programmer</h2>

Inline suggestions.
Autocomplete on caffeine.

<br>

**You code what you were going to code anyway — just faster.**

</div>

<div class="card">

<span class="label">Wave 2 · 2024</span>

<h2 style="font-size:30px">Peer Programmer</h2>

Synchronous agent mode.
The agent takes a bounded task while you build alongside it.

<br>

**You and the agent in the same flow, same minute.**

</div>

<div class="card">

<span class="label">Wave 3 · 2025–2026</span>

<h2 style="font-size:30px">Async Agentic SDLC</h2>

Multi-agent workflows.
Autonomous task execution.
Fleet-scale delivery.

<br>

**You guide a fleet. Outcomes ship while you sleep.**

</div>

</div>

<br>

> Each wave expands scope — from **tokens**, to **tasks**, to **end-to-end outcomes.**

---

## Wave 1 · Pair Programmer

<div class="grid-2">

<div>

<h4>What it felt like</h4>

- Ghost text at the end of your line.
- Boilerplate evaporated.
- Tests written one stub at a time.
- You were always in the driver's seat — keyboard hot, eyes on every token.

<br>

<h4>The unit of work</h4>

**A line. A function. A loop body.**

</div>

<div class="card-soft">

<h4>Trust model</h4>

- Suggestion → accept / reject
- No memory of the wider repo
- No actions taken on your behalf
- No way to break anything you didn't see

<br>

<h4>The implicit deal</h4>

> "I propose. You dispose."

</div>

</div>

---

## Wave 2 · Peer Programmer

<div class="grid-2">

<div>

<h4>What changed</h4>

- The agent moved from your *cursor* to your *project*.
- It could read the repo, run a terminal, edit multiple files, apply a refactor — *with you watching*.
- Synchronous. Bounded. You stayed in the conversation.

<br>

<h4>The unit of work</h4>

**A task. A feature slice. A bug.**

</div>

<div class="card-soft">

<h4>Trust model</h4>

- Iterative — propose, run, observe, correct
- Tool calls visible step by step
- You're still the one hitting ⏎ on changes that matter
- The session ends when you walk away

<br>

<h4>The implicit deal</h4>

> "We're pairing. I'm just very fast."

</div>

</div>

---

## Wave 3 · Asynchronous Agentic SDLC

<div class="grid-2">

<div>

<h4>What just changed</h4>

- Agents now **leave the editor**.
- They run on schedules, on events, on issue assignment.
- They open pull requests against your repo while you're at lunch.
- They orchestrate sub-agents: research, plan, implement, test, document, review.

<br>

<h4>The unit of work</h4>

**An outcome. A backlog item. A release.**

</div>

<div class="card">

<h4>Trust model</h4>

- The agent runs in a sandboxed cloud environment
- It produces an artefact: a **pull request**, an **issue triage**, a **report**
- Humans gate at the merge boundary — not at every keystroke
- Audit logs and traces are the record of work

<br>

<h4>The new implicit deal</h4>

> "I'll do the work. You decide if it ships."

</div>

</div>

---

## What actually exists in Wave 3 today

<div class="grid-2">

<div>

<h4>Autonomous coding agents</h4>

- **GitHub Copilot coding agent** — assign an issue, get a draft PR back from a cloud sandbox
- Background coding agents across IDE vendors
- Long-running, terminal-native CLI agents

<h4>Agentic workflows</h4>

- Markdown-defined repository automations
- Run inside GitHub Actions with least-privilege permissions and **safe-outputs**
- Triggered by schedule, event, or `/slash` command

</div>

<div>

<h4>The shared agent fabric</h4>

- **AGENTS.md** — an open, cross-tool spec; the "README for agents"
- **Model Context Protocol (MCP)** — the standard contract between agents and tools, with sandboxed transports, per-client consent, OAuth 2.1, audit trails
- **MCP Registry** — discoverable, governed catalogue of agent-callable capabilities
- **Skills / hooks / sub-agents** — composable units of agent behaviour

</div>

</div>

---

## The operating model has inverted

<div class="grid-3">

<div class="card-soft">

<h4>Wave 1</h4>

Helped you **type** faster.

<br>

*Linear leverage.*

</div>

<div class="card-soft">

<h4>Wave 2</h4>

Helped you **think and build** in parallel.

<br>

*Parallel leverage.*

</div>

<div class="card">

<h4>Wave 3</h4>

Changes the **operating model**:
agents execute, humans orchestrate, review, and own outcomes.

<br>

*Compound leverage.*

</div>

</div>

<br>

> As autonomy rises, **accountability concentrates** — it does not disappear.

---

<!-- _class: divider -->

<span class="label">Part 2</span>

# Rule Zero

---

<!-- _class: lead -->

<h1 style="font-size:120px;line-height:1;">You own
<br>the code.</h1>

<br>

<p style="font-size:30px;color:#FFFFFF;">Agents may code at your direction.
<br>You are accountable. You are responsible.
<br>You appear in the audit logs alongside the agent that did the work.</p>

---

## Rule Zero, said three ways

<div class="grid-3">

<div class="card">

<h4>For the engineer</h4>

The agent's PR has your reviewer name on it.
The blame line at 2am will trace to a human.
**Review like you mean it.**

</div>

<div class="card">

<h4>For the manager</h4>

You can scale the work.
You cannot delegate the accountability.
**The squad still owns the service.**

</div>

<div class="card">

<h4>For the organisation</h4>

Regulators, customers, and incident reports do not accept "the agent did it."
**Provenance is a feature, not a footnote.**

</div>

</div>

---

## The accountability compass

<div class="grid-13">

<div>

<div class="big">↑</div>

</div>

<div>

<h4>Autonomy rises ↑</h4>

- Agents take larger units of work
- More tool access, fewer keystrokes
- More work done while you're offline

<h4>Accountability concentrates → not disappears</h4>

- The reviewer's signature carries more weight, not less
- The policy author's defaults set the blast radius
- The platform team's guardrails define what *can't* go wrong

</div>

</div>

<br>

> Wave 3 doesn't kill the engineer's responsibility. **It promotes every engineer to an SRE for their own agents.**

---

## Your name in the audit log

<pre>
2026-05-17T02:47:14Z  actor=agent/copilot-coding-agent  action=push      branch=feat/checkout-refactor
2026-05-17T02:47:31Z  actor=agent/copilot-coding-agent  action=open_pr   pr=#4821
2026-05-17T08:12:08Z  actor=human/jane.doe              action=review    pr=#4821 state=approved
2026-05-17T08:12:22Z  actor=human/jane.doe              action=merge     pr=#4821 commit=sha:9f3c…
</pre>

<br>

<div class="grid-2">

<div class="card-soft">

<h4>The agent's line</h4>
Generated the diff.
Ran the tests.
Drafted the PR.

</div>

<div class="card">

<h4>The human's line</h4>
**Approved it. Merged it. Owns it.**

</div>

</div>

---

<!-- _class: divider -->

<span class="label">Part 3</span>

# The AI-Native
# SDLC

---

## "AI-Native" isn't a sticker. It's a re-shape.

<div class="grid-2">

<div class="card-soft">

<h4>AI-bolted-on</h4>

- AI lives inside the editor
- Process is unchanged
- Humans still do every stage manually
- Agents are an accelerator on one step

</div>

<div class="card">

<h4>AI-native</h4>

- Specs are written *for* agents to consume
- Repos publish **AGENTS.md** with conventions, constraints, build commands
- Tools are exposed via **MCP** with explicit scopes and consent
- Workflows are markdown-defined and version-controlled
- Humans gate at **decision boundaries**, not at typing speed

</div>

</div>

---

## The AI-native delivery loop

<pre>
   SPEC ───→ PLAN ───→ IMPLEMENT ───→ VERIFY ───→ SHIP ───→ OBSERVE ───→ LEARN
    │         │           │             │           │          │            │
  human     human +     agent (in     agent +     human     agent +      human +
  intent    agent       sandbox)      humans     gates      humans       agent
                          │             │           │          │            │
                       tools via     evals,      branch     traces,     dataset
                         MCP        red team    protection  audits      curation
</pre>

<br>

<div class="grid-3">

<div><h4>Agents drive</h4>Implementation, repetitive verification, observability synthesis.</div>

<div><h4>Humans gate</h4>Spec intent, design trade-offs, merge approval, incident response.</div>

<div><h4>Both learn</h4>Evals improve. AGENTS.md updates. The loop tightens.</div>

</div>

---

## A story · The 3am PR

<div class="grid-2">

<div>

<h4>The setup</h4>

A small team. An overflowing backlog.
An issue: *"Migrate the cart service to the new payment SDK."*

<br>

<h4>The night before</h4>

The on-call assigns the issue to the coding agent.
Adds two labels: **breaking-change-allowed: no**, **needs-design-review: yes**.

</div>

<div>

<h4>What the agent did</h4>

- Spun up a sandboxed environment
- Read AGENTS.md and the design doc linked from the issue
- Refactored 17 files across 3 services
- Ran the full test matrix
- Wrote a migration note
- Opened a draft PR — *and stopped*

<h4>What the human did at 9am</h4>

Read the diff. Pushed back on one shortcut.
Approved. Merged. **Owned it.**

</div>

</div>

---

<!-- _class: divider -->

<span class="label">Part 4</span>

# Human-in-the-Loop
# is the control system

---

## HITL: not friction, but the control plane

<br>

> Three years ago, "human-in-the-loop" was a UX pattern for ML predictions.
>
> In 2026, it is **the safety architecture** for autonomous software delivery.

<br>

<div class="grid-3">

<div class="card-soft">

<h4>In the loop</h4>
Human approves each decision.
*High-stakes, low-volume.*

</div>

<div class="card-soft">

<h4>On the loop</h4>
Human monitors, intervenes when needed.
*Medium-stakes, real-time.*

</div>

<div class="card-soft">

<h4>In command</h4>
Human sets goals, policy, and kill switches.
*High-volume autonomy.*

</div>

</div>

<br>

The right level is a function of **stakes × reversibility × blast radius.**

---

## Four control surfaces of agentic delivery

<div class="grid-2">

<div class="card">

<h4>1 · Permissions & scope</h4>

- Least-privilege tokens
- Scoped MCP servers, only what the task needs
- **`safe-outputs`** in agentic workflows — what the agent is allowed to emit
- Branch protection: agents cannot push to `main`

</div>

<div class="card">

<h4>2 · Sandboxes</h4>

- Ephemeral cloud environments per task
- Sandboxed stdio MCP servers — restricted file system and network
- No persistent secrets in the agent's workspace
- Network egress allowlists

</div>

</div>

<div class="grid-2">

<div class="card">

<h4>3 · Approval gates</h4>

- Pre-merge **human review** is non-negotiable
- Per-tool, per-session consent prompts
- Auto-approve only for explicitly whitelisted tools
- Tiered approvals by blast radius (touch infra? touch prod? touch customer data?)

</div>

<div class="card">

<h4>4 · Audit & traces</h4>

- Every tool call, with timestamp, input, output
- Trajectory logs — what the agent *thought*, not just what it *did*
- Provenance: which model, which version of AGENTS.md, which prompt
- Tamper-evident, retained, queryable

</div>

</div>

---

## Demo · GitHub Copilot coding agent

<div class="grid-13">

<div>

<h4>Live</h4>

<span class="pill">5 min</span>

</div>

<div>

<h4>What I'll show</h4>

- Assigning an issue to the agent from the GitHub UI
- The agent's plan, surfaced inside the issue
- The draft PR it opens — with diff, test output, and a description it wrote itself
- The reviewer experience: read, push back, approve

<br>

<h4>What to watch for</h4>

- The **bounded scope** — labels and AGENTS.md shape what's allowed
- The **audit trail** — who did what, when
- The **moment of accountability** — your click on "Merge"

</div>

</div>

---

## Demo · A multi-agent workflow

<div class="grid-13">

<div>

<h4>Live</h4>

<span class="pill">7 min</span>

</div>

<div>

<h4>The lineup</h4>

- **Orchestrator** — decomposes the request, never writes code itself
- **Researcher** — reads the codebase, maps dependencies
- **Planner** — produces a DAG of work
- **Implementer** — writes code TDD-style, in a sandbox
- **Reviewer** / **Critic** — challenges assumptions, blocks risky changes
- **Documentation writer** — updates AGENTS.md and the changelog

<br>

<h4>What to watch for</h4>

- The orchestrator is a **manager**, not an engineer
- Every sub-agent has a *single* responsibility
- The human enters at the **plan checkpoint** and the **merge checkpoint** — nowhere else

</div>

</div>

---

<!-- _class: divider -->

<span class="label">Part 5</span>

# Real-world
# practices

<p style="font-size:24px;color:#94A3B8">Governance + empathy
without slowing innovation.</p>

---

## AGENTS.md — the README for agents

<div class="grid-2">

<div>

<h4>What it is</h4>

A markdown file at the root of your repo that tells agents how *your* project works.

<br>

<h4>What goes in it</h4>

- Setup commands and prerequisites
- Code style and naming conventions
- Test commands and coverage expectations
- PR rules (small, conventional commits, no `main` pushes)
- Architectural decisions agents must respect
- Things agents **must not** do

</div>

<div class="card">

<h4>Why it matters</h4>

- Open spec — works across **20+ AI coding tools**
- Versioned in git, reviewed like code
- A *policy surface* the team owns together
- The single highest-leverage artefact in an AI-native repo

<br>

> If your project's invariants live only in someone's head, they'll get violated. **Write them down for the agents.**

</div>

</div>

---

## MCP — the contract between agents and the world

<div class="grid-2">

<div>

<h4>The protocol</h4>

- JSON-RPC over **stdio** or **streamable HTTP**
- Servers expose **tools**, **resources**, **prompts**
- Clients run agents that discover and invoke them
- Authorization via **OAuth 2.1** with per-client consent

<br>

<h4>What you can govern</h4>

- Which tools an agent can see
- Which actions need confirmation
- What network and filesystem the server can touch
- A complete audit trail of every call

</div>

<div class="card">

<h4>Practical implications</h4>

- Treat **MCP servers like microservices**: scoped, versioned, observable
- Run untrusted servers in **sandbox mode**
- Use the **MCP Registry** — don't install random tools
- Enforce **enterprise policy** on which servers your org can connect to

<br>

<h4>2026 directions</h4>

- **Async operations** for long-running tool calls
- Maturing governance, enterprise readiness, agent-to-agent comms

</div>

</div>

---

## Agentic workflows — automation that thinks

<div class="grid-2">

<div>

<h4>What they are</h4>

Markdown files in `workflows/` that combine:

- YAML frontmatter (triggers, permissions, **safe-outputs**)
- Natural-language instructions for a coding agent
- Compiled to GitHub Actions and run on schedule, event, or slash command

<br>

<h4>What they replace</h4>

- The 600-line YAML you were going to write
- The brittle scheduled scripts in cron
- The "someone should triage these issues" backlog

</div>

<div class="card">

<h4>Built-in guardrails</h4>

- **Least-privilege permissions** by default
- **Safe-outputs** — what the workflow is *allowed* to produce
- No raw `.yml` checked in by hand — compiled, validated, reviewed
- Same code review process as any other change

<br>

<h4>Examples in the wild</h4>

- Nightly issue triage
- Compliance scans + auto-PR for fixes
- Daily standup digests
- Stale-doc detection across the repo

</div>

</div>

---

## Eval-driven development

<div class="grid-2">

<div>

<h4>The new test pyramid</h4>

- **Unit & integration tests** — still here, still essential
- **Agent evals** — golden datasets of realistic tasks the agent must complete
- **Trajectory evals** — did the agent reason and act sensibly, not just produce the right answer?
- **Red-team evals** — prompt injection, tool misuse, scope escape

<br>

<h4>The principle</h4>

> Models change. Prompts change. AGENTS.md changes. **Your evals are the only thing that catches regressions.**

</div>

<div class="card-soft">

<h4>How teams actually run it</h4>

- Curate evals from real traces — your own users are the best dataset
- Run evals on every change to prompts, models, tools, or AGENTS.md
- Disaggregate scores by task type and by population
- Track an **eval budget** the same way you track a performance budget
- Block deploys on regressions, not on averages

</div>

</div>

---

## Observability for agents

<div class="grid-2">

<div>

<h4>What you need to see</h4>

- Every **tool call** — with inputs, outputs, latency, cost
- Every **reasoning step** the agent took
- The **prompt + context** that led to each decision
- The **diff** between agent intent and human approval

</div>

<div>

<h4>What you do with it</h4>

- Debug failed runs by replaying trajectories
- Detect drift when the same task starts costing more or going off-policy
- Feed corrections back as evals — the loop tightens
- Investigate incidents like you investigate any other production issue

</div>

</div>

<br>

> If you can't replay an agent run, you can't review your own engineering org.

---

## Cost, rate, and blast radius — all first-class

<div class="grid-3">

<div class="card">

<h4>Cost</h4>

- Per-agent, per-task spend caps
- Daily and per-PR budgets
- Alerts on runaway loops
- A finance review for agent fleets, not just cloud bills

</div>

<div class="card">

<h4>Rate</h4>

- Concurrency limits on agent fleets
- Tool-call rate limits per session
- Backoff on flaky external services
- Circuit breakers around irreversible actions

</div>

<div class="card">

<h4>Blast radius</h4>

- Production access only via human-approved playbooks
- Write actions tiered: read-only → suggest → execute
- Always reversible by default; irreversible by exception
- Kill switch — and *someone whose job it is to pull it*

</div>

</div>

---

## Pre-merge human review is non-negotiable

<br>

<div class="grid-2">

<div class="card-soft">

<h4>What "review" used to mean</h4>

- Read the diff
- Maybe run it locally
- Approve

</div>

<div class="card">

<h4>What "review" means for an agent PR</h4>

- Read the diff **and the agent's plan**
- Inspect which tools it called and why
- Verify it didn't widen scope beyond the issue
- Confirm tests cover the actual change
- Check AGENTS.md was respected
- Approve — knowing **your name lands in the audit log**

</div>

</div>

<br>

> The hardest skill in the AI-native SDLC isn't writing code. **It's reviewing it well.**

---

## Empathy is engineering — for agents too

<div class="grid-2">

<div>

<h4>Empathy for users</h4>

- Whose lives does this agent touch?
- What does it cost them if the agent is wrong?
- Are they given a human path of appeal?
- Does the agent explain itself, or just act?

<br>

<h4>Empathy for teammates</h4>

- Who's drowning in review load while others ship 30 PRs a day?
- Whose work is being attributed to whom?
- Are juniors learning, or just rubber-stamping?

</div>

<div class="card">

<h4>Empathy for the world the work goes into</h4>

- Energy cost of fleet inference — own it, report it
- Quality of jobs created and lost — see it clearly
- Communities whose data trained the system — are they represented in your reviewers?

<br>

<h4>The principle</h4>

> The team that builds with empathy ships systems that **last**. The team that doesn't, ships systems that **need to be apologised for**.

</div>

</div>

---

## Governance without gridlock

| Anti-pattern | Why it fails | The agentic fix |
|---|---|---|
| Ethics review as a final gate | Too late to change anything | Encode constraints in **AGENTS.md** and evals from day one |
| Checklist compliance | Tick-box, no real scrutiny | **Trajectory evals** that exercise the constraints |
| Central "AI safety" team | Not embedded in delivery | Ethics champions in each squad; shared MCP catalogue |
| "We'll fix it after launch" | Harm already done | Staged rollouts behind **feature flags + sandboxes** |
| No rollback plan | Irreversible by accident | **Reversibility-by-design**; tiered tool permissions |
| Manual audits | Don't scale | **Auto-generated** provenance from agent traces |

---

<!-- _class: divider -->

<span class="label">Part 6</span>

# Trustworthy
# agentic AI

<p style="font-size:24px;color:#94A3B8">Explainability · Reliability · Inclusivity
redrawn for the age of agents.</p>

---

## The trust triangle, redrawn

<div class="grid-3">

<div class="card">

<h4>Explainability</h4>

<h2>Trajectory transparency</h2>

What the agent thought, called, produced — visible and replayable.

</div>

<div class="card">

<h4>Reliability</h4>

<h2>Evals, guardrails, rollback</h2>

Predictable behaviour under change in models, tools, prompts, and the world.

</div>

<div class="card">

<h4>Inclusivity</h4>

<h2>Access, equity, sustainability</h2>

Who gets to wield this leverage — and at whose expense.

</div>

</div>

<br>

> Remove any corner and the triangle collapses. **All three must hold simultaneously.**

---

## Explainability for agents

<div class="grid-2">

<div>

<h4>From "show me your features" to "show me your trajectory"</h4>

- Every tool call, every reasoning step, recorded
- The PR description explains **why**, not just **what**
- The agent surfaces its uncertainty: *"I'm guessing at the schema here — please confirm."*
- The reviewer can replay the run, not just inspect the diff

</div>

<div class="card-soft">

<h4>What good looks like</h4>

❌ "Refactored cart service."

✅ "Refactored `Cart` to extract a `PriceCalculator` because the issue called for swapping the tax engine. Touched 4 files in `services/cart/*`. Did **not** modify the database schema (out of scope). Ran the full test suite — 412 pass, 0 fail. Flagged one assumption about discount stacking; please confirm before merge."

</div>

</div>

---

## Reliability for agents

<div class="grid-2">

<div>

<h4>Reliability ≠ "the agent was right this time"</h4>

- Predictable under model upgrades
- Predictable under prompt churn
- Predictable across teammates and use sites
- Predictable when the world drifts

<h4>The SRE mindset, applied</h4>

| Classic SRE | Agentic SDLC |
|---|---|
| SLOs / error budgets | Eval budgets per task class |
| Incident response | Trajectory replay, prompt rollback |
| Chaos engineering | Adversarial + injection testing |
| Canary deploys | Shadow runs of new models / prompts |

</div>

<div class="card">

<h4>Practical guardrails</h4>

- **Deterministic guardrails** around irreversible actions
- **Output validators** — schemas, lints, policy checks
- **Tool allowlists** + per-action confirmation
- **Rollback** at every layer: prompt, model, AGENTS.md, MCP server version
- **Kill switch** with a named owner

<br>

> Treat your agents like a production service. **Because they are one.**

</div>

</div>

---

## Inclusivity for agents

<div class="grid-2">

<div>

<h4>Who can wield this leverage?</h4>

- The senior engineer with a paid plan and a GPU budget?
- The student on a flaky connection?
- The contributor working in a language under-represented in the model?
- The team in a region where the data centre lives elsewhere?

<br>

<h4>Who reviews the agent's work?</h4>

- If the review bench is homogenous, the agent's blind spots become **your** blind spots.
- Diverse reviewers are not a *nice-to-have*. They are an **error-correction mechanism**.

</div>

<div class="card">

<h4>The billion-user test, agentic edition</h4>

If a billion developers used this agent across language, ability, region, and economic background — **who would it fail?**

<br>

- Does AGENTS.md assume English-only contributors?
- Do your evals reflect non-Western codebases and conventions?
- Is the tooling usable on a low-bandwidth connection?
- Does the cost model price out individual maintainers and OSS contributors?
- Is the energy bill of the fleet honest in your sustainability reports?

</div>

</div>

---

<!-- _class: divider -->

<span class="label">Part 7</span>

# The fleet

<p style="font-size:24px;color:#94A3B8">Your job changed
while you weren't looking.</p>

---

## A story · From six humans to six + twenty-four agents

<div class="grid-2">

<div>

<h4>The before</h4>

- 6 engineers, one platform service
- 18-month backlog
- Constant context-switching
- Burnout creeping in

<br>

<h4>The decision</h4>

Stop trying to type faster.
Start **conducting**.

</div>

<div class="card">

<h4>The after</h4>

- Same 6 engineers
- ~24 standing agents:
  triagers, doc-writers, dependency upgraders, test-fillers, release-noters, security-scanners, accessibility-checkers
- Every agent has an **owner** and a **scope**
- Every agent's work is **reviewed by a human** before merge

<br>

<h4>What changed for the team</h4>

- The work became more strategic, not more stressful
- Reviews became the craft — *taste* mattered more than typing
- The on-call rotation shrunk because the doc agent kept the runbooks fresh

</div>

</div>

---

## The conductor's new job

<div class="grid-2">

<div class="card">

<h4>Skills that compound</h4>

- **System design** — the agent can write code; only you can architect
- **Spec writing** — clear intent is the new programming
- **Review craft** — your judgement is the last line of defence
- **Eval design** — what does "good" mean for *this* task?
- **Tool curation** — which MCP servers, which scopes, which models
- **Coaching the fleet** — AGENTS.md, prompts, post-mortems

</div>

<div class="card-soft">

<h4>Skills that fade</h4>

- Rote boilerplate
- Mechanical refactors
- Copy-paste-from-StackOverflow
- One-off scripts you'll never reuse
- Manual changelog writing
- Hand-rolled YAML

<br>

<em>(They don't disappear. They just stop being where your value lives.)</em>

</div>

</div>

---

## Guiding the fleet — a working pattern

<pre>
1. INTENT        Write the issue. Be specific. Link the design doc.
2. POLICY        Apply labels. Set scope, blast radius, approval tier.
3. DELEGATE      Assign to the agent (or a multi-agent workflow).
4. OBSERVE       Watch the plan. Check the trajectory. Intervene early if needed.
5. REVIEW        Read the diff. Inspect the tool calls. Push back. Approve.
6. OWN           Merge. Your name is on it now.
7. LEARN         Feed the trace into evals. Update AGENTS.md if the agent struggled.
</pre>

<br>

> This is not "let the agent do it." This is **engineering management applied to a non-human teammate**.

---

<!-- _class: divider -->

<span class="label">Close</span>

# What we're
# actually building

---

## The stakes are different now

<div class="grid-2">

<div>

<h4>What's at stake when an agent ships code</h4>

- Production reliability for real users
- Security posture of your supply chain
- Compliance & audit-ability
- Trust between you and the humans who depend on the service
- The careers of the people on the team
- The reputation of the org

</div>

<div class="card-soft">

<h4>What's *not* at stake</h4>

- The novelty of "look, AI wrote code!"
- Headlines about productivity multipliers
- Whether your team adopted the agent first

<br>

> The competition isn't who ships fastest with agents. **It's who ships responsibly at scale, repeatedly, for years.**

</div>

</div>

---

## The opportunity

<div class="grid-2">

<div>

<h4>Teams that get this right</h4>

- Compounding leverage without compounding incidents
- Engineers doing more of the work *only humans can do*
- Codebases that stay healthy under fleet-scale change
- Audit trails that hold up under scrutiny
- A culture where saying "let's slow that agent down" is rewarded, not punished

</div>

<div>

<h4>Engineers who get this right</h4>

- Become indispensable conductors, not commodity typists
- Build a reputation for **judgement** — the most durable skill in tech
- Sleep better at night because **Rule Zero** isn't a slogan, it's a habit
- Mentor the next generation into a discipline that didn't exist five years ago

</div>

</div>

---

<!-- _class: lead -->

<h1 style="font-size:108px;line-height:1;">Trust is still
<br>the ultimate feature.</h1>

<br>

<p style="font-size:30px;color:#FFFFFF;">It is not a switch you flip before shipping.
<br>It is a property your fleet earns —
<br><strong>through every audit log entry that has your name on it.</strong></p>

---

## Your starter checklist for Monday morning

<div class="grid-2">

<div class="card">

<h4>In your repo</h4>

- [ ] Write or update **AGENTS.md** — even a one-pager
- [ ] Turn on **branch protection**; require human review on every PR
- [ ] Set up an **agent-assignable label** for clearly-scoped issues
- [ ] Define what your agents are **not** allowed to touch
- [ ] Curate a small **MCP catalogue** with explicit scopes
- [ ] Add **trajectory + tool-call logging** if you don't have it

</div>

<div class="card">

<h4>In your team</h4>

- [ ] Agree on **Rule Zero** out loud
- [ ] Name an owner for each standing agent / workflow
- [ ] Build a tiny **eval set** from your last 10 real tasks
- [ ] Schedule a monthly **agent retro** — what shipped, what surprised, what to tighten
- [ ] Plan a **kill switch drill** — make sure you can stop the fleet
- [ ] Talk about **review craft** like you talk about code craft

</div>

</div>

---

## Going deeper

<div class="grid-3">

<div>

<h4>Specs & standards</h4>

- AGENTS.md (open spec)
- Model Context Protocol (MCP)
- MCP Registry
- GitHub Agentic Workflows
- NIST AI RMF · EU AI Act

</div>

<div>

<h4>Practical patterns</h4>

- Multi-agent orchestrator + sub-agents
- Trajectory & tool-call observability
- Eval-driven dev
- Safe-outputs in CI workflows
- Sandboxed MCP servers

</div>

<div>

<h4>Communities</h4>

- Awesome Copilot (open community catalogue)
- MCP working groups
- Partnership on AI
- DAIR · AlgorithmWatch

</div>

</div>

---

<!-- _class: lead -->

<h1>Thank you.</h1>

<br>

**[Speaker Name]**
*[Email · LinkedIn · GitHub · Social handle]*

<br>

<p style="font-size:26px;color:#FFFFFF;">In the age of agents, <strong>your name on the merge button</strong>
<br>is still the most important line of code.</p>

<br>

<span class="pill">Slides</span> <span class="pill">Demo repos</span> <span class="pill">Eval starter pack</span>

---

<!-- _class: quote -->

> Q & A

<div class="attrib">The best agentic teams keep asking:<br><strong>"Who owns this — and would we be proud of the audit log?"</strong></div>
