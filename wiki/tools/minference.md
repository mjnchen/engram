---
title: MInference
url: https://github.com/microsoft/MInference
maker: Microsoft
tags: [llm, inference, efficiency]
created: 2026-05-14
---

# MInference

## What it is

MInference is a sparse attention inference technique from Microsoft Research. It accelerates the prefill phase of long-context LLM inference by identifying and computing only the most important attention patterns.

## What problem it solves

Prefilling a 1M-token context with full attention is quadratically expensive. MInference achieves ~10x prefill speedup by exploiting the observation that long-context attention is sparse and follows predictable static patterns (A-shape, vertical-slash, block-sparse).

## Concepts

- [[flash-attention]]
- [[speculative-decoding]]

## Notes

- MIT license; Python
- Works as a drop-in wrapper around existing models — no retraining or fine-tuning needed
- Three identified attention head patterns: A-shape, vertical-slash, block-sparse
- Evaluated on LLaMA, Mistral, Phi-3 with minimal accuracy degradation
- Targets prefill only; decode phase is unchanged
