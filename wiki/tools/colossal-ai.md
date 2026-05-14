---
title: Colossal-AI
url: https://github.com/hpcaitech/ColossalAI
maker: HPC-AI Tech
tags: [llm, training, infrastructure]
created: 2026-05-14
---

# Colossal-AI

## What it is

Colossal-AI is a unified training system by HPC-AI Tech with heterogeneous memory management that makes large model training accessible on fewer or cheaper GPUs.

## What problem it solves

Large model training typically requires expensive A100 clusters; Colossal-AI offloads parameters to CPU/NVMe and uses heterogeneous parallelism to lower the hardware bar significantly.

## Concepts

- [[zero-redundancy-optimizer]]
- [[tensor-parallelism]]
- [[foundation-models]]

## Notes

Provides Gemini heterogeneous memory manager. Includes RLHF training pipelines. Apache 2.0 license.
