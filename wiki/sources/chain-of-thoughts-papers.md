---
title: Chain-of-Thoughts Papers
url: https://github.com/Timothyxxx/Chain-of-ThoughtsPapers
tags: [llm, reasoning, prompting]
created: 2026-05-14
---

# Chain-of-Thoughts Papers

## Summary

Paper collection tracing chain-of-thought from the original Wei et al. discovery through extensions like zero-shot CoT, self-consistency, and tree-of-thoughts. The thread shows that eliciting intermediate reasoning steps is the single biggest lever for improving LLM performance on multi-step tasks.

## Key Points

- Chain-of-thought only reliably emerges in models above ~100B parameters — smaller models produce plausible-looking but incorrect chains
- Zero-shot CoT ("Let's think step by step") is surprisingly effective without any few-shot examples
- Self-consistency — sampling multiple chains and majority-voting — outperforms greedy decoding significantly
- Later work extends from linear chains to tree search and graph-based reasoning

## Concepts

- [[chain-of-thought-prompting]]
- [[tree-of-thoughts]]
- [[emergent-abilities]]
- [[prompt-engineering]]

## Notes
