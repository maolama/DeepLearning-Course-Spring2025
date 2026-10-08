# HW4 — Transformers: BERT for Persian QA and GPT-2 Fine-Tuning

**Goal:** Fine-tune pretrained transformers for an extractive task and a generative-model task.

- **Part 1 – Persian extractive question answering:** fine-tune **ParsBERT** on **PQuAD**, using a sliding window for long contexts (and comparing its tokenizer with ALBERT-fa). Reaches **EM 56.9 / F1 63.8**, compared against the results in the PQuAD paper.
- **Part 2 – GPT-2:** questions on GPT vs. BERT architecture, then fine-tuning GPT-2 for IMDB sentiment classification with a custom perplexity/early-stopping callback. Fine-tuning only the last layers gives **F1 0.90**, and LoRA improves it to **F1 0.93**.

Notebooks: [`HW4_Part1_ParsBERT_QA.ipynb`](HW4_Part1_ParsBERT_QA.ipynb) · [`HW4_Part2_GPT2_Finetuning.ipynb`](HW4_Part2_GPT2_Finetuning.ipynb) · Assignment: [`Assignment4.pdf`](Assignment4.pdf)
