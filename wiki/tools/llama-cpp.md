---
title: llama.cpp
url: https://github.com/ggerganov/llama.cpp
maker: Georgi Gerganov
tags: [llm, inference, local]
created: 2026-05-14
---

# llama.cpp

## What it is

llama.cpp is a C/C++ inference runtime for LLMs written by Georgi Gerganov. It runs on CPU and GPU with no Python dependency, and is the foundation for most local LLM tooling.

## What problem it solves

Running large language models requires GPUs with substantial VRAM. llama.cpp enables inference on consumer hardware — including CPU-only machines — through aggressive quantization (2-bit to 8-bit) and efficient memory layout.

## Concepts

- [[llm-quantization]]
- [[flash-attention]]

## Notes

- MIT license; pure C/C++
- Introduced the GGUF file format (successor to GGML) for portable quantized weights
- Supports Metal (Apple Silicon), CUDA, Vulkan, and CPU backends
- Underpins ollama, LM Studio, Jan, and many other local LLM tools
