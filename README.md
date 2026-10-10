# Neural Networks and Deep Learning — M.Sc. Coursework (Spring 2025)

Solutions to the graduate **Neural Networks and Deep Learning** course at the **Tehran Institute for Advanced Studies (TEIAS)**, taught by Dr. Behnam Bahrak, Spring 2025 (Iranian year 1403–1404).
Group work by **Mohammad Ali Olama** and **Erfan Ahmadi**.

The course runs from MLPs to CNNs, recurrent networks, transformers, generative models and LLM fine-tuning. The work uses TensorFlow/Keras, PyTorch and Hugging Face (Transformers, PEFT).

## Final Project
**[Final_Project/](Final_Project/)**
- **Instruction fine-tuning of Gemma-2-2B-IT on SlimOrca:** prompt tuning vs. LoRA vs. traditional fine-tuning, implemented with Transformers + PEFT only.
- **Image captioning on Flickr8k:** CNN–RNN, CNN + attention (with attention heatmaps) and a transformer decoder, all built from scratch in PyTorch. Attention performs best (BLEU-1 0.64, BLEU-2 0.41).

## Assignments
| # | Topic | Highlights |
|---|-------|-----------|
| [HW1](HW1/) | MLPs and training dynamics | Fashion-MNIST: optimizers, learning rate, width and depth; Adaline from scratch |
| [HW2](HW2/) | CNNs and transfer learning | Paper-reproduction CNN for skin-cancer images; VGG16/ResNet50 fine-tuning with augmentation (97% test accuracy) |
| [HW3](HW3/) | RNNs for time series and text | Oil-price forecasting with RNN/LSTM/Bi-LSTM/GRU (GRU best, R² 0.93) vs. ARIMA; tweet classification with Word2Vec vs. FastText embeddings (accuracy 0.88) |
| [HW4](HW4/) | Transformers | ParsBERT extractive QA on Persian PQuAD (F1 63.8); GPT-2 fine-tuning on IMDB, partial vs. LoRA (F1 0.90 → 0.93) |
| [HW5](HW5/) | Autoencoders and GANs | Convolutional-autoencoder features + K-Means pseudo-labeling; DCGAN with stabilization tricks |

## Notes
- The notebooks were run on Google Colab, Kaggle or a GPU server, and paths point to those environments. Datasets are not included; they are public (Fashion-MNIST, ISIC, PQuAD, IMDB, SlimOrca, Flickr8k) or were provided by the course.
- API tokens have been removed. Set your own Hugging Face token where `YOUR_HF_TOKEN` appears.
