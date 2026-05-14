---
title: Awesome-LLM-Compression
url: https://github.com/HuangOwen/Awesome-LLM-Compression
tags: [llm, compression, efficiency]
created: 2026-05-14
---

# Awesome-LLM-Compression

## Summary

Organized paper list covering the three main LLM compression axes: pruning (removing weights), quantization (reducing precision), and knowledge distillation (training a smaller model on a larger one's outputs). The field converged on post-training quantization as the most practical approach for deployment because it requires no retraining.

## Key Points

- Structured pruning removes entire heads/layers and preserves hardware efficiency; unstructured pruning improves compression ratios but requires sparse hardware support
- GPTQ and AWQ are the dominant post-training quantization methods for LLMs, operating on weights rather than activations
- Distillation at the token-distribution level (matching logits) outperforms distillation at the output level
- 4-bit quantization with groupwise scaling retains most model quality; 2-bit causes significant degradation

## Concepts

- [[llm-quantization]]
- [[lora]]
- [[flash-attention]]

## Notes
