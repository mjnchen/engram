---
title: TinyZero
url: https://github.com/Jiayi-Pan/TinyZero
maker: Jiayi Pan
tags: [llm, reasoning, research]
created: 2026-05-14
---

# TinyZero

## What it is

Minimal reproduction of DeepSeek R1-Zero by Jiayi Pan that trains small models (3B parameters) with reinforcement learning to develop chain-of-thought reasoning.

## What problem it solves

DeepSeek R1-Zero's training approach was described in a paper but not made easy to reproduce; TinyZero distills it into an accessible codebase that runs on modest hardware.

## Concepts

- [[chain-of-thought-prompting]]
- [[rlhf]]
- [[llm-math-reasoning]]

## Notes

- Based on veRL training framework
- Demonstrates that RL-induced reasoning emergence is not exclusive to very large models
- MIT licensed
