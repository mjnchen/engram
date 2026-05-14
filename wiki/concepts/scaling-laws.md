---
title: Scaling Laws for Neural Language Models
tags: [llm, training, scaling]
created: 2026-05-14
source: https://arxiv.org/pdf/2001.08361.pdf
---

# Scaling Laws for Neural Language Models

## Summary

Scaling laws describe how language model performance improves predictably as you increase model size, dataset size, and compute. The original Kaplan et al. paper showed that loss follows power-law relationships with each of these variables, enabling you to forecast model quality before training. This gave the field a principled framework for allocating compute budgets.

## Key Ideas

- Loss decreases as a power law with model parameters N, dataset tokens D, and compute C: L ∝ N^α, D^β, C^γ
- Model size dominates in the original findings: given a fixed compute budget, you should train larger models for fewer steps
- The relationship holds across many orders of magnitude with little deviation
- Architectural details (depth vs. width, attention heads) matter far less than total parameter count
- [[chinchilla-scaling-laws]] revised these findings, showing Kaplan-era models were significantly undertrained on data

## Related

- [[chinchilla-scaling-laws]]
- [[emergent-abilities]]
- [[foundation-models]]
- [[zero-redundancy-optimizer]]
- [[tensor-parallelism]]
