---
title: veRL
url: https://github.com/volcengine/verl
maker: Bytedance / Volcengine
tags: [llm, training, alignment]
created: 2026-05-14
---

# veRL

## What it is

veRL is an efficient reinforcement learning framework for LLM post-training by Bytedance/Volcengine that supports flexible backend swapping between training and inference engines.

## What problem it solves

RL post-training requires running both a training engine and a fast inference engine simultaneously, which most frameworks tightly couple; veRL separates these concerns so you can mix e.g. Megatron for training with vLLM for rollouts.

## Concepts

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]

## Notes

Supports GRPO, PPO, and other RL algorithms. Designed for large-scale multi-GPU setups. Apache 2.0 license.
