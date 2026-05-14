# Engram Repo Seed Design

**Date:** 2026-05-14  
**Type:** One-time seed operation  
**Status:** Approved

## Goal

Populate the engram wiki with an initial set of AI/LLM concept, tool, and source notes by importing and distilling content from two public GitHub repos.

## Sources

| Repo | Content type | URL |
|---|---|---|
| `Hannibal046/Awesome-LLM` | Curated list of papers, tools, frameworks | https://github.com/Hannibal046/Awesome-LLM |
| `NicholasSpisak/second-brain` | Personal wiki (concepts, sources, synthesis) | https://github.com/NicholasSpisak/second-brain |

## Fetch Strategy

Both repos are fetched via raw GitHub content in-session — no cloning required. For Awesome-LLM, fetch the main README. For second-brain, walk the `wiki/` subdirectories and fetch individual markdown files.

## Processing Rules

### From Awesome-LLM
- Techniques and papers (CoT, RLHF, RAG, LoRA, etc.) → `wiki/concepts/`
- Frameworks, libraries, services (LangChain, vLLM, llama.cpp, etc.) → `wiki/tools/`
- Surveys and blog posts → `wiki/sources/`
- Skip: dead links, citation-only entries with no useful summary, non-AI-LLM content

### From NicholasSpisak/second-brain
- Filter to AI/LLM topics only
- Map their structure directly: concepts → `wiki/concepts/`, sources → `wiki/sources/`, synthesis → `wiki/synthesis/`
- Adapt prose to engram style: second person, scannable, no filler phrases
- Skip anything already covered by Awesome-LLM

### Deduplication
If both sources cover the same concept or tool, produce one note. Take the best summary from either source; preserve all links.

## Output

- Notes written directly into `wiki/concepts/`, `wiki/tools/`, `wiki/sources/`, `wiki/synthesis/` — no inbox step
- `CLAUDE.md` updated with a "Seeding from external repos" section documenting the pattern for future use
- `index.md` log appended: `- 2026-05-14: seeded N notes from Awesome-LLM + NicholasSpisak/second-brain`

## Repeating This Pattern

To seed from additional repos in the future:
1. Identify the repo and its structure
2. Fetch raw content (README or individual files)
3. Filter to AI/LLM topics
4. Map each item to concept/tool/source note type using the templates in `_templates/`
5. Deduplicate against existing wiki notes before writing
6. Update `index.md` log
