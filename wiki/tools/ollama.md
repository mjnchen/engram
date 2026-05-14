---
title: ollama
url: https://github.com/ollama/ollama
maker: Ollama
tags: [llm, inference, local]
created: 2026-05-14
---

# ollama

## What it is

ollama is a local LLM runtime with a Docker-like CLI and REST API. It wraps llama.cpp under the hood and manages model downloads, versioning, and a background server process.

## What problem it solves

Setting up llama.cpp directly requires manual model downloads, format conversion, and flag configuration. ollama reduces this to `ollama run llama3` — a single command that fetches and runs any model from its registry.

## Concepts

- [[llm-quantization]]
- [[foundation-models]]

## Notes

- MIT license; Go + llama.cpp backend
- Modelfile system allows custom system prompts and parameter presets (similar to Dockerfile)
- OpenAI-compatible REST API at `localhost:11434`
- Supports macOS (Metal), Linux (CUDA/ROCm), and Windows
