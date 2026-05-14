---
title: LLM Security
tags: [llm, safety, security]
created: 2026-05-14
source: https://github.com/corca-ai/awesome-llm-security
---

# LLM Security

## Summary

LLM security covers the attack surfaces and defenses specific to deploying language models in applications. You face threats that don't exist in traditional software: models can be manipulated through their input, and their outputs can be weaponized. The field is rapidly evolving as LLM-powered applications become production infrastructure.

## Key Ideas

- Prompt injection: malicious content in user input or retrieved documents overrides the system prompt, hijacking model behavior
- Jailbreaking: crafted inputs bypass safety training to produce harmful outputs (e.g., DAN prompts, many-shot jailbreaking)
- Data poisoning: adversarial examples in training data influence model behavior at inference time
- Model extraction: repeated querying allows reconstruction of proprietary model weights or training data
- Indirect prompt injection: attacks embedded in external content (web pages, PDFs) that the model retrieves and processes
- Defenses: input filtering, output monitoring, [[guardrails-ai]], privilege separation between retrieval and generation

## Related

- [[llm-alignment]]
- [[prompt-engineering]]
- [[llm-hallucination]]
- [[llm-agents]]
- [[guardrails-ai]]
