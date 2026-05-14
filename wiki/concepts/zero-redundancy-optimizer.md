---
title: ZeRO (Zero Redundancy Optimizer)
tags: [llm, training, efficiency]
created: 2026-05-14
source: https://arxiv.org/pdf/1910.02054.pdf
---

# ZeRO (Zero Redundancy Optimizer)

## Summary

ZeRO is a memory optimization strategy for training large models across multiple GPUs that eliminates redundant copies of optimizer states, gradients, and model parameters. You use it to train models too large to fit on a single GPU by partitioning these tensors across all devices instead of replicating them. You achieve near-linear memory reduction with the number of devices while maintaining computational efficiency.

## Key Ideas

- Three stages: Stage 1 shards optimizer states, Stage 2 adds gradient sharding, Stage 3 shards model parameters
- Stage 3 reduces per-GPU memory by ~Nx where N is the number of GPUs, enabling trillion-parameter training
- Communication overhead replaces memory overhead: all-gather and reduce-scatter ops replace full replication
- ZeRO-Infinity extends to CPU and NVMe memory when GPU memory is exhausted
- Implemented in [[deepspeed]]; tightly integrated into the HuggingFace training ecosystem

## Related

- [[scaling-laws]]
- [[tensor-parallelism]]
- [[flash-attention]]
- [[deepspeed]]
- [[megatron-lm]]
