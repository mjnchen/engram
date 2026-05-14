---
title: Flash Attention
tags: [llm, training, efficiency]
created: 2026-05-14
source: https://arxiv.org/pdf/2205.01068.pdf
---

# Flash Attention

## Summary

Flash Attention is a GPU-efficient implementation of exact attention that reduces memory usage from O(N²) to O(N) by tiling the attention computation to stay within fast on-chip SRAM rather than reading/writing to slow HBM. You get the same mathematical result as standard attention but dramatically faster wall-clock time and lower peak memory. You will find it as the de facto attention implementation in most LLM training and inference frameworks.

## Key Ideas

- Standard attention materializes the full N×N attention matrix in HBM (GPU global memory), which is the bottleneck
- Flash Attention tiles the computation: processes blocks of Q, K, V that fit in SRAM, updating output incrementally
- Uses the online softmax trick to compute softmax correctly without seeing the full row at once
- Flash Attention 2 improved parallelism across the sequence dimension and reduced non-matmul FLOPs
- Flash Attention 3 adds async pipelining and FP8 support for H100 GPUs
- Enables training on longer context windows that would OOM with standard attention

## Related

- [[transformer]]
- [[mixture-of-experts]]
- [[zero-redundancy-optimizer]]
- [[tensor-parallelism]]
- [[lora]]
