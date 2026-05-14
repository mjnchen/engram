---
title: Mistral 7B
url: https://mistral.ai/news/announcing-mistral-7b/
maker: Mistral AI
tags: [llm, model, open-weight]
created: 2026-05-14
---

# Mistral 7B

## What it is

Efficient 7B parameter open-weight model from Mistral AI using sliding window attention and grouped-query attention to outperform Llama 2 13B on most benchmarks.

## What problem it solves

Prior 7B models lagged larger models significantly; Mistral 7B showed that architectural improvements (GQA, SWA) could close much of that gap at the same parameter count.

## Concepts

- [[flash-attention]]
- [[foundation-models]]
- [[transformer]]

## Notes

- Apache 2.0 licensed
- Sliding window attention (SWA) with window size 4096 and rolling buffer cache
- Grouped-query attention (GQA) for faster inference
