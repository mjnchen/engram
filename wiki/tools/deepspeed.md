---
title: DeepSpeed
url: https://github.com/microsoft/DeepSpeed
maker: Microsoft
tags: [llm, training, infrastructure]
created: 2026-05-14
---

# DeepSpeed

## What it is

DeepSpeed is a deep learning optimization library by Microsoft that implements ZeRO optimizer stages, pipeline parallelism, and mixed-precision training for training large models efficiently.

## What problem it solves

Training models with billions of parameters exceeds single-GPU memory; DeepSpeed shards optimizer states, gradients, and parameters across GPUs to make large-scale training feasible.

## Concepts

- [[zero-redundancy-optimizer]]
- [[tensor-parallelism]]
- [[foundation-models]]

## Notes

Integrates with Hugging Face Transformers. Supports ZeRO stages 1–3 and ZeRO-Infinity (NVMe offloading). Apache 2.0 license.
