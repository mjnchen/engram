---
title: LM Reasoning Papers
url: https://github.com/atfortes/LM-Reasoning-Papers
tags: [llm, reasoning, survey]
created: 2026-05-14
---

# LM Reasoning Papers

## Summary

Broader survey of reasoning in language models, covering arithmetic, commonsense, symbolic, and causal reasoning benchmarks. Distinguishes between prompting-based reasoning improvements and training-based approaches, showing the two are complementary rather than competing.

## Key Points

- Arithmetic reasoning (GSM8K, MATH) and commonsense reasoning (HellaSwag, WinoGrande) require different interventions
- Process reward models (rewarding correct steps) outperform outcome reward models on math tasks
- Scratchpad and chain-of-thought increase compute at inference time, which trades off against latency
- Fine-tuning on reasoning traces can distill chain-of-thought ability into smaller models

## Concepts

- [[chain-of-thought-prompting]]
- [[tree-of-thoughts]]
- [[llm-math-reasoning]]
- [[rlhf]]

## Notes
