---
title: Awesome-LLM-Inference
url: https://github.com/DefTruth/Awesome-LLM-Inference
tags: [llm, inference, survey]
created: 2026-05-14
---

# Awesome-LLM-Inference

## Summary

Paper and resource list focused on the systems side of LLM serving: batching strategies, memory management, and hardware-level optimizations. The core insight across papers is that LLM inference is memory-bandwidth-bound, not compute-bound, which inverts the usual GPU optimization assumptions.

## Key Points

- Continuous batching (Orca) dramatically improves GPU utilization over static batching by processing requests as tokens complete
- PagedAttention (vLLM) manages KV cache as virtual memory pages, nearly eliminating fragmentation waste
- Speculative decoding uses a small draft model to propose tokens, verified in parallel by the large model
- Quantization and KV cache compression are the main levers for fitting larger models into memory

## Concepts

- [[speculative-decoding]]
- [[flash-attention]]
- [[llm-quantization]]
- [[tensor-parallelism]]

## Notes
