---
title: Awesome-Align-LLM-Human
url: https://github.com/GaryYufei/AlignLLMHumanSurvey
tags: [llm, alignment, survey]
created: 2026-05-14
---

# Awesome-Align-LLM-Human

## Summary

Survey and paper list on the full alignment pipeline: collecting human preference data, training reward models, and updating the LLM via RL or direct methods. Covers both the InstructGPT RLHF approach and newer preference optimization methods like DPO that bypass the explicit reward model.

## Key Points

- RLHF requires a reward model trained on preference pairs, which itself can be gamed by the policy (reward hacking)
- DPO reformulates the alignment objective to optimize directly on preference data without a separate reward model
- Constitutional AI (CAI) uses the model's own judgments as a substitute for human feedback at scale
- Alignment tax: RLHF-tuned models sometimes perform worse on standard benchmarks than their base versions

## Concepts

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]
- [[instruction-tuning]]

## Notes
