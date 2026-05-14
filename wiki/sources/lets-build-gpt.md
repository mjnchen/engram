---
title: Let's build GPT (Andrej Karpathy)
url: https://www.youtube.com/watch?v=kCc8FmEb1nY
tags: [llm, tutorial, architecture]
created: 2026-05-14
---

# Let's build GPT (Andrej Karpathy)

## Summary

Video tutorial building a character-level GPT from scratch in PyTorch, explaining every architectural decision as it's added. Starts from a bigram model and builds up to multi-head self-attention, making the transformer architecture concrete rather than abstract.

## Key Points

- Self-attention is "nodes in a graph looking at each other" — each token aggregates information from previous tokens weighted by learned compatibility scores
- The residual stream is a communication highway: attention heads and MLP layers read from and write back to it
- Layer normalization happens before attention and MLP (pre-norm) in modern transformers, not after as in the original paper
- Scaling from character-level to BPE tokens and from 1M to 1T parameters is mostly engineering, not new algorithms

## Concepts

- [[transformer]]
- [[flash-attention]]
- [[bpe-tokenization]]
- [[foundation-models]]

## Notes
