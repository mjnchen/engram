---
title: Retrieval-Augmented Generation (RAG)
tags: [llm, inference, knowledge]
created: 2026-05-14
source: https://lilianweng.github.io/posts/2023-06-23-agent/
---

# Retrieval-Augmented Generation (RAG)

## Summary

RAG augments a language model's generation by first retrieving relevant documents from an external knowledge store and including them in the context. You use it to ground LLM outputs in up-to-date or domain-specific information without retraining, reducing hallucinations on knowledge-intensive tasks. The retriever finds relevant chunks; the generator conditions on both the query and retrieved text.

## Key Ideas

- Retrieval typically uses dense embeddings (FAISS, vector DBs) or sparse BM25, or a combination (hybrid search)
- Retrieved chunks are inserted into the prompt context window before generation; the model attends to them directly
- Enables using knowledge that postdates training or is too voluminous to memorize in weights
- Key failure modes: retrieval misses relevant docs, retrieved docs are noisy/contradictory, context window overflow
- Advanced patterns: re-ranking retrieved results, iterative/multi-hop retrieval, RAG-Fusion (querying multiple reformulations)

## Related

- [[llm-hallucination]]
- [[llm-agents]]
- [[prompt-engineering]]
- [[llamaindex]]
- [[langchain]]
- [[autorag]]
- [[ragas]]
