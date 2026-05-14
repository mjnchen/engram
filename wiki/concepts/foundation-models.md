---
title: Foundation Models
tags: [llm, research, overview]
created: 2026-05-14
source: https://arxiv.org/pdf/2108.07258.pdf
---

# Foundation Models

## Summary

Foundation models are large neural networks trained on broad data at scale that can be adapted to a wide range of downstream tasks. You can think of them as general-purpose bases that specialize via fine-tuning, prompting, or retrieval rather than training task-specific models from scratch. The term was coined by the Stanford HAI group to describe models like GPT-3, BERT, and CLIP.

## Key Ideas

- Trained via self-supervised learning on massive corpora; task-specific supervision is applied only during adaptation
- Exhibit emergent capabilities that weren't explicitly trained: translation, code generation, reasoning
- Enable paradigm shift: one model → many applications, rather than one model per task
- Raise societal concerns: homogenization of AI (single model failure propagates widely), bias amplification at scale, compute concentration
- Multimodal foundation models (CLIP, Flamingo, GPT-4V) extend the pattern beyond text to images, audio, video

## Related

- [[scaling-laws]]
- [[emergent-abilities]]
- [[instruction-tuning]]
- [[rlhf]]
- [[bert]]
- [[t5]]
- [[transformer]]
