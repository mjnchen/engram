---
title: BERT
tags: [llm, architecture, training]
created: 2026-05-14
source: https://aclanthology.org/N19-1423.pdf
---

# BERT

## Summary

BERT (Bidirectional Encoder Representations from Transformers) is a pretrained Transformer encoder that uses masked language modeling and next-sentence prediction to learn bidirectional context. You fine-tune it on downstream classification, QA, and NER tasks by adding a task head on top of the pretrained representations. You can credit it with establishing the pretraining + fine-tuning paradigm that dominated NLP before instruction-tuned generative models.

## Key Ideas

- Masked Language Model (MLM): 15% of tokens are masked; the model predicts them using both left and right context
- Bidirectional context distinguishes BERT from autoregressive models like GPT, which can only attend to prior tokens
- Next-sentence prediction (NSP) was included for sentence-pair tasks; later ablations showed it adds little value
- Fine-tuning on downstream tasks is inexpensive: add a linear head, fine-tune the whole model for a few epochs
- RoBERTa and DeBERTa improved on BERT by removing NSP, training longer, and using dynamic masking

## Related

- [[transformer]]
- [[t5]]
- [[foundation-models]]
- [[instruction-tuning]]
