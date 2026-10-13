# Week 7: Fine-Tuning, Distillation, and Fairness

## Readings

- [The Adaptation Decision](https://craigtrim.com/articles/adaptation-decision/) — the framing article: when to fine-tune versus the alternatives from Weeks 3-6 (prompting, tools, RAG, memory), with cost, latency, capability, and data-availability tradeoffs and named wrong-choice cases.

- [LoRA Efficiency](https://craigtrim.com/articles/lora-efficiency/) — the mechanics of low-rank adaptation: what the rank parameter controls, choosing target modules, learning-rate behavior, when LoRA suffices versus full fine-tuning, and QLoRA as the four-bit quantized variant.

- [Fine-Tuning Data](https://craigtrim.com/articles/fine-tuning-data/) — the dataset-engineering pipeline: collection, quality filtering, deduplication (exact, MinHash, embedding-based), format consistency, stratified train/eval splitting, and evaluation-set design.

- [Fine-Tuning the Teacher](https://craigtrim.com/articles/fine-tuning-the-teacher/) — how to fine-tune a large model into a good teacher that produces high-fidelity synthetic training pairs: sampling strategy, diversity controls, filtering, and the handoff to distillation.

- [Knowledge Distillation](https://craigtrim.com/articles/knowledge-distillation/) — how a small student learns from a teacher's outputs: the three distillation signals (behavior cloning, logit matching, feature matching), temperature scaling, and when distillation beats fine-tuning on raw data.

- [Bias in Fine-Tuned Models](https://craigtrim.com/articles/bias-in-fine-tuned-models/) — the causal mechanism specific to fine-tuning: how a small skewed training set shifts outputs disproportionately, plus detection methods (base-versus-fine-tuned diffing, counterfactual swaps, demographic-stratified evaluation) and mitigation.

- [Fairness Testing for LLM Systems](https://craigtrim.com/articles/fairness-testing/) — the evaluation methodology: counterfactual testing, stereotype and association benchmarks (WEAT, StereoSet, CrowS-Pairs, BBQ), toxicity measurement, the three formal fairness criteria with the impossibility theorem, and continuous monitoring.