---
title: A Visual Guide to Mamba
url: https://maartengrootendorst.substack.com/p/a-visual-guide-to-mamba-and-state
tags: [llm, architecture, tutorial]
created: 2026-05-14
---

# A Visual Guide to Mamba

## Summary

Illustrated explainer of the Mamba state space model, showing how it processes sequences through a hidden state update instead of attention. The key contrast with transformers is that Mamba's inference cost is constant per token (recurrent) while its training is still parallelizable via the parallel scan algorithm.

## Key Points

- State space models represent sequence processing as a continuous-time system discretized into steps — Mamba learns the discretization parameters
- Unlike LSTM hidden states, Mamba's selection mechanism makes the state transition input-dependent, fixing the fixed-dynamics problem of linear RNNs
- At inference time Mamba is O(1) per token vs O(n) for attention, making it significantly faster for long sequences
- Mamba-2 bridges SSMs and attention by showing they are instances of the same structured state space duality

## Concepts

- [[mamba]]
- [[transformer]]
- [[rwkv]]

## Notes
