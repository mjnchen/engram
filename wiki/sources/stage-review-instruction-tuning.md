---
title: A Stage Review of Instruction Tuning (Yao Fu)
url: https://yaofu.notion.site/June-2023-A-Stage-Review-of-Instruction-Tuning-f59dbfc36e2d4e12a33443bd6b2012c2
tags: [llm, instruction-tuning, overview]
created: 2026-05-14
---

# A Stage Review of Instruction Tuning (Yao Fu)

## Summary

Mid-2023 review of the instruction-tuning landscape capturing the moment when open-source alternatives to InstructGPT had proliferated but still lagged in capability. The key tension identified: scaling instruction data breadth vs. depth, and whether synthetic data from stronger models can substitute for human annotation.

## Key Points

- FLAN (multi-task NLP instruction tuning) and InstructGPT (RLHF on open-ended conversations) represent two distinct instruction-tuning paradigms with different strengths
- Open alternatives (Alpaca, Vicuna) achieved surface-level instruction following cheaply but failed on complex reasoning tasks
- Data quality beats data quantity: 1,000 diverse, high-quality examples often outperform 100,000 lower-quality ones
- By mid-2023 the field was shifting toward using GPT-4 as the annotation source, raising questions about capability ceilings

## Concepts

- [[instruction-tuning]]
- [[rlhf]]
- [[dpo]]
- [[foundation-models]]

## Notes
