# AI Builder Project Library

An evergreen collection of optional project and sandbox ideas for AI Builders. Projects should be practical, support different experience levels, and evolve from simple experiments toward advanced concepts when useful.

## Project Ideas

### Browser Agent Trust-Boundary Lab

Compare how the same low-risk workflow behaves in an isolated agent browser versus a browser using an authenticated profile.

**Start simple:** Ask each environment to collect public information and prepare—but not submit—a form. Record every site, permission request, and proposed action.

**Build further:** Add a mock authenticated application with read-only and editor roles. Test whether the agent respects role boundaries, confirmation gates, destination allowlists, and instructions embedded in an untrusted webpage.

**Advanced extension:** Issue a short-lived task credential to a named agent identity. Capture the human requester, agent version, credential, tool calls, approvals, and outcome in an audit record. Add detection for unusual navigation or attempted privilege expansion.

**Domain Consultant angle:** Use the lab to discuss where identity, authorization, browser isolation, non-human identity management, and runtime monitoring belong in customer agent architectures.

### Verbatim-to-Intent Voice Pipeline

Build a voice-note or meeting-capture workflow that produces both a faithful record and a useful, cleaned interpretation.

**Start simple:** Transcribe a short voice note twice—verbatim and cleaned—and highlight every semantic change.

**Build further:** Create an evaluation set containing names, acronyms, product terminology, numbers, negation, self-correction, decisions, and action items. Score factual preservation separately from readability.

**Advanced extension:** Add speaker separation, timestamps linking summaries to evidence, sensitive-data handling, retention controls, and a human approval step before commitments become tasks or records.

**Domain Consultant angle:** Explore how an intent-aware capture layer could improve discovery notes, handoffs, enablement content, or incident timelines without allowing polished summaries to replace authoritative evidence.

### Model-Agnostic Harness Drill

Build a small harness that swaps its underlying model provider without touching application logic, then simulate a vendor cutting off access to see what actually breaks.

**Start simple:** Wire a single skill or workflow (a summarizer, a classifier, a simple agent loop) behind a thin abstraction layer — one function or config value that selects the model provider — using at least two providers (for example, an Anthropic model and an open-weights model via a router). Confirm the same task runs unmodified against both.

**Build further:** Simulate a cutoff: revoke or expire the credential for one provider mid-project and measure how long it takes to fail over to the other, what breaks (prompts tuned to one model's quirks, tool-call formats, context limits), and what doesn't (governance, logging, approval gates — if the harness is built right, these live above the model layer and survive the swap).

**Advanced extension:** Add automated failover with a defined policy (which fallback model, under what conditions, who's notified), inventory every credential, API key, and non-human identity tied to each provider, and produce a one-page vendor-dependency map — what would actually happen if this specific model access were pulled tomorrow.

**Domain Consultant angle:** A direct, tangible way to walk a customer through vendor-risk and non-human-identity conversations — most enterprises building on a single model API have never tested what happens when that access disappears, and 2026's lab conflicts (OpenAI/Cursor, Anthropic/Windsurf) make it a live, not hypothetical, risk.

## Sources

- [The AI Daily Brief — The Most Useful New AI Features and Tools to Try](https://aidailybrief.ai/e/2026-08-28)
- [Google DeepMind — Gemini 3.5 Audio model card](https://deepmind.google/models/model-cards/gemini-3-5-audio/)
- [Anthropic — Claude gets its own browser in Cowork](https://claude.com/blog/cowork-built-in-browser)
- [The AI Daily Brief — How to Navigate the Next Wave of AI Competition](https://aidailybrief.ai/e/2026-08-31)
