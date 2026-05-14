---
title: DBRX
url: https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm
maker: Databricks
tags: [llm, model, open-weight]
created: 2026-05-14
---

# DBRX

## What it is

Large open-weight sparse mixture-of-experts model from Databricks with 132B total parameters and 36B active parameters per forward pass.

## What problem it solves

Enterprises needed a powerful, open model they could host on their own infrastructure with no data leaving their environment; DBRX delivers frontier-class performance with an open license.

## Concepts

- [[mixture-of-experts]]
- [[foundation-models]]
- [[tensor-parallelism]]

## Notes

- Fine-tuned variant DBRX Instruct available
- Released under Databricks Open Model License
- Requires significant GPU memory (multi-GPU for inference)
