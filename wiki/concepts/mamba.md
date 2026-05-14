---
title: Mamba (State Space Model)
tags: [llm, architecture, efficiency]
created: 2026-05-14
source: https://arxiv.org/pdf/2312.00752
---

# Mamba (State Space Model)

## Summary

Mamba is a sequence model based on structured state space models (SSMs) that achieves linear-time inference and training with respect to sequence length. You can think of it as a recurrent model that selectively filters what information to retain in its hidden state based on the input, unlike fixed-coefficient linear recurrences. You get Transformer-quality results on language tasks while gaining significantly faster inference on long sequences.

## Key Ideas

- Based on S4 (Structured State Space Sequence Model); Mamba adds input-dependent (selective) state transitions
- Selection mechanism: the state space parameters A, B, C become functions of the input, allowing dynamic focusing
- Trained efficiently via a hardware-aware parallel scan algorithm; no quadratic attention bottleneck
- Memory is fixed-size (state dimension × model width), enabling arbitrarily long contexts at constant memory
- Hybrid architectures (Jamba, Zamba) interleave Mamba layers with attention layers, combining strengths

## Related

- [[transformer]]
- [[rwkv]]
- [[flash-attention]]
- [[speculative-decoding]]
