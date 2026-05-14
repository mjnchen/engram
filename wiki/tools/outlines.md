---
title: Outlines
url: https://github.com/normal-computing/outlines
maker: Normal Computing
tags: [llm, inference, structured-output]
created: 2026-05-14
---

# Outlines

## What it is

Outlines is a structured text generation library by Normal Computing that constrains LLM outputs to JSON schemas, regex patterns, or context-free grammars at the logit level.

## What problem it solves

Reliably extracting structured data from LLMs requires enforcing output format guarantees that sampling alone cannot provide; Outlines uses finite-state machines to mask invalid tokens at each generation step.

## Concepts

- [[prompt-engineering]]
- [[llm-hallucination]]

## Notes

Works with local models via transformers and llama.cpp. Zero overhead vs. unguided generation for many schemas. Apache 2.0 license.
