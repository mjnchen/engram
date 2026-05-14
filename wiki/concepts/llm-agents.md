---
title: LLM Agents
tags: [llm, agents, reasoning]
created: 2026-05-14
source: https://lilianweng.github.io/posts/2023-06-23-agent/
---

# LLM Agents

## Summary

An LLM agent uses a language model as the core reasoning engine, augmented with tools, memory, and a planning loop to autonomously complete multi-step tasks. You give the agent access to external APIs, code execution, web search, or databases, and it decides which tools to call and in what order to achieve a goal. This extends LLMs from single-turn Q&A to long-horizon task execution.

## Key Ideas

- Core components: Planning (task decomposition, reflection), Memory (in-context, external vector store, parameter), Tools (APIs, search, code interpreter)
- ReAct: interleaves reasoning traces and tool-call actions in a single sequence; the model thinks and acts in alternating steps
- Reflection and self-critique loops allow agents to detect and correct errors without human intervention
- Multi-agent systems: specialized agents collaborate and delegate; improves on single-agent for complex tasks
- Key failure modes: compounding errors, infinite loops, context length overflow, poor tool selection
- Memory management is a bottleneck: long tasks exceed context windows; retrieval-based memory is the primary workaround

## Related

- [[chain-of-thought-prompting]]
- [[tree-of-thoughts]]
- [[rag]]
- [[llm-alignment]]
- [[prompt-engineering]]
- [[langchain]]
- [[llamaindex]]
- [[dspy]]
- [[semantic-kernel]]
