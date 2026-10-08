# HW2 — Convolutional Networks and Transfer Learning

**Goal:** Reproduce a CNN from a paper, then compare it with fine-tuning pretrained models.

- **Part 1 – Skin-cancer classification (ISIC / HAM10000):** EDA, rebuilding the CNN architecture from the reference paper, then an improved version with batch normalization and dropout.
- **Part 2 – Transfer learning on a small image dataset:** fine-tune **VGG16** and **ResNet50** with and without data augmentation, following the paper's 500/200 train/validation split. The best fine-tuned model reaches **97% test accuracy**.

Notebooks: [`HW2_Part1_CNN_SkinCancer.ipynb`](HW2_Part1_CNN_SkinCancer.ipynb) · [`HW2_Part2_Transfer_Learning.ipynb`](HW2_Part2_Transfer_Learning.ipynb)
