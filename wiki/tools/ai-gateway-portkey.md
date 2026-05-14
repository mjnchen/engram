---
title: AI Gateway (Portkey)
url: https://github.com/Portkey-AI/gateway
maker: Portkey AI
tags: [llm, infrastructure, tooling]
created: 2026-05-14
---

# AI Gateway (Portkey)

## What it is

AI Gateway by Portkey AI is a unified API gateway that routes LLM requests across 200+ providers (OpenAI, Anthropic, Cohere, etc.) with caching, retries, fallbacks, and observability.

## What problem it solves

Applications relying on a single LLM provider are vulnerable to outages and rate limits, and switching providers requires code changes; the gateway provides a single OpenAI-compatible endpoint with automatic fallback routing and cost tracking.

## Concepts

- [[llm-agents]]
- [[prompt-engineering]]

## Notes

Supports load balancing, semantic caching, and request logging. Available as open-source self-hosted or managed cloud. MIT license.
