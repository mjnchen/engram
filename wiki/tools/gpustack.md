---
title: GPUStack
url: https://github.com/gpustack/gpustack
maker: GPUStack
tags: [llm, inference, infrastructure]
created: 2026-05-14
---

# GPUStack

## What it is

GPUStack is a Kubernetes-style cluster manager for GPU nodes focused on LLM inference workloads. It schedules and scales inference workers across heterogeneous GPU fleets with a web dashboard.

## What problem it solves

Running LLM inference across multiple GPU machines requires orchestration: scheduling models to appropriate hardware, load balancing requests, and monitoring utilization. GPUStack handles this without requiring a full Kubernetes setup.

## Concepts

- [[tensor-parallelism]]
- [[foundation-models]]

## Notes

- Apache 2.0 license; Go + Python
- Supports NVIDIA, AMD, Apple Silicon, and Ascend NPU backends
- Built-in model catalog pulls from Hugging Face Hub and ollama registry
- Provides OpenAI-compatible API endpoint for the whole cluster
- Lighter-weight alternative to running KServe or Ray Serve on Kubernetes
