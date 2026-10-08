# Final Project — Instruction Fine-Tuning and Image Captioning

Assignment: [`Final_Project.pdf`](Final_Project.pdf)

## Q1 — Instruction fine-tuning of an LLM
Fine-tune **Gemma-2-2B-IT** on **SlimOrca** using only Hugging Face Transformers + PEFT (no ready-made fine-tuning pipelines). Three methods are compared:

| Method | Trainable parameters |
|---|---|
| Soft prompt (prompt tuning) | 46K (0.002%) |
| LoRA | 41.5M (1.6%) |
| Traditional fine-tuning (first and last two layers unfrozen) | 746M (28.5%) |

The notebook compares loss curves and generation quality before and after fine-tuning, and discusses why a lower loss does not always mean better outputs.

Notebook: [`Q1_Instruction_Finetuning.ipynb`](Q1_Instruction_Finetuning.ipynb)

## Q2 — Image captioning on Flickr8k (PyTorch)
Three encoder–decoder models built from scratch:
1. **CNN–RNN baseline:** a pretrained CNN encoder with an LSTM decoder.
2. **CNN + attention:** spatial features with an attention-based decoder, plus attention-heatmap visualization.
3. **Transformer decoder:** a WordPiece tokenizer, positional encoding and a transformer decoder over image features.

| Model | BLEU-1 | BLEU-2 | BLEU-3 |
|---|---|---|---|
| CNN–RNN | 0.55 | 0.29 | 0.09 |
| CNN + Attention | **0.64** | **0.41** | **0.16** |
| Transformer | 0.59 | 0.30 | 0.09 |

The attention model performs best. The complete evaluation is in the base-model notebook: BLEU-1 to BLEU-4 with smoothing, plus a qualitative comparison and error analysis of all three models.

Notebooks: [`Q2_Captioning_Base_and_Evaluation.ipynb`](Q2_Captioning_Base_and_Evaluation.ipynb) · [`Q2_Captioning_Attention.ipynb`](Q2_Captioning_Attention.ipynb) · [`Q2_Captioning_Transformer.ipynb`](Q2_Captioning_Transformer.ipynb)
