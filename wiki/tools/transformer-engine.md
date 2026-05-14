---
title: Transformer Engine
url: https://github.com/NVIDIA/TransformerEngine
maker: NVIDIA
tags: [llm, training, efficiency]
created: 2026-05-14
---

# Transformer Engine

## What it is

Transformer Engine is a library by NVIDIA for accelerating Transformer training and inference on Hopper and later GPUs using FP8 mixed-precision arithmetic.

## What problem it solves

FP16/BF16 training leaves performance on the table on H100 GPUs that have dedicated FP8 tensor cores; Transformer Engine automatically selects FP8 vs higher precision per operation to maximize throughput while preserving accuracy.

## Concepts

- [[transformer]]
- [[flash-attention]]

## Notes

Integrates with PyTorch, JAX, and PaddlePaddle. Required by NeMo Framework for FP8 training. Apache 2.0 license.
