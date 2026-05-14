---
title: How does GPT Obtain its Ability? (Yao Fu)
url: https://yaofu.notion.site/How-does-GPT-Obtain-its-Ability-Tracing-Emergent-Abilities-of-Language-Models-to-their-Sources-b9a57ac0fcf74f30a1ab9e3e36fa1dc1
tags: [llm, emergent-abilities, overview]
created: 2026-05-14
---

# How does GPT Obtain its Ability? (Yao Fu)

## Summary

Yao Fu's analysis tracing specific GPT capabilities back to the training stages and data that produced them. The key argument is that emergent abilities are not magical phase transitions but predictable consequences of what data and training signals were provided — you get out what you put in.

## Key Points

- World knowledge comes from pre-training on diverse web text; instruction following comes specifically from SFT on instruction data
- Code data in pre-training is disproportionately responsible for improved reasoning — code has explicit logical structure that generalizes
- RLHF adds safety and stylistic calibration but does not add factual knowledge
- Chain-of-thought ability requires both scale (for the reasoning capability) and instruction tuning (for the format)

## Concepts

- [[emergent-abilities]]
- [[instruction-tuning]]
- [[rlhf]]
- [[chain-of-thought-prompting]]
- [[scaling-laws]]

## Notes
