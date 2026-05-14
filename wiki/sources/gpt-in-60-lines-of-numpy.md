---
title: GPT in 60 Lines of NumPy
url: https://jaykmody.com/blog/gpt-from-scratch/
tags: [llm, tutorial, architecture]
created: 2026-05-14
---

# GPT in 60 Lines of NumPy

## Summary

Minimal GPT implementation in pure NumPy that strips away framework abstractions to expose the core forward pass. Useful for building intuition because every matrix multiply is explicit and the full model fits in a single screen of code.

## Key Points

- The full GPT-2 forward pass is: token embed → positional embed → N × (layer norm → attention → layer norm → MLP) → layer norm → unembed
- Multi-head attention splits Q, K, V into heads, computes attention independently, then concatenates — the split is purely computational, not conceptual
- Softmax temperature scaling at inference directly controls output diversity (lower temp = more greedy)
- The parameter count is dominated by the embedding matrix and MLP layers, not the attention weights

## Concepts

- [[transformer]]
- [[bpe-tokenization]]

## Notes
