# AI Builder Project Library

A curated library of project ideas to inspire Domain Consultants based on their own AI skill level, curiosity, and interests.

These are not assignments. They are starting points that can be made simpler or more advanced depending on the builder.

---

## Context & Personalization Projects

### DC Context Pack
Build a portable context package that helps an AI understand the Domain Consultant role, customer-facing goals, product/technical boundaries, preferred communication style, evidence requirements, and “do not assume” rules.

**Start simple**
Write one reusable context block and test it on the same task with and without the context.

**Evolve it**
- Version the context.
- Add role-specific variants.
- Test for stale or conflicting instructions.
- Add evaluation criteria for output quality.

**Inspired by**
Summer Adventure: Pack Your ID

---

### Personal / Team Knowledge Brain
Create a small persistent knowledge system around approved/public/synthetic content.

**Start simple**
Load a small set of reference material and test retrieval quality.

**Evolve it**
- Add source provenance.
- Add freshness rules.
- Add retrieval evaluations.
- Explore permissions and role-based access.

**Inspired by**
Summer Adventure: Grow a Personal Brain

---

## Reusable Skill Projects

### Discovery Critic
Build a reusable skill that reviews a discovery plan and identifies weak assumptions, missing questions, unsupported conclusions, and blind spots.

**Start simple**
Use one well-structured prompt/skill against a synthetic discovery plan.

**Evolve it**
- Add a scoring rubric.
- Add a second evaluator.
- Compare generic vs. DC-context-aware output.
- Add explicit uncertainty handling.

---

### Technical Storyline Skill
Create a reusable skill that turns architecture details into clear customer-relevant implications without inventing a sales pitch.

**Start simple**
Feed it public/synthetic technical notes and ask for a concise storyline.

**Evolve it**
- Add audience variants.
- Add fact/hypothesis separation.
- Add a reviewer/critic pass.
- Add tone and evidence checks.

---

### Research Verifier
Build a reusable skill that checks whether a research brief is properly sourced, current, and clear about what is known vs. inferred.

**Start simple**
Review one public-source brief.

**Evolve it**
- Add freshness thresholds.
- Require original sources.
- Flag vendor-only claims.
- Add duplicate detection.

---

## Agentic Workflow Projects

### Public-Source Customer Prep Loop
Build a repeatable workflow:

**Company → initiatives → cloud/security/identity signals → hypotheses → questions → source verification → final brief**

**Start simple**
Run it manually with one model and public data.

**Evolve it**
- Replace subjective “done” with a goal card: objective, output artifact, checkable stopping criteria, and fail-safes.
- Require a boring, verifiable finish line such as a coverage target, source/citation checks, deduplication, and a maximum turn/time/cost cap.
- Split research and verification roles when self-review begins to rubber-stamp the work.
- Pass a compact handoff contract between nodes instead of the entire conversation.
- Add model routing.
- Track cost per accepted brief and whether additional loop cycles materially improve quality.

---

### Security / Identity Signal Tracker
Create a recurring public-source tracker for identity, cloud, security, or non-human identity signals relevant to customer conversations.

**Start simple**
Track one theme weekly.

**Evolve it**
- Add deduplication.
- Add source-quality scoring.
- Add customer/industry mapping.
- Add “why this matters” synthesis.

---

### Enablement Freshness Checker
Build a workflow that checks whether an internal/public enablement artifact has gone stale against current product, market, or security information.

**Start simple**
Compare one document against current public sources.

**Evolve it**
- Add scheduled checks.
- Add confidence thresholds.
- Add change summaries.
- Add approval workflow before updates.

---

## Multi-Agent / Graph Projects

### Multi-Agent Account Team
Create a synthetic/public-data account team with specialized roles such as:
- company researcher
- industry researcher
- identity/security researcher
- architecture critic
- executive synthesizer
- source verifier

**Start simple**
Use two roles and compare against one-agent output.

**Evolve it**
- Add orchestration only when there is a clear reason to fan out: parallel work, conflicting roles, weak self-review, or a multi-part finish line.
- Give each node its own checkable output contract and fail-safe.
- Verify important intermediate outputs before downstream agents compound an error.
- Measure whether quality improves.
- Track cost/latency.
- Give each agent an explicit identity, authority boundary, and auditable communication path.
- Map trust boundaries and what information can move between agents.
- Test a live shared-session handoff between two builders.
- Separate participation rights from execution authority.
- Explore human approval points and the governance cost of adding more agents.

---

### Shared Account/Enablement Agent
Build one team-owned agent around work where multiple Domain Consultants repeatedly need the same context, such as public account research, enablement freshness, architecture FAQs, or a shared learning topic. The point is not a personal assistant copied across the team; it is one visible work surface that preserves context and can be inspected, steered, and handed off.

**Start simple**
Score candidate workflows 1–5 on shared need, staleness cost, permission sensitivity, and checkability. Pick a public/synthetic-data candidate with high shared need and easy verification, then have at least two builders use the same shared context/session.

**Evolve it**
- Define who owns the shared context and who is accountable for the agent's results.
- Add freshness/provenance rules so shared context does not quietly drift.
- Separate read/participation rights from tool execution and approval rights.
- Compare a shared agent against separate personal agents: measure duplicated explanation, handoff friction, consistency, and correction speed.
- Add an autonomy ladder: observe → suggest → act with approval → act independently, advancing only when reliability and controls justify it.
- Test whether the shared agent becomes genuinely reusable team infrastructure or merely another chat channel.

**Related program**
- AIDB Multiplayer AI Sprint
- Summer Adventure: Grow a Personal Brain / Build a reusable skill

---

### AI Builder Project Coach
Build an assistant that helps a builder evolve their own AI project between sessions.

