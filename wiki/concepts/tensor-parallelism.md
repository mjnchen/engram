---
title: Megatron-LM (Tensor Parallelism)
tags: [llm, training, infrastructure]
created: 2026-05-14
source: https://arxiv.org/pdf/1909.08053.pdf
---

# Megatron-LM (Tensor Parallelism)

## Summary

Tensor parallelism, introduced by Megatron-LM, splits individual weight matrices across multiple GPUs so each device holds and computes a shard of each layer. You use it when a single layer is too large to fit on one GPU, complementing data parallelism (splitting the batch) and pipeline parallelism (splitting layers). Megatron-LM combined all three strategies to train GPT-3-scale models before [[zero-redundancy-optimizer]] became widespread.

## Key Ideas

- Column-parallel linear: split weight matrix column-wise; each GPU computes a partial output, then an all-reduce synchronizes
- Row-parallel linear: split weight matrix row-wise; each GPU takes a chunk of the input
- In Transformer blocks: attention heads split across GPUs naturally; MLP can also be column+row parallel
- Sequence parallelism (Megatron v3): distribute layer norm and dropout across GPUs to reduce activation memory
- Combined with pipeline parallelism (layers split across stages) and data parallelism for trillion-parameter training
- 3D parallelism (tensor × pipeline × data) is the standard approach at the largest scales

## Related

- [[zero-redundancy-optimizer]]
- [[scaling-laws]]
- [[flash-attention]]
- [[mixture-of-experts]]
- [[deepspeed]]
- [[megatron-lm]]
