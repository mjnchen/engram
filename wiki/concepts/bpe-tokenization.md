---
title: BPE Tokenization
tags: [llm, training, tokenization]
created: 2026-05-14
source: https://www.youtube.com/watch?v=zduSFxRajkE&t=1157s
---

# BPE Tokenization

## Summary

Byte Pair Encoding (BPE) is the dominant tokenization algorithm for LLMs, building a vocabulary of subword units by iteratively merging the most frequent adjacent byte pairs in a corpus. You use it to represent any text as a sequence of tokens that balances vocabulary size against sequence length — common words become single tokens while rare words split into meaningful subwords. GPT-2, GPT-4, and LLaMA all use BPE variants.

## Key Ideas

- Training: count all byte pairs in the corpus, merge the most frequent pair into a new symbol, repeat until vocab size is reached
- At inference, a trie-based algorithm greedily applies learned merges to new text
- Vocabulary size is a hyperparameter (typically 32K–128K); larger vocab = shorter sequences but sparser embeddings
- BPE is byte-level in GPT-2 and descendants: every byte is a base token, ensuring any UTF-8 text is representable
- Tokenization affects model behavior: numbers, non-Latin scripts, code, and whitespace are tokenized inconsistently
- SentencePiece (used in LLaMA, T5) uses a different algorithm (unigram LM) but achieves similar subword splitting

## Related

- [[transformer]]
- [[bert]]
- [[t5]]
- [[llm-math-reasoning]]
