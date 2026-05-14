---
title: Datatrove
url: https://github.com/huggingface/datatrove
maker: Hugging Face
tags: [llm, data, training]
created: 2026-05-14
---

# Datatrove

## What it is

Datatrove is a platform-agnostic large-scale data processing pipeline library by Hugging Face for preparing pre-training datasets for LLMs.

## What problem it solves

Curating web-scale pre-training corpora (deduplication, quality filtering, language detection) requires distributed processing infrastructure that is painful to build from scratch; Datatrove provides composable pipeline blocks that run locally or on SLURM/cloud.

## Concepts

- [[foundation-models]]
- [[bpe-tokenization]]

## Notes

Used to process FineWeb and other public Hugging Face datasets. Executor-agnostic: same pipeline code runs locally or distributed. Apache 2.0 license.
