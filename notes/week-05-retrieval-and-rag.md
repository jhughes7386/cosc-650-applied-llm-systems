# Week 5: Retrieval and RAG

## What Classic Search Does Before the LLM

[What Classic Search Does Before the LLM](https://craigtrim.com/articles/classic-search/)

The lexical retriever (BM25) still runs underneath most production RAG systems. This reading covers the classic search methods that come before the LLM and provides the foundation for understanding how retrieval works in RAG systems.

## The Simplest Possible RAG

[The Simplest Possible RAG](https://craigtrim.com/articles/simplest-possible-rag/)

The minimum viable RAG system uses BM25 along with a single LLM call. The reading demonstrates how a basic RAG system can be built in about forty lines of Python.

## Vector RAG: Inside the Dense-Vector Retrieval Stack

[Vector RAG: Inside the Dense-Vector Retrieval Stack](https://craigtrim.com/articles/vector-rag/)

This reading covers the dense-vector retrieval path as an integrated stack, including embedding-model selection, vector-database internals such as HNSW, IVF, and product quantization, as well as chunking.

## Measuring Retrieval

[Measuring Retrieval](https://craigtrim.com/articles/measuring-retrieval/)

This reading focuses on measuring retrieval performance through a closed BM25 evaluation loop and the MTEB leaderboard. It also covers how to interpret retrieval measurements without being misled by the results.

## Retrieval Provenance

[Retrieval Provenance](https://craigtrim.com/articles/retrieval-provenance/)

This reading introduces a four-field schema consisting of source, confidence, timestamp, and agent_id. These fields make retrieved chunks into traceable evidence that can be used to understand where information came from.

## The Amortization Assumption

[The Amortization Assumption](https://craigtrim.com/articles/the-amortization-assumption/)

This reading examines situations where the index used by RAG does not provide enough benefit to justify its cost. In these cases, prompt caching and Cache-Augmented Generation can be alternative patterns.
