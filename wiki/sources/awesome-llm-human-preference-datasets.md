---
title: Awesome LLM Human Preference Datasets
url: https://github.com/PolisAI/awesome-llm-human-preference-datasets
tags: [llm, alignment, data]
created: 2026-05-14
---

# Awesome LLM Human Preference Datasets

## Summary

Curated list of datasets containing human preference labels — the raw material for RLHF and DPO training. The collection reveals that preference data is sparse, expensive, and domain-specific: there is no universal preference dataset, and different datasets optimize for different values (helpfulness, harmlessness, honesty).

## Key Points

- Preference data formats vary: pairwise comparisons (A vs. B), ranked lists, and scalar ratings — each has different statistical properties for reward model training
- Anthropic HH-RLHF covers helpfulness and harmlessness separately, making it possible to study the tension between the two
- OpenAssistant dataset is multilingual and covers conversation trees rather than single-turn preferences, enabling multi-turn RLHF
- Synthetic preference data (using a stronger model to judge) scales more cheaply but can inherit the judge model's biases

## Concepts

- [[rlhf]]
- [[dpo]]
- [[llm-alignment]]
- [[instruction-tuning]]

## Notes
