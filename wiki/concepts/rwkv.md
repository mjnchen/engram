---
title: RWKV
tags: [llm, architecture, inference]
created: 2026-05-14
source: https://arxiv.org/abs/2305.13048
---

# RWKV

## Summary

RWKV is a language model architecture that combines the parallelizable training of Transformers with the constant-memory inference of RNNs. You train it like a Transformer using parallelism over the sequence, but at inference time it runs as a recurrent network with a fixed-size hidden state, making it O(1) in memory per step. This makes it suitable for long contexts and resource-constrained deployment.

## Key Ideas

- "Receptance Weighted Key Value" — reformulates attention as a linear recurrence that can be computed in parallel during training
- At inference, the model maintains a rolling hidden state rather than a growing KV cache; memory is constant regardless of context length
- Trades the ability to attend to arbitrary positions (Transformer) for linear-time inference; information from distant positions decays
- Competitive with Transformer models of similar size on language benchmarks, though typically slightly behind
- An alternative to [[mamba]] in the sub-quadratic architecture space

## Related

- [[transformer]]
- [[mamba]]
- [[flash-attention]]
- [[speculative-decoding]]
- [[llm-quantization]]
