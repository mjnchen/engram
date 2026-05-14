---
title: TensorRT-LLM
url: https://github.com/NVIDIA/TensorRT-LLM
maker: NVIDIA
tags: [llm, inference, efficiency]
created: 2026-05-14
---

# TensorRT-LLM

## What it is

TensorRT-LLM is NVIDIA's inference framework that compiles LLMs into optimized TensorRT engines. It extracts maximum throughput from NVIDIA GPUs through kernel fusion, quantization, and hardware-specific graph optimization.

## What problem it solves

General-purpose inference frameworks leave GPU performance on the table. TensorRT-LLM AOT-compiles model graphs to hardware-specific kernels, achieving higher token throughput than frameworks that rely on dynamic dispatch.

## Concepts

- [[llm-quantization]]
- [[flash-attention]]
- [[tensor-parallelism]]
- [[speculative-decoding]]

## Notes

- Apache 2.0 license; C++/Python
- Supports FP8, INT8, INT4 (AWQ/GPTQ) quantization on Hopper and Ada GPUs
- In-flight batching and paged KV-cache included
- Integrates with NVIDIA Triton Inference Server for production deployment
- Higher setup complexity than vLLM; best suited for dedicated inference fleets
