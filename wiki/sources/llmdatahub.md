---
title: LLMDataHub
url: https://github.com/Zjh-819/LLMDataHub
tags: [llm, data, training]
created: 2026-05-14
---

# LLMDataHub

## Summary

Curated index of datasets for each stage of LLM training: pre-training corpora, instruction-tuning datasets, and RLHF preference data. Useful for understanding what data goes into each training phase and locating specific datasets by license, language, and domain.

## Key Points

- Pre-training data is dominated by web crawls (Common Crawl derivatives) — quality filtering matters more than raw size
- Instruction datasets range from human-annotated (FLAN, Dolly) to synthetic (Alpaca, Open-Orca) — synthetic data scales more cheaply but can introduce artifacts
- RLHF preference datasets (Anthropic HH, OpenAssistant) are small relative to pre-training data but high-signal
- Dataset contamination (test sets appearing in training data) inflates benchmark scores and is difficult to audit retroactively

## Concepts

- [[instruction-tuning]]
- [[rlhf]]
- [[foundation-models]]
- [[bpe-tokenization]]

## Notes
