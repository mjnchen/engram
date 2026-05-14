---
title: Guidance
url: https://github.com/microsoft/guidance
maker: Microsoft
tags: [llm, prompting, inference]
created: 2026-05-14
---

# Guidance

## What it is

Guidance is a templating language by Microsoft that interleaves control flow (conditionals, loops) with LLM generation in a single prompt program, enabling constrained and structured output.

## What problem it solves

Getting LLMs to reliably produce structured output (JSON, specific formats) requires awkward post-processing; Guidance constrains generation token-by-token so the model cannot produce invalid structure.

## Concepts

- [[prompt-engineering]]
- [[llm-hallucination]]

## Notes

Supports local models (llama.cpp, transformers) and API-based models. Token healing prevents formatting artifacts at generation boundaries. MIT license.
