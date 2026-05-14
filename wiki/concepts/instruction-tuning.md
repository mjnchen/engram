---
title: Instruction Tuning
tags: [llm, training, alignment]
created: 2026-05-14
source: https://arxiv.org/pdf/2210.11416.pdf
---

# Instruction Tuning

## Summary

Instruction tuning fine-tunes a pretrained language model on a large collection of tasks formatted as natural language instructions with expected outputs. You use it to make a model that was trained to predict next tokens behave as an instruction-following assistant. You get dramatically improved zero-shot generalization to unseen tasks without requiring task-specific prompting.

## Key Ideas

- Training data consists of (instruction, output) pairs covering diverse tasks: summarization, translation, QA, classification, etc.
- Scaling the number and diversity of instruction types improves generalization more than scaling data volume for a fixed task
- FLAN, InstructGPT, and Alpaca are prominent examples; they show that instruction tuning transfers across tasks
- Works synergistically with [[rlhf]]: instruction tuning first, then RLHF to align outputs with human preferences
- Chain-of-thought examples in instruction tuning data improve reasoning performance

## Related

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]
- [[chain-of-thought-prompting]]
- [[lora]]
