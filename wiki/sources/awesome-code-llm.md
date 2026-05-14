---
title: Awesome-Code-LLM
url: https://github.com/huybery/Awesome-Code-LLM
tags: [llm, coding, survey]
created: 2026-05-14
---

# Awesome-Code-LLM

## Summary

Research paper list on code-specialized language models, covering training data, benchmarks, and model architectures. Code LLMs differ from general LLMs in that their training data has ground-truth correctness signals (tests pass or fail), enabling stronger reinforcement learning without human annotators.

## Key Points

- Code pre-training improves general reasoning in LLMs even when code is not the target task
- HumanEval and MBPP are the standard pass@k benchmarks; models now saturate HumanEval, pushing the field to harder benchmarks (LiveCodeBench, SWE-bench)
- Fill-in-the-middle (FIM) training teaches models to complete code given prefix and suffix context, critical for IDE use
- Execution feedback (running generated code) is a stronger training signal than human preference for code tasks

## Concepts

- [[code-llms]]
- [[instruction-tuning]]
- [[rlhf]]

## Notes
