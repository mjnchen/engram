---
title: EasyEdit
url: https://github.com/zjunlp/EasyEdit
maker: Zhejiang University NLP
tags: [llm, research, tooling]
created: 2026-05-14
---

# EasyEdit

## What it is

Unified Python framework from Zhejiang University NLP group for editing factual knowledge stored in LLMs using multiple editing algorithms.

## What problem it solves

Retraining an LLM to correct or update a single fact is prohibitively expensive; EasyEdit provides plug-in methods (ROME, MEMIT, FT, etc.) to surgically modify model weights.

## Concepts

- [[model-editing]]
- [[llm-hallucination]]

## Notes

- Supports ROME, MEMIT, GRACE, IKE, and other editing methods
- Works with LLaMA, GPT-2, GPT-J, and other HuggingFace models
- Apache 2.0 licensed
