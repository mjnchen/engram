---
title: ChatGPT Prompt Engineering for Developers (DeepLearning.AI)
url: https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/
tags: [llm, prompting, tutorial]
created: 2026-05-14
---

# ChatGPT Prompt Engineering for Developers (DeepLearning.AI)

## Summary

Short course by Isa Fulford (OpenAI) and Andrew Ng covering practical prompting patterns for developers building on the ChatGPT API. Focuses on the instruction-following model rather than the base model, so all techniques assume an aligned assistant.

## Key Points

- Two core principles: write clear specific instructions, and give the model time to think (avoid asking for immediate answers to complex questions)
- Delimiters (triple quotes, XML tags) help the model distinguish instructions from content, reducing prompt injection risk
- Iterative prompt development — start simple, identify failure modes, refine — is more effective than trying to write the perfect prompt first
- Output format specification (JSON, markdown, specific fields) dramatically improves reliability for downstream parsing

## Concepts

- [[prompt-engineering]]
- [[instruction-tuning]]
- [[chain-of-thought-prompting]]

## Notes
