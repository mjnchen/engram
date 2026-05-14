---
title: Axolotl
url: https://github.com/axolotl-ai-cloud/axolotl
maker: Axolotl AI
tags: [llm, training, fine-tuning]
created: 2026-05-14
---

# Axolotl

## What it is

Axolotl is a flexible fine-tuning framework by Axolotl AI that wraps Hugging Face libraries with support for LoRA, QLoRA, and a wide variety of dataset formats via YAML configuration.

## What problem it solves

Fine-tuning LLMs on custom datasets involves juggling many libraries and configuration options; Axolotl consolidates these into a single config-driven interface that handles data loading, PEFT setup, and training loop.

## Concepts

- [[lora]]
- [[instruction-tuning]]
- [[llm-quantization]]

## Notes

Supports full fine-tune, LoRA, QLoRA, and ReLoRA. Configuration is YAML-based, making experiments reproducible. Apache 2.0 license.
