---
title: Text Generation Inference (TGI)
url: https://huggingface.co/docs/text-generation-inference/en/index
maker: Hugging Face
tags: [llm, inference, serving]
created: 2026-05-14
---

# Text Generation Inference (TGI)

## What it is

TGI is Hugging Face's production-ready toolkit for deploying and serving open-weight LLMs. It ships as a Docker container and integrates natively with the Hugging Face Hub.

## What problem it solves

Researchers need to move from a Hub model checkpoint to a production inference endpoint without writing a serving stack. TGI provides continuous batching, quantization, and a REST API out of the box.

## Concepts

- [[llm-quantization]]
- [[flash-attention]]
- [[tensor-parallelism]]

## Notes

- Apache 2.0 license; Rust + Python
- Supports GPTQ, AWQ, and bitsandbytes quantization
- Flash Attention 2 and Paged Attention enabled by default where supported
- Powers Hugging Face's Inference Endpoints product
