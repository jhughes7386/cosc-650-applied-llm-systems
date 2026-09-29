# Week 6: Advanced RAG and Knowledge Systems

## Readings

- [Re-ranking: The Second Chance](https://craigtrim.com/articles/reranking-second-chance/) — the two-stage retrieval pattern most production systems converge on: a fast bi-encoder first pass, then a slower cross-encoder reranks the top candidates, plus reciprocal rank fusion across retrievers.

- [GraphRAG: When the Index Is a Graph](https://craigtrim.com/articles/graphrag/) — the structural alternative to vector RAG: an LLM extracts entities and relations into a knowledge graph, and retrieval becomes graph traversal or community-summary aggregation.

- [Ontology-Driven Parsing for Retrieval](https://craigtrim.com/articles/ontology-driven-parsing/) — what makes GraphRAG do real work: a curated ontology commits at ingest to the entities and relations the corpus contains; typed extraction beyond raw NER, at the cost of upfront curation.

- [Structured Data RAG: Routing and Text-to-SQL](https://craigtrim.com/articles/structured-data-rag/) — when the answer lives in a relational database: Text-to-SQL patterns, the sandboxing problem, and the query-router layer that ties vector, graph, and relational backends together.

- [RAGAS Evaluation](https://craigtrim.com/articles/ragas-evaluation/) — the RAGAS framework in depth: faithfulness, answer relevance, context precision, and context recall, with threshold selection, golden datasets, and stratified per-category reporting.

- [LLM-as-Judge](https://craigtrim.com/articles/llm-as-judge/) — using models to evaluate models: rubric design, calibration against human judgment, and why the judge must run in a fresh session to avoid confirmation-biased self-review.

- [Human Evaluation Frameworks](https://craigtrim.com/articles/human-evaluation/) — annotation guidelines, inter-rater reliability, and when human evaluation is irreplaceable: field-level confidence, the reviewer's decision schema, and which escalation triggers prove well-calibrated.