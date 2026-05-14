---
title: Quantization (LLM)
tags: [llm, inference, efficiency]
created: 2026-05-14
source: https://github.com/HuangOwen/Awesome-LLM-Compression
---

# Quantization (LLM)

## Summary

Quantization reduces the numerical precision of model weights and/or activations from 32-bit or 16-bit floats to lower-bit integers (INT8, INT4, even INT2), shrinking model size and speeding up inference. You trade a small amount of model quality for dramatically lower memory requirements and faster matrix multiplications on hardware with integer arithmetic units. Modern techniques minimize quality degradation to near-zero at INT8 and acceptable levels at INT4.

## Key Ideas

- Post-training quantization (PTQ): quantize a trained model without any further gradient updates; fast but lossy at low bits
- Quantization-aware training (QAT): simulate quantization during training to recover quality; expensive but recovers more accuracy
- GPTQ: layer-wise quantization using second-order weight correction; dominant PTQ method for INT4 weight-only quantization
- AWQ (Activation-Aware Weight Quantization): protects salient weights identified by activation magnitude
- QLoRA uses 4-bit base model (NF4 format) with double quantization, enabling fine-tuning of 65B models on one GPU
- Weight-only vs. weight+activation quantization: the latter requires more careful calibration but gives bigger speedups on certain hardware

## Related

- [[lora]]
- [[speculative-decoding]]
- [[flash-attention]]
- [[llama-cpp]]
- [[ollama]]
- [[vllm]]
- [[tensorrt-llm]]
