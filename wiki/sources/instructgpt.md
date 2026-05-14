---
title: InstructGPT Paper
url: https://arxiv.org/pdf/2203.02155.pdf
tags: [llm, alignment, training]
created: 2026-05-14
---

# InstructGPT Paper

## Summary

OpenAI's paper introducing RLHF as a method for aligning GPT-3 to follow instructions and be more helpful. The key empirical finding: a 1.3B InstructGPT model was preferred over the 175B GPT-3 base model in human evaluations, demonstrating that alignment training is more sample-efficient than scaling for helpfulness.

## Key Points

- Three-stage pipeline: supervised fine-tuning on demonstrations, reward model training on preference pairs, then PPO optimization against the reward model
- Human raters preferred InstructGPT outputs 85% of the time over GPT-3 despite being 100x smaller
- InstructGPT is more truthful (less likely to fabricate) and less toxic — but still makes factual errors
- KL divergence penalty in the RL objective prevents the policy from straying too far from the SFT model (prevents reward hacking)

## Concepts

- [[rlhf]]
- [[llm-alignment]]
- [[instruction-tuning]]
- [[dpo]]

## Notes
