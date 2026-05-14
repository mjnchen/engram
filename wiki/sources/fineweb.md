---
title: FineWeb (HuggingFace)
url: https://arxiv.org/abs/2406.17557
tags: [llm, data, training]
created: 2026-05-14
---

# FineWeb (HuggingFace)

## Summary

Hugging Face paper introducing FineWeb, a 15-trillion-token high-quality web dataset for LLM pre-training built from Common Crawl with rigorous filtering. The paper's ablation study is the most useful part: it quantifies the impact of each filtering decision on downstream benchmark performance.

## Key Points

- URL filtering, language identification, and quality heuristics (like C4-quality filters) each contribute independently to downstream quality
- Deduplication at the document level matters more than deduplication at the URL level — the same content appears on many domains
- FineWeb-Edu (educational content subset) outperforms the full FineWeb on knowledge-intensive benchmarks despite being much smaller
- All data, code, and training logs are released — enabling true reproduction of filtering pipeline decisions

## Concepts

- [[foundation-models]]
- [[scaling-laws]]
- [[chinchilla-scaling-laws]]

## Notes
