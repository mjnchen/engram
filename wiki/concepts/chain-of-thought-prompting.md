---
title: Chain-of-Thought Prompting
tags: [llm, prompting, reasoning]
created: 2026-05-14
source: https://arxiv.org/pdf/2201.11903.pdf
---

# Chain-of-Thought Prompting

## Summary

Chain-of-thought (CoT) prompting elicits step-by-step reasoning from a language model by including reasoning traces in the prompt examples. You use it to improve performance on tasks that require multi-step logic—arithmetic, commonsense reasoning, symbolic reasoning—without changing model weights. The key insight is that decomposing a problem into intermediate steps substantially improves accuracy over direct answer prompting.

## Key Ideas

- Few-shot CoT: include exemplars with explicit reasoning steps; the model mimics the format
- Zero-shot CoT: append "Let's think step by step" to the prompt, which is surprisingly effective
- Gains are most pronounced in large models (100B+ parameters); smaller models benefit less
- CoT emerges as an ability that is not present in small models, suggesting it's an [[emergent-abilities]] phenomenon
- Self-consistency: sample multiple reasoning chains and take majority vote to improve robustness

## Related

- [[tree-of-thoughts]]
- [[prompt-engineering]]
- [[emergent-abilities]]
- [[llm-math-reasoning]]
- [[llm-agents]]
