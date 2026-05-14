---
title: Prompt Engineering
tags: [llm, prompting, inference]
created: 2026-05-14
source: https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/
---

# Prompt Engineering

## Summary

Prompt engineering is the practice of designing input text to elicit desired behavior from a language model without changing its weights. You control model outputs through instruction phrasing, few-shot examples, output format specification, and persona assignment. You interact with deployed LLMs almost entirely through this interface.

## Key Ideas

- Few-shot prompting: include input-output examples in the prompt to prime the model toward a format or task
- Zero-shot: rely on instruction following from [[instruction-tuning]]; no examples needed for capable models
- Role prompting: assigning a persona ("You are an expert in X") shifts output style and accuracy on domain tasks
- Output formatting: requesting JSON, markdown, or step-by-step responses significantly improves downstream parseability
- Prompt injection and jailbreaking are adversarial failure modes where malicious inputs override intended behavior
- [[chain-of-thought-prompting]] and [[tree-of-thoughts]] are specialized prompting techniques for reasoning tasks

## Related

- [[chain-of-thought-prompting]]
- [[tree-of-thoughts]]
- [[instruction-tuning]]
- [[llm-security]]
- [[guidance]]
- [[outlines]]
- [[dspy]]
