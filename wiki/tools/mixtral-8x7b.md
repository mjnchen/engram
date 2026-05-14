---
title: Mixtral 8x7B
url: https://mistral.ai/news/mixtral-of-experts/
maker: Mistral AI
tags: [llm, model, open-weight]
created: 2026-05-14
---

# Mixtral 8x7B

## What it is

Sparse mixture-of-experts model from Mistral AI with 8 expert feed-forward layers per block, activating 2 per token, delivering GPT-3.5-level performance at lower inference cost.

## What problem it solves

Dense models must run all parameters for every token; Mixtral's sparse MoE routing activates only a fraction of parameters per forward pass, making strong performance more compute-efficient at inference time.

## Concepts

- [[mixture-of-experts]]
- [[foundation-models]]
- [[transformer]]

## Notes

- 46.7B total parameters; 12.9B active per token
- Apache 2.0 licensed
- Instruction-tuned variant: Mixtral 8x7B Instruct
