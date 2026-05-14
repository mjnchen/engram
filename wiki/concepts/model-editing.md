---
title: Model Editing
tags: [llm, research, training]
created: 2026-05-14
source: https://github.com/zjunlp/ModelEditingPapers
---

# Model Editing

## Summary

Model editing updates specific factual knowledge stored in a pretrained LLM without retraining from scratch or degrading other capabilities. You use it to correct outdated facts, remove harmful content, or inject new information into a deployed model. The core challenge is making targeted edits that generalize to paraphrases of the edited fact while leaving unrelated knowledge intact.

## Key Ideas

- Locate-and-edit methods (ROME, MEMIT): identify which MLP layers store specific facts via causal tracing, then directly modify those weights
- Meta-learning methods (MEND, KE): train a hypernetwork that predicts weight updates from an (input, target) pair
- Key properties to evaluate: efficacy (edit succeeds), generalization (paraphrases work), specificity (unrelated facts unchanged)
- Editing thousands of facts simultaneously degrades model quality; large-scale editing remains an open problem
- Alternative: [[rag]] avoids editing weights altogether by externalizing knowledge to a retrieval index

## Related

- [[rag]]
- [[llm-hallucination]]
- [[lora]]
- [[easyedit]]
