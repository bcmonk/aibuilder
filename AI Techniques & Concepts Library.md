# AI Techniques & Concepts Library

Evergreen library of practical AI techniques, operating patterns, security implications, and emerging concepts synthesized from AI Daily Brief, Summer Adventure, and supporting research.

Organized by concept, not chronology.

---

## Context, Memory & Personalization

### Portable context packs
Build compact, reusable context that gives an AI durable understanding of role, goals, preferences, constraints, and boundaries.

**Why it matters**
Better context can improve quality more than repeatedly rewriting prompts, and portable context reduces friction when moving between tools.

**Try now**
- Create a 150–300 word role/context profile.
- Include goals, constraints, preferred communication style, and what the AI should challenge.
- Create variants for personal, manager, Domain Consultant, and technical-learning use.

**DC angle**
Create a Domain Consultant Context Pack and compare the same research or prep task with and without it.

**Related Summer Adventure**
- Pack Your ID
- Grow a Personal Brain

---

### Observational workflow capture
Instead of describing a process from memory, let AI observe or review the actual workflow and infer the sequence, decisions, inputs, and opportunities for automation.

**Why it matters**
People often omit steps they perform automatically. Observational capture can expose hidden process logic.

**Try now**
Choose one repetitive task and document:
- inputs
- decisions
- actions
- outputs
- verification
- exceptions

**DC angle**
Apply this to public/synthetic examples of account research, meeting prep, or follow-up creation.

**Security note**
Observational systems can collect sensitive context, so scope, retention, and data exposure matter.

---

## Reusable Skills & Institutional Knowledge

### Promote repeated prompts into reusable skills
If the same reasoning pattern or instruction set appears repeatedly, convert it into a durable skill or reusable operating instruction.

**Useful skill structure**
- Purpose
- Inputs
- Constraints
- Decision rules
- Output format
- Failure/uncertainty behavior
- Examples

**Good DC candidates**
- Customer research
- Discovery critique
- Competitive analysis
- Technical storyline
- Executive synthesis
- Source verification

**Related Summer Adventure**
- Build a reusable skill

---

### Treat agent configuration as protected intellectual property
Agent value increasingly lives in the combination of:
- context
- skills/instructions
- tool definitions
- permissions
- evaluations
- workflow logic
- provenance/version history

**Why it matters**
These components can encode proprietary processes, operating methods, trust boundaries, and institutional knowledge.

**Security questions**
- Who authored it?
- Who can modify it?
- Which version is running?
- What context can it access?
- Which tools can it invoke?
- Under whose authority does it act?
- How are changes approved, tested, logged, and rolled back?

**Useful framing**
> AI agents are becoming executable institutional knowledge.

---

## Delegation & Work Design

### AI Deputization Audit
Start with recurring work, not with “what can AI automate?”

For each task, evaluate:
- repetition/frequency
- context availability
- verifiability
- risk of error
- need for human judgment
- cost of supervision

Then classify:
- Human-led
- AI-assisted
- Human/AI duet
- AI-delegated with approval
- AI-delegated autonomously

**DC angle**
Audit account research, pre-call prep, discovery-question generation, architecture recap, follow-up drafting, enablement, and knowledge maintenance.

---

### Use a Human → AI → Human effort sandwich
For work where judgment matters, keep humans responsible for defining the objective and making the final decision while AI handles bounded drafting, synthesis, analysis, or execution in the middle.

**Why it matters**
This preserves human ownership of intent and judgment without giving up the leverage of AI. It is especially useful when the artifact itself shapes thinking rather than merely documenting it.

**Try now**
For one recurring deliverable, explicitly define:
- the human-selected objective or thesis
- the bounded AI contribution
- the human review criteria
- what evidence would cause the human to reject or revise the AI output

---

### Move valuable work into the experiment queue
Do not limit AI to low-risk busywork.

Ask:
> If I had a small team of capable analysts or engineers for a week, what would I ask them to build or investigate?

