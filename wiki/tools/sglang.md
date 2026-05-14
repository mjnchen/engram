---
title: SGLang
url: https://github.com/sgl-project/sglang
maker: SGLang Project
tags: [llm, inference, serving]
created: 2026-05-14
---

# SGLang

## What it is

SGLang is a fast LLM serving framework with a Python-based structured generation language. It supports constrained decoding (JSON, regex) and is popular for multi-turn and agentic workloads.

## What problem it solves

Structured generation (outputting valid JSON, following schemas) is slow when done naively. SGLang's RadixAttention reuses KV-cache across shared prompt prefixes, cutting latency for programs that call the same model repeatedly with common prefixes.

## Concepts

- [[speculative-decoding]]
- [[flash-attention]]
- [[llm-agents]]

## Notes

- Apache 2.0 license; Python/CUDA
- RadixAttention is the signature feature: a radix tree tracks prefix sharing across requests
- Competitive with vLLM on throughput; often faster for structured generation tasks
- Supports OpenAI-compatible API
