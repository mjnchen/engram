---
title: nanotron
url: https://github.com/huggingface/nanotron
maker: Hugging Face
tags: [llm, training, infrastructure]
created: 2026-05-14
---

# nanotron

## What it is

nanotron is a minimalistic 3D-parallelism LLM training framework by Hugging Face designed for research clarity and experimentation rather than production complexity.

## What problem it solves

Large training codebases (Megatron, NeMo) are hard to modify for research; nanotron provides a clean, readable implementation of tensor + pipeline + data parallelism that researchers can understand and extend quickly.

## Concepts

- [[tensor-parallelism]]
- [[foundation-models]]
- [[transformer]]

## Notes

Used to train Hugging Face's SmolLM and other research models. Apache 2.0 license.
