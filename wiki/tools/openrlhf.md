---
title: OpenRLHF
url: https://github.com/OpenRLHF/OpenRLHF
maker: OpenRLHF
tags: [llm, training, alignment]
created: 2026-05-14
---

# OpenRLHF

## What it is

OpenRLHF is a scalable RLHF training framework built on Ray that supports large-scale PPO and DPO training across many GPUs.

## What problem it solves

RLHF at scale requires coordinating actor, critic, reward, and reference models simultaneously, which is difficult to schedule efficiently; OpenRLHF uses Ray to distribute these roles across separate GPU groups.

## Concepts

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]

## Notes

Supports 70B+ model training with vLLM-accelerated generation. Apache 2.0 license.
