---
title: State of GPT (Microsoft Build 2023)
url: https://build.microsoft.com/en-US/sessions/db3f4859-cd30-4445-a0cd-553c3304f8e2
tags: [llm, overview, training]
created: 2026-05-14
---

# State of GPT (Microsoft Build 2023)

## Summary

Andrej Karpathy's 2023 presentation walking through how GPT models are trained stage by stage and what that means for how to use them effectively. The most practically useful section is the mental model it provides: the base model is a document completer, and RLHF is what turns it into an assistant.

## Key Points

- GPT training pipeline: pre-training → SFT → reward model training → PPO/RLHF — each stage has a distinct purpose
- The base model "wants to" complete documents, not follow instructions — few-shot prompting works by making the desired behavior look like a natural document continuation
- RLHF significantly shifts the distribution: the assistant is more opinionated, more concise, and more likely to refuse
- For complex tasks: use chain-of-thought, give the model time to "think", avoid asking it to do too much in one pass

## Concepts

- [[rlhf]]
- [[instruction-tuning]]
- [[chain-of-thought-prompting]]
- [[prompt-engineering]]
- [[foundation-models]]

## Notes
