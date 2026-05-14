---
title: Speculative Decoding
tags: [llm, inference, efficiency]
created: 2026-05-14
source: https://github.com/DefTruth/Awesome-LLM-Inference
---

# Speculative Decoding

## Summary

Speculative decoding accelerates autoregressive LLM inference by using a small draft model to propose multiple tokens at once, then verifying them in parallel with the large target model. You get a speed-up because the large model can check K tokens in one forward pass rather than generating them one-by-one, while guaranteeing the output distribution is identical to standard sampling. Typical speed-ups are 2-3x for text tasks.

## Key Ideas

- Draft model (small, fast) generates a candidate sequence of K tokens autoregressively
- Target model (large, expensive) evaluates all K tokens in a single parallel forward pass
- Acceptance criterion: each token is accepted with probability min(1, p_target(x) / p_draft(x)); rejected tokens are resampled from a corrected distribution, guaranteeing output identical to sampling from the target model alone
- Works best when draft and target models share vocabulary and the draft is well-aligned with the target distribution
- Self-speculative decoding: use early layers or a pruned version of the same model as the draft, avoiding a separate model
- Medusa and EAGLE extend the approach with multiple parallel draft heads attached to the target model

## Related

- [[llm-quantization]]
- [[flash-attention]]
- [[mamba]]
- [[rwkv]]
- [[vllm]]
- [[tgi]]
- [[tensorrt-llm]]
