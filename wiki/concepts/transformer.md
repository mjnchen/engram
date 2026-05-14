---
title: Attention Is All You Need (Transformer)
tags: [llm, architecture, training]
created: 2026-05-14
source: https://arxiv.org/pdf/1706.03762.pdf
---

# Attention Is All You Need (Transformer)

## Summary

The Transformer is a neural network architecture that replaced recurrence and convolutions with self-attention to model sequential data. You can think of it as a mechanism that lets every token in a sequence directly attend to every other token, capturing long-range dependencies without processing words one-by-one. You will find it at the foundation of virtually all modern large language models.

## Key Ideas

- Self-attention computes a weighted sum of all positions in the sequence for each position, using query, key, and value matrices
- Multi-head attention runs several attention operations in parallel, each learning different relationships
- Positional encodings inject sequence order information since attention itself is permutation-invariant
- The encoder-decoder architecture was designed for translation; decoder-only variants (GPT-style) dominate generative LLMs
- Attention complexity scales quadratically with sequence length, motivating research into efficient variants

## Related

- [[flash-attention]]
- [[bert]]
- [[t5]]
- [[mixture-of-experts]]
- [[mamba]]
- [[rwkv]]
- [[scaling-laws]]
