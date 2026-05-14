---
title: LLM Hallucination
tags: [llm, alignment, safety]
created: 2026-05-14
source: https://github.com/LuckyyySTA/Awesome-LLM-hallucination
---

# LLM Hallucination

## Summary

Hallucination refers to LLM outputs that are fluent and confident but factually wrong, fabricated, or inconsistent with the provided context. You encounter two main types: intrinsic hallucination (contradicts source material) and extrinsic hallucination (adds information not in the source). It is one of the primary barriers to deploying LLMs in high-stakes domains.

## Key Ideas

- Caused by gaps between training data distribution and inference-time queries; models interpolate or extrapolate from patterns
- Common manifestations: fake citations, wrong dates/numbers, invented entities, inconsistent reasoning chains
- Detection approaches: self-consistency sampling (agreement across multiple generations), factual verification against external sources
- Mitigation: [[rag]] grounds outputs in retrieved documents; [[rlhf]] can reduce but not eliminate hallucination
- Calibration is correlated: models that assign lower confidence to uncertain outputs tend to hallucinate less
- Evaluation benchmarks: TruthfulQA, HaluEval, FActScoring

## Related

- [[rag]]
- [[llm-alignment]]
- [[model-editing]]
- [[prompt-engineering]]
- [[ragas]]
