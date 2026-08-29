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

## Sources

- [The AI Daily Brief — The Most Useful New AI Features and Tools to Try](https://aidailybrief.ai/e/2026-08-28)
- [Google DeepMind — Gemini 3.5 Audio model card](https://deepmind.google/models/model-cards/gemini-3-5-audio/)
- [Anthropic — Claude gets its own browser in Cowork](https://claude.com/blog/cowork-built-in-browser)
