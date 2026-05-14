---
title: Why did all public GPT-3 reproductions fail?
url: https://jingfengyang.github.io/gpt
tags: [llm, training, overview]
created: 2026-05-14
---

# Why did all public GPT-3 reproductions fail?

## Summary

Technical post-mortem on why early open-source GPT-3 reproductions (OPT, BLOOM, GPT-NeoX) fell short despite similar parameter counts. The conclusion: data quality, data mixture, and training stability decisions mattered far more than architecture, and OpenAI's data pipeline was not replicable from public sources.

## Key Points

- OPT matched GPT-3 architecture but used different data — quality filtering and domain mixture, not scale, explain the gap
- Training instability at large scale causes loss spikes that require learning rate rollbacks, and each rollback loses progress; small labs can't absorb this cost
- The "you need X tokens for Y parameters" intuition was poorly understood before Chinchilla — most reproductions were severely undertrained
- Data deduplication is critical: models trained on deduplicated data generalize better than those trained on larger raw corpora

## Concepts

- [[scaling-laws]]
- [[chinchilla-scaling-laws]]
- [[foundation-models]]
- [[bpe-tokenization]]

## Notes
