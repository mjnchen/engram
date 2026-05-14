---
title: LLM-RL-Visualized
url: https://github.com/changyeyu/LLM-RL-Visualized
tags: [llm, alignment, visualization]
created: 2026-05-14
---

# LLM-RL-Visualized

## Summary

Visual diagram collection illustrating how RL algorithms (PPO, GRPO, REINFORCE, DPO) are applied in LLM training. Particularly useful for understanding the differences between on-policy and off-policy methods and where each algorithm sits in the RLHF pipeline.

## Key Points

- PPO in RLHF requires four models simultaneously: the actor (policy), critic (value), reward model, and reference model — making it memory-intensive
- GRPO (Group Relative Policy Optimization) eliminates the critic by estimating advantages from a group of sampled responses, halving memory requirements
- DPO collapses reward model + RL into a single supervised objective — simpler but less flexible for online feedback
- Diagrams make the token-level credit assignment problem concrete: each token's reward depends on all subsequent tokens

## Concepts

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]

## Notes
