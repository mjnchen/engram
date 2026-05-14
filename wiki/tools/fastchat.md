---
title: FastChat
url: https://github.com/lm-sys/FastChat
maker: LMSYS
tags: [llm, inference, serving]
created: 2026-05-14
---

# FastChat

## What it is

FastChat is a distributed multi-model serving system built by LMSYS (Berkeley/CMU). It powers Chatbot Arena and exposes an OpenAI-compatible REST API for serving multiple models simultaneously.

## What problem it solves

Research teams need to serve many models side-by-side for evaluation and comparison. FastChat's controller/worker architecture lets you add or remove model workers independently without restarting the whole stack.

## Concepts

- [[instruction-tuning]]
- [[rlhf]]
- [[llm-alignment]]
- [[foundation-models]]

## Notes

- Apache 2.0 license; Python
- Originated as the serving infrastructure for Vicuna and Chatbot Arena
- Supports vLLM as a worker backend for high-throughput serving
- Includes a web UI, CLI, and OpenAI-compatible API server
