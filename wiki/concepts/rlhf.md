---
title: Reinforcement Learning from Human Feedback (RLHF)
tags: [llm, alignment, training]
created: 2026-05-14
source: https://arxiv.org/pdf/2203.02155.pdf
---

# Reinforcement Learning from Human Feedback (RLHF)

## Summary

RLHF is a training procedure that uses human preference judgments to fine-tune a language model toward outputs humans find helpful, harmless, and honest. You train a reward model on ranked human comparisons of model outputs, then optimize the language model against that reward using reinforcement learning (typically PPO). It's the key technique behind InstructGPT and ChatGPT.

## Key Ideas

- Step 1: Supervised fine-tuning on demonstration data to get a reasonable starting policy
- Step 2: Collect human preference pairs (response A vs. B) and train a scalar reward model
- Step 3: Use PPO to optimize the LLM to maximize reward while penalizing KL divergence from the original policy
- KL penalty prevents the model from "reward hacking" — producing outputs that exploit the reward model without being genuinely better
- Reward models can be noisy; the distribution shift between training and inference is a known failure mode
- [[dpo]] eliminates the explicit reward model and RL loop, simplifying the pipeline

## Related

- [[dpo]]
- [[instruction-tuning]]
- [[llm-alignment]]
- [[trl]]
- [[openrlhf]]
