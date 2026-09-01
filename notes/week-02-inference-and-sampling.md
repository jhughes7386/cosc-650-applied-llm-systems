# Week 2: Inference and Sampling

## Readings

### 1. Inside the Decoder-Only Transformers

[Inside the Decoder-Only Transformers](https://craigtrim.com/articles/transformer-architecture-review/)

Bridges transformer fundamentals to the LLM-specific engineering perspective. Covers decoder-only architecture, the autoregressive loop, KV-cache mechanics, and why attention scales quadratically. Students who took DSCI-630 will recognize the building blocks; those who did not will find the article self-contained.

### 2. Words Learning the Company They Keep

[Words Learning the Company They Keep](https://craigtrim.com/articles/words-learning-company-they-keep/)

Explains how static embeddings create the centroid problem, where one vector represents all meanings of a word such as "oracle," and how attention resolves this by computing context-dependent representations. Includes four interactive demos showing the disambiguation process.

### 3. From Prompt to Token: How LLM Inference Actually Works

[From Prompt to Token: How LLM Inference Actually Works](https://craigtrim.com/articles/inference-pipeline/)

Covers the complete inference pipeline, including embedding lookup, positional encoding, multi-head attention, feedforward layers, layer normalization, logit computation, softmax, and sampling. Each stage is explained with its engineering implications for cost, latency, and quality.

### 4. The Invisible Boundaries of AI Conversations

[The Invisible Boundaries of AI Conversations](https://craigtrim.com/articles/context-windows-token-limits/)

Explains context window mechanics, the evolution from 512 tokens to millions, truncation strategies, and the engineering tradeoffs behind each approach. Connects back to Week 1 tokenization by showing how the same text can consume different amounts of context depending on how it tokenizes.
