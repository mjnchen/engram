---
title: torchtune
url: https://github.com/pytorch/torchtune
maker: PyTorch
tags: [llm, training, fine-tuning]
created: 2026-05-14
---

# torchtune

## What it is

torchtune is a native PyTorch library by the PyTorch team for fine-tuning LLMs using a modular, recipe-based design with no framework dependencies beyond PyTorch itself.

## What problem it solves

Fine-tuning frameworks often add layers of abstraction that obscure what is happening; torchtune keeps the training loop in plain PyTorch so practitioners can read, modify, and trust every step.

## Concepts

- [[lora]]
- [[instruction-tuning]]
- [[flash-attention]]

## Notes

Recipes are standalone Python scripts. Supports full fine-tune, LoRA, and QLoRA. BSD 3-Clause license.
