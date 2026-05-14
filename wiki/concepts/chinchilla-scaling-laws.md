---
title: Chinchilla Scaling Laws
tags: [llm, scaling, training]
created: 2026-05-14
source: https://arxiv.org/pdf/2203.15556
---

# Chinchilla Scaling Laws

## Summary

The Chinchilla paper (Hoffmann et al., DeepMind 2022) revised earlier [[scaling-laws]] to show that for a fixed compute budget, the optimal strategy is to train a smaller model on proportionally more data than previously thought. The rule of thumb: train on roughly 20 tokens per parameter. Chinchilla (70B parameters, 1.4T tokens) outperformed Gopher (280B, 300B tokens) at the same compute cost.

## Key Ideas

- Optimal allocation: N ∝ C^{0.5} and D ∝ C^{0.5}, meaning model size and data should scale equally with compute
- Kaplan et al. (2020) underemphasized data scaling because they used small, fixed datasets; Chinchilla corrects this
- Implication: GPT-3 (175B) was significantly undertrained; a 70B model trained longer matches it
- Llama 1 explicitly applied Chinchilla ratios; Llama 2 trained even beyond Chinchilla-optimal for inference efficiency
- "Inference-optimal" training may justify training past Chinchilla optimum if deployment costs dominate training costs

## Related

- [[scaling-laws]]
- [[emergent-abilities]]
- [[llama-3]]
- [[zero-redundancy-optimizer]]
- [[tensor-parallelism]]
