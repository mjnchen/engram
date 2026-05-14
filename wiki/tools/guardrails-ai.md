---
title: Guardrails.ai
url: https://www.guardrailsai.com/docs/
maker: Guardrails AI
tags: [llm, safety, inference]
created: 2026-05-14
---

# Guardrails.ai

## What it is

Guardrails.ai is an output validation library by Guardrails AI that enforces structure, type safety, and custom assertions on LLM-generated text, with automatic retry on failure.

## What problem it solves

LLM outputs are non-deterministic and may fail schema constraints or business rules; Guardrails wraps model calls with validators that detect failures and trigger re-prompting to correct them.

## Concepts

- [[llm-hallucination]]
- [[llm-security]]
- [[prompt-engineering]]

## Notes

Validators are composable and community-contributed. Supports async and streaming. Apache 2.0 license.
