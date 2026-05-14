---
title: LLM Wiki Pattern (NicholasSpisak)
url: https://github.com/NicholasSpisak/second-brain/blob/main/docs/llm-wiki.md
tags: [llm, knowledge-management, architecture]
created: 2026-05-14
---

# LLM Wiki Pattern (NicholasSpisak)

## Summary

Design document describing a pattern for using an LLM as a persistent knowledge base maintainer: the LLM reads an inbox of new items, writes structured markdown notes, and maintains wikilink-based cross-references. The pattern turns an LLM from a stateless query-answerer into a stateful knowledge curator.

## Key Points

- Three core operations: ingest (process inbox items into notes), query (retrieve and synthesize across notes), and lint (check for broken links, orphaned notes, inconsistencies)
- Wikilinks (`[[note-name]]`) serve as the knowledge graph — the LLM writes them as cross-references and they can be queried as a graph
- Notes are categorized by type (concept, tool, source, synthesis) to guide retrieval and avoid mixing granularity
- The pattern works best when note types have strict templates — structure compensates for LLM verbosity and inconsistency

## Concepts

- [[llm-agents]]
- [[rag]]

## Notes

This wiki (engram) implements this pattern directly.
