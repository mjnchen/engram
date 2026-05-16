---
title: Evaluating AI Agents
url: https://www.deeplearning.ai/short-courses/evaluating-ai-agents/
tags: [llm-evaluation, agents, evals]
created: 2026-05-15
---

# Evaluating AI Agents

## Summary

A cluster of resources on evaluating LLM agents: tool use accuracy, task completion, agentic reasoning, and multi-step behavior. Agent evals are harder than single-turn evals because errors compound across steps.

## Key Points

- Tool use eval: does the agent call the right tool with the right arguments?
- Task completion: did the agent achieve the end goal?
- Agentic reasoning: are intermediate steps sensible?
- T-Eval (ACL 2024) breaks tool use into sub-steps to diagnose where agents fail
- Braintrust recommends scoring intermediate steps, not just final outputs

## Concepts

- [[llm-agents]]
- [[prompt-engineering]]

## Notes

- [Evaluating AI Agents - DeepLearning.AI short course](https://www.deeplearning.ai/short-courses/evaluating-ai-agents/)
- [LLM Agent Evaluation: Tool Use, Task Completion, Agentic Reasoning - Confident AI](https://www.confident-ai.com/blog/llm-agent-evaluation-complete-guide)
- [Evaluating agents - Braintrust blog](https://www.braintrust.dev/blog/evaluating-agents)
- [open-compass/T-Eval: Evaluating Tool Utilization Step by Step (ACL 2024)](https://github.com/open-compass/T-Eval)
- [How to evaluate AI systems/agents? - r/AI_Agents](https://www.reddit.com/r/AI_Agents/comments/1isvh11/how_to_evaluate_ai_systems_agents/)
