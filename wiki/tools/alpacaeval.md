---
title: AlpacaEval
url: https://tatsu-lab.github.io/alpaca_eval/
maker: Stanford / Tatsu Lab
tags: [llm, evaluation, benchmark]
created: 2026-05-14
---

# AlpacaEval

## What it is

Automatic evaluation framework from Stanford Tatsu Lab that uses GPT-4 as a judge to score instruction-following quality relative to a reference model.

## What problem it solves

Human evaluation of instruction-following is expensive and slow; AlpacaEval provides a cheap, fast proxy that correlates well with human preferences on the AlpacaFarm dataset.

## Concepts

- [[instruction-tuning]]
- [[rlhf]]
- [[prompt-engineering]]

## Notes

- win-rate against text-davinci-003 is the primary metric
- AlpacaEval 2.0 uses length-controlled win rates to reduce verbosity bias
- Open-source; evaluator model is configurable
