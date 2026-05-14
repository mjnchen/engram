---
title: TRL (Transformer Reinforcement Learning)
url: https://huggingface.co/docs/trl/en/index
maker: Hugging Face
tags: [llm, training, alignment]
created: 2026-05-14
---

# TRL (Transformer Reinforcement Learning)

## What it is

TRL is a full-stack library by Hugging Face for training LLMs with RLHF, DPO, PPO, and other alignment and post-training methods.

## What problem it solves

Aligning LLMs with human preferences requires specialized training loops (reward modeling, PPO updates, preference optimization) that are complex to implement; TRL provides tested, production-ready implementations of these algorithms.

## Concepts

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]
- [[instruction-tuning]]

## Notes

Integrates with the full Hugging Face ecosystem (transformers, PEFT, datasets). Supports SFT, reward modeling, PPO, DPO, and ORPO trainers. Apache 2.0 license.
