---
title: Tree of Thoughts
tags: [llm, reasoning, prompting]
created: 2026-05-14
source: https://arxiv.org/pdf/2305.10601.pdf
---

# Tree of Thoughts

## Summary

Tree of Thoughts (ToT) extends chain-of-thought prompting by framing problem-solving as a search over a tree of intermediate reasoning steps. You use it for tasks where backtracking or exploring multiple solution paths is beneficial — the model generates candidate thoughts, evaluates them, and uses search algorithms (BFS, DFS, beam search) to find the best path to an answer. You get substantially better results than linear CoT on planning and creative writing tasks.

## Key Ideas

- Each "thought" is a coherent text chunk that serves as an intermediate step toward solving a problem
- The LLM plays dual roles: thought generator (propose candidates) and evaluator (score/prune paths)
- Search strategy determines exploration: BFS for shallow trees, DFS for deep narrow paths
- Requires many more LLM calls than standard CoT, making it expensive; best reserved for high-stakes tasks
- Demonstrates that deliberate search over language can compensate for single-pass reasoning failures

## Related

- [[chain-of-thought-prompting]]
- [[prompt-engineering]]
- [[llm-agents]]
- [[llm-math-reasoning]]
