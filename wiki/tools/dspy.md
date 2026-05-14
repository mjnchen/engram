---
title: DSPy
url: https://github.com/stanfordnlp/dspy
maker: Stanford NLP
tags: [llm, framework, prompting]
created: 2026-05-14
---

# DSPy

## What it is

DSPy is a programming framework by Stanford NLP that compiles declarative LLM pipelines by automatically optimizing prompts and model weights rather than requiring hand-written prompts.

## What problem it solves

Hand-crafted prompts are brittle and hard to tune; DSPy treats prompt optimization as a compilation problem, searching for instructions and few-shot examples that maximize a metric on a dev set.

## Concepts

- [[prompt-engineering]]
- [[chain-of-thought-prompting]]
- [[instruction-tuning]]

## Notes

Supports multiple optimizers (BootstrapFewShot, MIPRO, BayesianSignatureOptimizer). MIT license.