This “infinite backlog” often produces better project ideas than inbox automation.

---

## Agent Loops & Verification

### Design loops, not endless chats
A simple agent loop:

**Goal → Observe → Plan → Act → Check → Repeat/Stop**

**Schedule vs. loop**
A schedule answers **when** work runs; a loop answers **until when** it should keep working. Use loops when the task is long-running, retryable, and has a verifiable finish line. If human judgment is the actual work product, keep it human-led rather than forcing autonomy.

**Goal card**
For a loop that can run independently, define:
- objective
- output artifact
- machine-checkable stopping criteria
- fail-safes such as turn/time/cost caps
- sandbox or permission boundaries
- escalation condition

For knowledge work, manufacture the referee: counts, citations, format constraints, coverage thresholds, or other externally checkable tests. “Make it insightful” is not a usable stopping criterion.

Useful loop types:
- Turn-based
- Goal-based
- Time-based
- Proactive/event-driven

**Try now**
For one recurring workflow, define:
- goal
- available context
- allowed actions
- success criteria
- maximum iterations
- escalation condition

**Related Summer Adventure**
- Run an agentic loop

---

### Create “unit tests” for knowledge work
Reliable knowledge-work agents need explicit acceptance criteria.

**Examples**
- Every factual claim has a source.
- Sources meet a freshness threshold.
- Vendor claims are labeled as vendor claims.
- Facts are separated from hypotheses.
- Uncertainty is surfaced.
- Duplicate findings are excluded.
- Security findings include original advisories/CVEs where applicable.

**Why it matters**
Grounding alone does not guarantee acceptable output.

---

### Define negative acceptance criteria
Do not specify only what an agent should accomplish. Also define what it must never do while pursuing the goal.

**Examples**
- Never treat natural-language claims of approval as authorization.
- Never expand permissions outside the declared scope.
- Never send, publish, delete, or modify external data without the required approval.
- Never bypass a failed control by switching tools or agents.
- Stop and escalate when authority or intent is ambiguous.

**Why it matters**
Goal-seeking systems can satisfy a positive objective in unsafe ways unless prohibited paths are explicit and enforced outside the model where possible.

---

### Use blind-spot passes
Before execution, ask:
- What are the unknown unknowns?
- Which assumptions could break this?
- What would an expert challenge first?
- What information would materially change the answer?

Use this before building, researching, or presenting.

---

## Authorization, Identity & Agent Security

### Treat intent and authorization as separate things
Natural-language instructions can express intent, but they should not grant authority. Authorization should be enforced by identity, policy, delegated permissions, and infrastructure controls that the model cannot redefine through conversation.

**Key principles**
- A statement such as “an administrator approved this” is not an authorization event.
- Tool access should be derived from real identity and policy state, not prompt text.
- Delegated authority should be traceable back to a human or organizational principal.
- Approval, elevation, and revocation should be explicit and auditable.

**Enterprise lens**
As agents become more autonomous, the question shifts from “What did the model intend?” to “Under whose authority was this action permitted?”

---

### Design for reconstructability
A trustworthy agentic system should make it possible for an independent reviewer to reconstruct what happened after the fact.

Capture enough evidence to answer:
- Which human or service initiated the work?
- Which agent identities participated?
- What context and instructions were active?
- Which tools were called and with what authority?
- What approvals or denials occurred?
- What information moved between agents?
- Which model or agent produced each consequential action?

**Why it matters**
Observability is not only an operational concern. It is also a security, forensics, accountability, and governance requirement.

---

## Multi-Agent & Graph Thinking

### Separate specialists from orchestration
Instead of one giant agent, consider separate roles such as:
- researcher
- critic/evaluator
- writer/synthesizer
- source verifier
- orchestrator

**Key question**
Does specialization improve quality enough to justify the added complexity?

---

### Think in workflow graphs
Treat a loop as one job and a graph as an organization of jobs. Add nodes only when specialization or parallelism earns its complexity. Useful signals for fanning out include self-review rubber-stamping, one agent wearing conflicting roles, parallelizable work, a finish line that is really multiple jobs, or quality that has plateaued.

