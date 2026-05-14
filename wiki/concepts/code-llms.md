---
title: Code LLMs
tags: [llm, coding, research]
created: 2026-05-14
source: https://github.com/huybery/Awesome-Code-LLM
---

# Code LLMs

## Summary

Code LLMs are language models pretrained or fine-tuned specifically on source code, enabling code generation, completion, bug fixing, and translation across programming languages. You use them to automate software engineering tasks that require understanding syntax, semantics, and the conventions of programming languages. They are trained on GitHub repositories, competitive programming sites, and documentation.

## Key Ideas

- Pretraining corpora: The Stack (GitHub permissive licenses), CodeSearchNet, APPS, HumanEval for eval
- Evaluation benchmarks: HumanEval (functional correctness via unit tests), MBPP, SWE-bench (real GitHub issues)
- Models: Codex (GPT fine-tuned on code), CodeLlama (LLaMA fine-tuned), DeepSeek-Coder, StarCoder
- Fill-in-the-middle (FIM) training: randomly mask middle spans and train to predict them; critical for code completion tools
- Code models benefit from [[chain-of-thought-prompting]] for multi-step reasoning about programs
- Self-repair: use test execution feedback to iteratively debug generated code (execution-guided refinement)

## Related

- [[instruction-tuning]]
- [[chain-of-thought-prompting]]
- [[llm-math-reasoning]]
- [[prompt-engineering]]
- [[lm-evaluation-harness]]