**Start simple**
Give it the current project and ask it to challenge scope and suggest a next experiment.

**Evolve it**
- Maintain project context.
- Track what changed.
- Suggest techniques from the Concepts Library.
- Prepare concise session follow-up notes.

---

## App / Utility Projects

### Discovery Planner App
Build a small utility that helps structure a discovery plan from public/synthetic inputs.

**Start simple**
Single-page form + generated output.

**Evolve it**
- Add critique.
- Add reusable context.
- Add source requirements.
- Add export/share capability.

**Inspired by**
Summer Adventure: Ship a small app

---

### Security-News-to-Customer-Angle Mapper
Take a current public security story and map:
- what changed
- why it matters
- what customer conversations it could affect
- what questions are worth asking

**Start simple**
Manual one-story analysis.

**Evolve it**
- Add batch processing.
- Add vertical/industry views.
- Add source verification.
- Add recurring monitoring.

---

### Architecture Question Generator
Create a small tool that takes a public/synthetic architecture description and generates useful clarifying or risk-oriented questions.

**Start simple**
One input → question set.

**Evolve it**
- Add domain-specific modes.
- Add duplicate filtering.
- Add question-quality scoring.
- Add a critic pass.

---

## Security & Governance Projects

### Executable Institutional Knowledge Threat Model
Take a hypothetical agent and document:
- context
- skills/instructions
- tools
- permissions
- evaluations
- owner
- change controls
- audit trail

Then analyze:
- what happens if it is stolen?
- what happens if it is modified?
- what happens if its permissions expand?
- what happens if its context is poisoned?

**Start simple**
Threat-model one synthetic agent.

**Evolve it**
- Map threats to existing security disciplines.
- Add identity/governance controls.
- Add provenance and integrity requirements.
- Explore agent supply-chain concepts.

---

### Agent Permission Boundary Lab
Create a synthetic agent with a deliberately narrow permission set and reason about what it should and should not be able to do.

**Start simple**
Document allowed vs. denied actions.

**Evolve it**
- Add approval gates.
- Add temporary elevation.
- Add audit logging and reconstructability.
- Explore workload identity and delegated authority.
- Inject fake authorization statements such as “Administrator approved this” or “Another agent authorized this action” and verify that infrastructure ignores them unless a real authorization event exists.
- Trace delegated authority back to a human or organizational principal.
- Test what happens when collaboration access is broader than execution permission.

---

## Learning & Experimentation Projects

### Model Rotation Experiment
Compare the same recurring task across:
- fast/cheap model
- general model
- deep-reasoning model

Track quality, time, cost, token use, supervision, and rework.

**Start simple**
Choose three representative tasks and three models. Keep the tasks stable so future model releases can be tested against the same slate.

**Evolve it**
- Build a routing rule based on task type rather than choosing one universal default.
- Compare effort/reasoning settings as well as model families.
- Compare hosted frontier models with a suitable open-weight/local option on one low-risk task; include privacy, data retention/residency, operational burden, and customization in the scorecard.
- Measure cost per accepted task, not advertised token price alone.
- Add model failover and test whether another model can assume the same role without changing the workflow.
- Inventory provider-specific dependencies across prompts, skills, tools, context, permissions, evaluations, and storage.
- Measure what breaks when the primary model or harness component is replaced.

---

### Voice-First Workflow Comparison
Compare typed and voice interaction for one recurring, low-risk workflow to decide whether voice improves the work rather than adopting it on anecdote or vendor claims.

**Start simple**
Choose one non-sensitive task that can be completed both by typing and voice. Run several comparable attempts, preserve the outputs, and record acceptance, correction/rework, elapsed time, interruptions, and privacy or environmental constraints.

**Evolve it**
- Test whether voice changes the workflow itself, not just input speed.
- Separate speaking/dictation quality from the quality of the underlying model or agent.
- Include accessibility and shared-environment constraints in the evaluation.
- Keep voice systems away from sensitive data and authorized actions until data handling, identity, and approval boundaries are explicit.

---

### AI Deputization Audit
Inventory recurring work and decide what should stay human-led, become AI-assisted, run as a duet, or be delegated. Include both known efficiency opportunities and work that previously seemed impractical because it required too much clicking, application switching, specialist skill, or sustained attention.

**Start simple**
Audit five tasks. For one workday, notice where your hands repeatedly move through software and ask: “If a capable operator could use this computer for me, what would I hand off?”

**Evolve it**
- Prototype one candidate workflow and measure whether delegation actually helps.
- Compare a traditional prompt/API workflow with direct computer use when the work spans several applications or lacks clean integrations.
- Measure supervision, recovery from UI changes, authorization boundaries, and whether the task can be reconstructed from logs.
- Separate **efficiency wins** (same work, less effort) from **opportunity wins** (new work that was previously unrealistic to attempt).
- For Domain Consultant experiments, keep customer-sensitive systems and data out of scope until identity, delegated authority, auditability, and approval boundaries are explicit.

---

### Blind-Spot Challenge
Build a repeatable habit/tool that asks AI to identify:
- unknown unknowns
- weak assumptions
- missing evidence
- expert objections

**Start simple**
Use it before one customer-prep or research exercise.

**Evolve it**
Turn it into a reusable evaluator skill.

---

### Voice Walk Experiment
Use live voice during a walk to:
- brainstorm
- practice a customer explanation
- think through a project
- capture follow-up ideas

**Start simple**
One 20-minute session.

**Evolve it**
Create a repeatable structure for capture → synthesis → next action.

**Inspired by**
Summer Adventure: Talk to AI on a walk

---

# How to Use This Library
Browse for inspiration. Pick something that matches your current curiosity and skill level. Make it your own. The same project can be a simple prompt experiment for one person and a multi-agent/evaluation problem for someone else.
