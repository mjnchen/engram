---
title: Wllama
url: https://github.com/ngxson/wllama
maker: ngxson
tags: [llm, inference, browser]
created: 2026-05-14
---

# Wllama

## What it is

Wllama is a WebAssembly binding for llama.cpp that runs LLM inference directly in the browser. It requires no server — the model weights are fetched and executed entirely client-side.

## What problem it solves

Deploying LLMs typically requires server infrastructure. Wllama enables privacy-preserving, zero-backend inference in any modern browser by compiling llama.cpp to WASM and leveraging multi-threading via SharedArrayBuffer.

## Concepts

- [[llm-quantization]]
- [[foundation-models]]

## Notes

- MIT license; TypeScript/WASM
- Requires HTTPS and cross-origin isolation headers (`COOP`/`COEP`) for multi-threaded mode
- Model files are streamed and cached in the browser's Cache API
- Performance is CPU-bound; practical for small models (1–3B parameters at 4-bit)
- Provides a React hook and vanilla JS API
