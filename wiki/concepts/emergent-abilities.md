---
title: Emergent Abilities of LLMs
tags: [llm, scaling, research]
created: 2026-05-14
source: https://openreview.net/pdf?id=yzkSU5zdwD
---

# Emergent Abilities of LLMs

## Summary

Emergent abilities are capabilities that appear sharply and unpredictably in large language models once they exceed a certain scale, absent in smaller models of the same family. You cannot predict their onset from extrapolating small-model performance — they appear to arise discontinuously. Examples include multi-step arithmetic, chain-of-thought reasoning, and few-shot learning.

## Key Ideas

- Defined as abilities not present in small models that appear in large ones, not predicted by smooth scaling
- Contrasts with smooth scaling: most benchmarks improve gradually; emergent tasks show flat-then-jump behavior
- The apparent discontinuity may partially be a measurement artifact: metrics with sharp thresholds (exact match) create cliff-like curves even for underlying smooth improvement
- Examples: BIG-Bench tasks, multi-step math, chain-of-thought reasoning, instruction following
- Raises concerns for AI safety: dangerous capabilities could emerge unpredictably as models scale

## Related

- [[scaling-laws]]
- [[chinchilla-scaling-laws]]
- [[chain-of-thought-prompting]]
- [[foundation-models]]
