---
title: vLLM
url: https://github.com/vllm-project/vllm
maker: vLLM Project (UC Berkeley)
tags: [llm, inference, serving]
created: 2026-05-14
---

# vLLM

## What it is

vLLM is a high-throughput LLM inference and serving engine developed at UC Berkeley. It exposes an OpenAI-compatible REST API and supports most major open-weight models.

## What problem it solves

GPU memory fragmentation limits how many concurrent requests a serving system can handle. vLLM's PagedAttention allocates KV-cache in non-contiguous blocks, dramatically improving throughput and concurrency without wasting memory.

## Concepts

- [[speculative-decoding]]
- [[flash-attention]]
- [[llm-quantization]]
- [[tensor-parallelism]]

## Notes

- Apache 2.0 license; Python/CUDA
- PagedAttention is the core innovation, borrowing paging from OS virtual memory
- Supports tensor and pipeline parallelism across multiple GPUs
- Continuous batching reduces latency variance across requests
