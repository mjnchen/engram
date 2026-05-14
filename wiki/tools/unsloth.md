---
title: Unsloth
url: https://github.com/unslothai/unsloth
maker: Unsloth AI
tags: [llm, training, fine-tuning]
created: 2026-05-14
---

# Unsloth

## What it is

Unsloth is an efficient fine-tuning framework by Unsloth AI that uses custom CUDA kernels to speed up LoRA training 2-5x while reducing memory usage compared to standard implementations.

## What problem it solves

LoRA fine-tuning on consumer or mid-range GPUs is slow and memory-constrained; Unsloth rewrites key backward-pass operations in Triton/CUDA to eliminate overhead without changing model behavior.

## Concepts

- [[lora]]
- [[flash-attention]]
- [[llm-quantization]]

## Notes

Supports Llama, Mistral, Gemma, and other popular architectures. Drop-in replacement for Hugging Face PEFT. Apache 2.0 license.
