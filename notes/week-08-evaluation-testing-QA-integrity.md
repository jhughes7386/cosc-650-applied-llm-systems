# Week 8: Evaluation, Testing, and QA Integrity

## Readings

- [End-to-End LLM Systems](https://craigtrim.com/articles/end-to-end-systems/) — the framing article for the recap week: how tokenization, inference, prompting, tools, RAG, fine-tuning, and evaluation compose into one system, the three architectural shapes (single agent, hub-and-spoke, flat shared state), and cross-cutting concerns of provenance, observability, cost, and guardrails.

- [Continuous Testing for LLM Systems](https://craigtrim.com/articles/continuous-testing/) — testing non-deterministic outputs through four families (regression, snapshot with diff review, property-based, and metamorphic testing), synchronous versus batch evaluation, context isolation, CI/CD integration, and drift detection.

- [LLM Failure Post-Mortems](https://craigtrim.com/articles/llm-failure-postmortems/) — the methodology for learning from production failures: six failure modes at component boundaries and the six-field postmortem template (Incident, Symptom, Root Cause, Detection Gap, Resolution, Lesson) used for this week's assignment.

- [Tool Use Postmortems](https://craigtrim.com/articles/tool-use-postmortems/) — seven tool-use failure cases and the PocketOS worked example involving a nine-second production database deletion. The readings emphasize that failures often occur at tool boundaries and that model explanations are not always reliable accounts of what happened.

- [The Moltbook Phenomenon](https://craigtrim.com/articles/moltbook-phenomenon/) — a case study on the autonomy spectrum: the gap between headlines describing Level 4 self-directed agents and engineering systems operating at Level 2 (act with confirmation), along with monoculture risk and the indirect prompt-injection attack surface associated with OpenClaw.