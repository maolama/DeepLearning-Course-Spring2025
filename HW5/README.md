# HW5 — Autoencoders and GANs

**Goal:** Learn representations without labels, and generate images.

- **Part 1 – Self-supervised labeling:** train a **convolutional autoencoder** on MNIST and Fashion-MNIST, use the encoder as a feature extractor, and cluster the features with K-Means to generate pseudo-labels (choosing *k* by silhouette score).
- **Part 2 – DCGAN:** implement a generator and discriminator and train them on an image dataset, experimenting with label smoothing and input noise for stability.

Notebooks: [`HW5_Part1_Autoencoder_Clustering.ipynb`](HW5_Part1_Autoencoder_Clustering.ipynb) · [`HW5_Part2_DCGAN.ipynb`](HW5_Part2_DCGAN.ipynb) · Assignment: [`Assignment5.pdf`](Assignment5.pdf)