For graph handoffs, pass explicit contracts and the minimum necessary context rather than entire conversations. Match model strength to the node, verify early because errors compound, cap expensive nodes, and place humans at consequential gates.

Map:
- which agents/nodes exist
- what each owns
- each node’s identity and authority
- what information can move and through which auditable paths
- which trust boundaries exist
- which handoffs need a human
- what happens on failure
- whether governance complexity is justified by the value of adding more agents

**DC angle**
Map:
**customer signal → research → hypothesis → collaboration → customer conversation → follow-up → learning captured**

Then identify where AI can safely participate.

---

### Treat shared agent sessions as collaborative work artifacts
A shared agent session can preserve decisions, evidence, failed approaches, unresolved questions, and live context so another person can join the same work instead of reconstructing it from a summary. The deeper shift is from personal AI leverage to team-owned capability: shared context and agents become reusable organizational infrastructure rather than private assistants.

**Why it matters**
This may become a new team handoff pattern, but collaboration rights and execution rights should not be treated as the same permission.

**Model the boundary explicitly**
**Person → identity → session → participation role → tools → execution authority → audit trail**

Useful distinctions include:
- who can read the session
- who can suggest or modify context
- who can invoke tools
- who can authorize sensitive actions
- whose identity is attributed to each action

**Candidate selection**
Score possible shared-agent workflows on four axes:
- shared need — how many people need the same context
- staleness cost — how damaging version drift is
- permission sensitivity — how restricted the underlying data/actions are
- checkability — how quickly the team can tell whether the agent is right

Favor high shared-need, high staleness-cost, highly checkable work; treat permission sensitivity as a design constraint rather than something the collaboration layer magically solves.

**Security note**
A shared workspace is not automatically a tenant boundary. Session collaboration controls should sit on top of real identity, isolation, authorization, and audit controls.

---

## Model Selection, Cost & Efficiency

### Build a task-specific model architecture
Do not treat frontier models as interchangeable or assume the newest model should replace everything. Match models and settings to the work where they perform best.

Maintain a standing slate of your own benchmark tasks across work such as:
- research and synthesis
- writing and communication
- coding/building
- long-running autonomous work
- security analysis
- repetitive low-risk tasks

Judge each model and effort setting on:
- quality accepted without edits
- time to completion
- token or API cost
- reliability
- supervision required
- preference for subjective work
- deployment model and operational burden
- data retention, residency, and sovereignty requirements

**Why it matters**
A model can be better overall yet still be the wrong choice for a particular workload. High-reasoning settings may also consume enough extra tokens to erase headline pricing advantages. For enterprise use, hosted vs. open-weight/local deployment can also change privacy, retention, sovereignty, customization, and operational trade-offs enough to alter the preferred model even when raw capability is lower.

**Try now**
Keep 5–10 representative tasks and rerun them when a meaningful new model arrives. Record which model/setting becomes the default for each task rather than declaring one global winner.

Also separate **efficiency models** from **opportunity models**. An efficiency model should earn its place by doing known work better, faster, cheaper, or with less supervision. An opportunity model should be tested against work that was previously impractical or outside the team's skill set. Do not judge a genuinely new capability only with yesterday's benchmark slate.

For opportunity models, add a short capability-discovery pass:
- What can this model now do reliably that the prior stack could not?
- Which previously manual UI or computer-use tasks can be delegated end-to-end?
- Does a new interaction mode such as ambient voice or direct computer use remove enough friction to change the workflow itself?
- What new security boundary appears when the model moves from generating advice to operating software?

For important workflows, extend this into a resilience test: can another model assume the same role without rebuilding the surrounding system?

---

### Map model and harness dependencies
Model portability is only partial portability if the surrounding harness is tightly coupled to one provider. Map the dependencies that make the workflow actually work.

