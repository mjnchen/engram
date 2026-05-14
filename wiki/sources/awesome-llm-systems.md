---
title: Awesome-LLM-Systems
url: https://github.com/AmberLJC/LLMSys-PaperList
tags: [llm, infrastructure, survey]
created: 2026-05-14
---

# Awesome-LLM-Systems

## Summary

Curated paper list on the infrastructure required to train and serve LLMs at scale, covering distributed training, memory management, and hardware efficiency. The systems perspective reveals that algorithmic advances in LLMs are often bottlenecked by systems challenges rather than mathematical ones.

## Key Points

- Distributed training at scale requires tensor parallelism, pipeline parallelism, and data parallelism in combination — no single strategy scales alone
- ZeRO optimizer sharding distributes optimizer states, gradients, and parameters across GPUs, enabling training of models 8x larger than GPU memory alone allows
- Flash Attention is a systems optimization, not an algorithmic change — same result, but reorders memory access to stay within SRAM
- KV cache is the primary memory bottleneck for serving — multi-query attention and grouped-query attention are architectural responses

## Concepts

- [[tensor-parallelism]]
- [[zero-redundancy-optimizer]]
- [[flash-attention]]
- [[mixture-of-experts]]

## Notes
