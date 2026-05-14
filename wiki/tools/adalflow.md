---
title: AdalFlow
url: https://github.com/SylphAI-Inc/AdalFlow
maker: SylphAI
tags: [llm, framework, optimization]
created: 2026-05-14
---

# AdalFlow

## What it is

AdalFlow is an LLM application optimization library by SylphAI that applies auto-differentiation principles to jointly optimize prompt instructions and retrieval components.

## What problem it solves

Tuning LLM pipelines manually is labor-intensive; AdalFlow treats the pipeline as a computation graph and uses gradient-like signals to automatically improve prompts and retriever parameters end-to-end.

## Concepts

- [[prompt-engineering]]
- [[rag]]
- [[chain-of-thought-prompting]]

## Notes

Inspired by PyTorch's autograd design. Suitable for both prompt-only and hybrid retrieval+generation systems. MIT license.
