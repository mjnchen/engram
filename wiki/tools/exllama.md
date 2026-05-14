---
title: exllama
url: https://github.com/turboderp/exllama
maker: turboderp
tags: [llm, inference, efficiency]
created: 2026-05-14
---

# exllama

## What it is

exllama (and its successor exllamav2) is a memory-efficient quantized inference engine by turboderp. It targets consumer NVIDIA GPUs and is optimized for GPTQ-quantized models.

## What problem it solves

Consumer GPUs have limited VRAM (8–24 GB). exllama minimizes memory overhead through custom CUDA kernels for quantized matrix-vector products, enabling larger models to run on GPUs that cannot fit the full-precision weights.

## Concepts

- [[llm-quantization]]

## Notes

- MIT license; Python/CUDA
- Successor exllamav2 adds EXL2 quantization format with variable bit-width per layer
- Significantly faster than llama.cpp on NVIDIA hardware for the same quantization level
- Widely used as the backend for text-generation-webui
