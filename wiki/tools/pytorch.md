---
title: PyTorch
url: https://pytorch.org/
maker: Meta AI
tags: [pytorch, deep-learning, framework, autograd]
created: 2026-05-15
---

# PyTorch

## What it is

The dominant deep learning framework for research and production. Dynamic computation graphs (eager mode), autograd, and a large ecosystem (torchvision, torchaudio, torchtext). Most LLM research is written in PyTorch.

## What problem it solves

Provides tensor computation with GPU acceleration and automatic differentiation. Replaces manual gradient computation. Flexible enough for research prototypes and production serving (via TorchScript and TorchServe).

## Concepts

- [[transformer]]
- [[flash-attention]]
- [[tensor-parallelism]]

## Notes

- Most open-source LLMs ship PyTorch weights
- `torch.compile` (PyTorch 2.0+) brings significant speedups via graph compilation
- Ecosystem: HuggingFace Transformers, vLLM, DeepSpeed all built on PyTorch
