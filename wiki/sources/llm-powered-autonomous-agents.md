---
title: LLM Powered Autonomous Agents (Lilian Weng)
url: https://lilianweng.github.io/posts/2023-06-23-agent/
tags: [llm, agents, overview]
created: 2026-05-14
---

# LLM Powered Autonomous Agents (Lilian Weng)

## Summary

Lilian Weng's comprehensive breakdown of LLM agent architectures, decomposing them into three components: planning (task decomposition), memory (in-context, external, parametric), and tools (APIs, calculators, search). The framework is still the standard mental model for thinking about agent design.

## Key Points

- Planning strategies include task decomposition (Chain-of-Thought, Tree-of-Thoughts) and self-reflection (ReAct, Reflexion)
- Memory types: in-context (prompt), external (vector DB), and parametric (model weights) — each has different update cost and capacity
- Tool use requires the model to generate structured calls and parse results — few-shot demonstrations significantly improve reliability
- Agent reliability degrades exponentially with task length because each step compounds errors

## Concepts

- [[llm-agents]]
- [[chain-of-thought-prompting]]
- [[tree-of-thoughts]]
- [[rag]]
- [[prompt-engineering]]

## Notes