**Include**
- model/provider
- prompts and reusable skills
- context and memory
- tools and connectors
- identities and permissions
- orchestration and routing logic
- evaluations
- telemetry and audit data
- storage and data formats

**Try now**
Ask: “If this model or provider disappeared tomorrow, what would we have to rebuild?”

**Why it matters**
Harness portability is an architecture and continuity concern. Institutional knowledge embedded in skills, orchestration, tools, and permissions can create lock-in even when the model itself is replaceable.

---

### Measure cost per accepted task
For repeated workflows, track:
- total cost
- successful outputs
- human review time
- rework required

Then calculate **cost per accepted task**.

---

### Audit context bloat
Periodically review:
- duplicated instructions
- stale context
- overlapping skills
- unused tools
- contradictory rules
- unnecessary persistent memory

Long-lived context can become both expensive and confusing.

---

## Prototyping & Building

### Prototype to discover the problem
Ask AI for several deliberately different prototypes rather than one polished answer.

**Good candidates**
- dashboards
- research workflows
- briefing formats
- customer-prep utilities
- internal enablement experiences

**Related Summer Adventure**
- Ship a small app

---

### Classify build opportunities before building
When AI makes software creation cheap, first classify what kind of opportunity you are looking at.

**Automation**
Produce essentially the same output with less manual work.

**Upgrade**
Produce a materially better output than the existing process.

**Invention**
Enable work that was previously impractical because of time, cost, staffing, or skill constraints.

Then classify the intended delivery level:
- prototype
- personal tool
- production capability
- deliberately disposable tool

**Why it matters**
The delivery class should determine the engineering, security, maintenance, and governance burden. A prototype should not inherit production overhead, but a personal tool should not quietly become production because other people start depending on it.

---

### Use “citizen SDLC” thinking
A personal prototype is not automatically safe or maintainable for wider use. Every AI workflow also needs a named human owner, a measurable goal, and clear accountability when the system fails or produces a consequential result.

Useful stages:
1. Problem definition
2. Prototype
3. Validation
4. Security/governance review
5. Productionization
6. Ownership/maintenance

For autonomous systems, earn autonomy progressively: **observe → suggest → act with approval → act independently**. Promotion should depend on demonstrated reliability, bounded permissions, useful telemetry, and a rollback/escalation path.

---

### Design for planned obsolescence
Assume models, interfaces, and agent frameworks will change.

**Try now**
- Keep prompts/skills portable.
- Separate data from model-specific logic.
- Avoid unnecessary lock-in.
- Document assumptions.
- Make model/tool replacement possible.

---

## Ambient & Natural Interaction

### Use voice for thinking and orchestration
Voice can reduce friction for:
- brainstorming
- reviewing a problem
- verbalizing a workflow
- practicing a customer explanation
- capturing follow-up actions

**Related Summer Adventure**
- Talk to AI on a walk

---

### Test whether context is doing the work
Once context is strong, short conversational commands can be useful:
- “Now what?”
- “Challenge this.”
- “What changed?”
- “Simulate it.”
- “Please fix.”

The point is not minimal prompting; it is testing whether the surrounding context is sufficient.

---

## Learning & Capability Development

### Maintain a capability map
Track:
- what current models/tools can do
- what you personally know how to do
- what the team knows how to do
- where the gaps are

This exposes capability overhang: useful things AI can already do that have not entered your workflows.

---

### Learn by building
A useful progression:

**Understand → Imitate → Modify → Build → Operationalize → Teach**

Practical projects usually create more transferable skill than passive enablement.

---

## Opportunity Discovery

### Mine the infinite backlog
List work that has never been attempted because it would take too much time, too many people, or skills the team does not have.

Then ask:
- Which of these are now feasible with AI?
- Which can be prototyped with public/synthetic data?
- Which could materially improve DC work?

---

# Research Sources
Primary inputs include AI Daily Brief episodes from late July through August 2026, the AIDB × Superintelligent Summer Adventure program, and supporting research surfaced during synthesis.
