---
title: LLM for Mathematical Reasoning
tags: [llm, reasoning, math]
created: 2026-05-14
source: https://github.com/atfortes/LM-Reasoning-Papers
---

# LLM for Mathematical Reasoning

## Summary

Mathematical reasoning in LLMs covers the methods and benchmarks for making language models reliably solve math problems — from grade-school arithmetic to competition-level proofs. You use specialized training data, prompting techniques, and tool augmentation to overcome the fragility of pure token prediction on formal numerical tasks. It is a leading indicator of general reasoning capability.

## Key Ideas

- Benchmarks: GSM8K (grade school word problems), MATH (competition problems), MGSM (multilingual), AIME
- [[chain-of-thought-prompting]] is essential: models that show work dramatically outperform those that answer directly
- Process Reward Models (PRMs): provide step-level supervision during training rather than only outcome-level; improves reliability
- Tool use: connecting LLMs to Python interpreters (PoT: Program of Thought) offloads arithmetic to exact computation
- Reinforcement learning on verifiable rewards: since math answers are checkable, RL against a correctness signal is tractable (see [[deepseek-r1]], [[tinyzero]])
- Self-consistency sampling improves accuracy without additional training by taking majority vote over many reasoning chains

## Related

- [[chain-of-thought-prompting]]
- [[tree-of-thoughts]]
- [[code-llms]]
- [[llm-agents]]
- [[deepseek-r1]]
- [[tinyzero]]
- [[prompt-engineering]]
