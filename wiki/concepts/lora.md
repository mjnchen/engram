---
title: LoRA (Low-Rank Adaptation)
tags: [llm, training, fine-tuning]
created: 2026-05-14
source: https://arxiv.org/abs/2106.09685
---

# LoRA (Low-Rank Adaptation)

## Summary

LoRA is a parameter-efficient fine-tuning method that freezes pretrained model weights and injects trainable low-rank decomposition matrices into each Transformer layer. You train only these small adapter matrices (rank r << d) instead of the full model, reducing trainable parameters by orders of magnitude while recovering most of the performance of full fine-tuning. This makes fine-tuning feasible on consumer hardware.

## Key Ideas

- Decomposes weight updates as ΔW = AB where A ∈ ℝ^{d×r} and B ∈ ℝ^{r×k}, with r << min(d, k)
- Typically applied to query and value projection matrices in attention; can extend to all linear layers
- At inference, you can merge the adapter weights into the base model (W + AB) for zero overhead
- QLoRA combines 4-bit quantized base model with LoRA adapters, fitting 65B models on a single consumer GPU
- Dozens of variants: AdaLoRA (adaptive rank), DoRA (magnitude+direction decomposition), LoRA+

## Related

- [[instruction-tuning]]
- [[rlhf]]
- [[llm-quantization]]
- [[flash-attention]]
- [[axolotl]]
- [[unsloth]]
