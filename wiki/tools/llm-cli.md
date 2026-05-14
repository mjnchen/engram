---
title: LLM CLI (Simon Willison)
url: https://github.com/simonw/llm
maker: Simon Willison
tags: [llm, tooling, local]
created: 2026-05-14
---

# LLM CLI (Simon Willison)

## What it is

Command-line tool and Python library by Simon Willison for interacting with any LLM via a unified, plugin-based interface.

## What problem it solves

Each LLM provider has its own SDK and CLI; `llm` provides a single command that works across OpenAI, Anthropic, local models (via Ollama), and many others through a plugin system.

## Concepts

- [[prompt-engineering]]
- [[foundation-models]]

## Notes

- Plugin ecosystem covers 30+ model providers
- Supports embeddings, chat history, and template management
- Apache 2.0 licensed; installable via pip or Homebrew
