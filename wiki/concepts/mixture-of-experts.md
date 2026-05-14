---
title: Mixture of Experts (MoE)
tags: [llm, architecture, efficiency]
created: 2026-05-14
source: https://arxiv.org/pdf/2101.03961.pdf
---

# Mixture of Experts (MoE)

## Summary

Mixture of Experts replaces a dense feed-forward layer in a Transformer with multiple parallel "expert" networks, routing each token to only a subset of experts (typically 1-2) via a learned gating function. You get a model with far more total parameters than a dense model while keeping per-token compute constant. This decouples model capacity from inference cost.

## Key Ideas

- A router network scores each token against all experts and selects the top-k; only those experts run for that token
- Total parameter count scales with number of experts; FLOPs per token stays roughly the same as a smaller dense model
- Load balancing is a critical challenge: without auxiliary losses, routing collapses to a few popular experts
- Mixtral 8x7B showed MoE can match larger dense models at lower inference cost; GPT-4 is rumored to be MoE
- Communication overhead across devices (expert parallelism) adds infrastructure complexity during training

## Related

- [[transformer]]
- [[scaling-laws]]
- [[mixtral-8x7b]]
- [[tensor-parallelism]]
- [[flash-attention]]
