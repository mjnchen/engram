---
title: Prompt Engineering (Lilian Weng)
url: https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/
tags: [llm, prompting, overview]
created: 2026-05-14
---

# Prompt Engineering (Lilian Weng)

## Summary

Thorough survey of prompting techniques written by an OpenAI researcher, covering the spectrum from zero-shot to multi-step reasoning. The post is notable for being grounded in experiments rather than just cataloging techniques, and for situating prompting within what is known about how LLMs process instructions.

## Key Points

- Few-shot examples work not just by showing format but by activating the model's learned task representations
- Chain-of-thought prompting requires the examples themselves to contain reasoning traces, not just answers
- Self-consistency (sampling and voting) is more reliable than greedy decoding for reasoning tasks
- Prompt sensitivity is a real problem: minor wording changes can substantially change outputs, especially for smaller models

## Concepts

- [[prompt-engineering]]
- [[chain-of-thought-prompting]]
- [[instruction-tuning]]
- [[emergent-abilities]]

## Notes
