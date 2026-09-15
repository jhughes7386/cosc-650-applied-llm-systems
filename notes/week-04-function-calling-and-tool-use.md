# Week 4: Function Calling and Tool Use

## Readings

* [From Prompts to Actions](https://craigtrim.com/articles/from-prompts-to-actions/) — the conceptual leap. Why function calling exists, what changes when prompts produce structured calls instead of text, and the JSON schema contract as the new interface. The bridge from Week 3.

* [From Rules to LLMs: Three Architectures](https://craigtrim.com/articles/function-calling-mechanics/) — three system shapes for the same task, walked from a toy classifier through function calling to a production AWS Step Functions workflow. The architectural argument for code-as-orchestrator with the LLM constrained to leaf operations where its strength lives.

* [Token Burn Is Not Productivity](https://craigtrim.com/articles/token-burn-is-not-productivity/) — companion piece to "From Rules to LLMs." Where that article argues for the LLM at leaf operations, this one argues against the inverse: replacing deterministic primitives with runtime LLM calls. The lines-of-code parallel, the empirical productivity case, and a worked toy example of what a function's contract dissolves into when `sorted()` is rewritten as a frontier-model call.

* [Schemas That Models Can Follow](https://craigtrim.com/articles/reliable-tool-schemas/) — schema design for tools the model actually uses correctly. Type constraints, enums, description writing, required vs. optional fields, and error response shapes.

* [Tool Loops: Multi-Step and Parallel Calls](https://craigtrim.com/articles/tool-loops/) — beyond a single call. Sequential chains, parallel calls, retries, when the loop terminates, and how to recover when an intermediate step fails.

* [The Instruction You Didn't Write](https://craigtrim.com/articles/prompt-injection/) — why instruction/data separation is architecturally impossible. Four documented incidents (Microsoft Copilot exfiltration, SpAIware persistent memory, GitHub Copilot RCE, EchoLeak), the lethal-trifecta framework for production defense, and what no major lab has solved.
