---
title: LLM Alignment
tags: [llm, alignment, safety]
created: 2026-05-14
source: https://github.com/GaryYufei/AlignLLMHumanSurvey
---

# LLM Alignment

## Summary

LLM alignment is the set of techniques and research directions aimed at making language models behave in accordance with human values and intentions — being helpful, harmless, and honest. You need alignment because models trained purely on next-token prediction learn to reproduce patterns in training data, including harmful, biased, and misleading content. The field spans training methods, evaluation, and theoretical frameworks.

## Key Ideas

- The alignment tax: alignment techniques sometimes reduce benchmark performance while improving safety; the tradeoff is active research
- Key training methods: [[rlhf]], [[dpo]], [[instruction-tuning]] — each trades off complexity, data requirements, and stability
- Constitutional AI (Anthropic): self-critique and revision guided by a written set of principles, reducing reliance on human labelers
- Red teaming: systematic adversarial probing to find failure modes before deployment
- Evaluation is hard: automated metrics don't capture harmlessness well; human evaluation is expensive and inconsistent
- Alignment generalizes beyond text: multimodal models, agents, and code models each have domain-specific alignment challenges

## Related

- [[rlhf]]
- [[dpo]]
- [[instruction-tuning]]
- [[llm-hallucination]]
- [[llm-security]]
- [[llm-agents]]
