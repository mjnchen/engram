---
title: Direct Preference Optimization (DPO)
tags: [llm, alignment, training]
created: 2026-05-14
source: https://arxiv.org/pdf/2305.18290.pdf
---

# Direct Preference Optimization (DPO)

## Summary

DPO is an alignment algorithm that trains a language model directly on human preference pairs without a separate reward model or reinforcement learning. You reformulate the [[rlhf]] objective to show that the optimal policy is implicitly encoded in the ratio of log-probabilities between the trained model and a reference model. This makes alignment training as simple as running a classification loss on preference data.

## Key Ideas

- The key insight: the reward function can be expressed in closed form using the language model itself, so no separate reward model is needed
- Training loss is a binary cross-entropy on (chosen, rejected) pairs weighted by how much the model diverges from reference on each
- Simpler and more stable than PPO-based RLHF; does not require online sampling during training
- Can underperform RLHF in settings with very noisy or limited preference data, since it has no explicit reward signal to filter noise
- Variants: IPO, KTO, SimPO address different limitations of the original DPO formulation

## Related

- [[rlhf]]
- [[instruction-tuning]]
- [[llm-alignment]]
- [[trl]]
