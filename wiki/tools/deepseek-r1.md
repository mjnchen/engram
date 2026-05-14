---
title: DeepSeek-R1
url: https://github.com/deepseek-ai/DeepSeek-R1
maker: DeepSeek
tags: [llm, reasoning, model]
created: 2026-05-14
---

# DeepSeek-R1

## What it is

Open-weight reasoning model from DeepSeek trained with group relative policy optimization (GRPO) to generate chain-of-thought before answering, matching OpenAI o1-level performance on math and coding benchmarks.

## What problem it solves

State-of-the-art reasoning had been locked behind closed APIs; DeepSeek-R1 provides a fully open-weight model with competitive reasoning capability.

## Concepts

- [[chain-of-thought-prompting]]
- [[rlhf]]
- [[llm-math-reasoning]]
- [[foundation-models]]

## Notes

- Released with MIT license, including weights
- Distilled versions available from 1.5B to 70B; full model is 671B MoE
- Training uses only RL on verifiable rewards (no supervised fine-tuning for reasoning)
