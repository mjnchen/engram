---
title: Awesome LLM Security
url: https://github.com/corca-ai/awesome-llm-security
tags: [llm, security, safety]
created: 2026-05-14
---

# Awesome LLM Security

## Summary

Collection of tools, papers, and documentation covering the attack surface unique to LLMs: prompt injection, jailbreaking, data extraction, and model theft. The key insight is that LLMs blur the boundary between instructions and data, creating an attack class with no equivalent in traditional software.

## Key Points

- Prompt injection exploits the fact that LLMs cannot reliably distinguish user-supplied data from system instructions
- Jailbreaks often transfer across models because they exploit alignment training weaknesses, not model-specific bugs
- Indirect prompt injection embeds malicious instructions in content retrieved by an agent (web pages, documents)
- Red-teaming LLMs requires both automated and human attack strategies; neither alone is sufficient

## Concepts

- [[llm-security]]
- [[llm-alignment]]
- [[llm-agents]]

## Notes
