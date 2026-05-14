---
title: LMDeploy
url: https://github.com/InternLM/lmdeploy
maker: Shanghai AI Lab
tags: [llm, inference, serving]
created: 2026-05-14
---

# LMDeploy

## What it is

LMDeploy is a high-throughput inference and serving toolkit from Shanghai AI Lab (the team behind InternLM). It includes quantization tooling and a custom TurboMind inference engine.

## What problem it solves

Deploying models from the InternLM family — and other popular architectures — at scale requires both quantization and efficient batching. LMDeploy packages both into a single toolkit with an OpenAI-compatible API.

## Concepts

- [[llm-quantization]]
- [[tensor-parallelism]]
- [[flash-attention]]

## Notes

- Apache 2.0 license; Python/C++
- TurboMind engine is optimized for continuous batching on NVIDIA GPUs
- Supports W4A16 (AWQ) and W8A8 quantization
- Can export quantized models for use with other runtimes
- Primary vehicle for deploying InternLM model series
