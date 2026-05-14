---
title: Megatron-LM
url: https://github.com/NVIDIA/Megatron-LM
maker: NVIDIA
tags: [llm, training, infrastructure]
created: 2026-05-14
---

# Megatron-LM

## What it is

Megatron-LM is a research framework by NVIDIA for training large Transformer models using tensor parallelism, pipeline parallelism, and data parallelism in combination.

## What problem it solves

Training frontier-scale language models requires splitting model layers across hundreds of GPUs efficiently; Megatron-LM implements the parallelism strategies and kernel optimizations needed to do this at scale.

## Concepts

- [[tensor-parallelism]]
- [[transformer]]
- [[foundation-models]]
- [[flash-attention]]

## Notes

Used to train the original Megatron-LM models and serves as the backbone for many production training stacks (e.g., Falcon, BLOOM). Apache 2.0 license.
