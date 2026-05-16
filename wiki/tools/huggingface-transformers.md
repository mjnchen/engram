---
title: HuggingFace Transformers
url: https://github.com/huggingface/transformers
maker: HuggingFace
tags: [transformers, huggingface, pytorch, tensorflow, jax, framework]
created: 2026-05-15
---

# HuggingFace Transformers

## What it is

The dominant open-source library for loading, fine-tuning, and running transformer-based models. Supports PyTorch, TensorFlow, and JAX backends. Provides a unified API across thousands of pretrained models on the HuggingFace Hub.

## What problem it solves

Removes the need to reimplement model architectures from scratch. Download any pretrained model in a few lines; fine-tune with Trainer; export to ONNX or TorchScript for inference.

## Concepts

- [[transformer]]
- [[instruction-tuning]]
- [[lora]]

## Notes

- Standard entry point for open-source LLM work
- Integrates with PEFT for LoRA/QLoRA fine-tuning
- Hub hosts model weights, tokenizers, and datasets
