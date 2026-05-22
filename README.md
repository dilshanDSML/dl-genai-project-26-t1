# DL Project - Messy Mashup Music Genre Classification

This project focuses on **Music Genre Classification** in challenging noisy conditions as part of the Messy Mashup competition.

---

## 📋 Project Overview

The goal of this project is to classify music into **10 different genres** from audio files that are:
- Mixed from different songs (mashups)
- Rhythmically synchronized with tempo changes
- Mixed with background noise

This is a difficult task because the training data (clean stems) and test data (noisy mashups) have very different distributions.

---

## 🎵 Genres

- Blues, Classical, Country, Disco, Hiphop, Jazz, Metal, Pop, Reggae, Rock

---

## 🛠️ Tools & Libraries Used

- **Python**
- **NumPy** & **Pandas** — Data handling
- **Librosa** — Audio processing and feature extraction
- **Scikit-learn** — Evaluation metrics and preprocessing
- **PyTorch** — Deep Learning framework
- **Torchaudio** — Audio handling with PyTorch

---

## 🧠 Models Implemented

I experimented with three different deep learning approaches:

1. **CNN (Convolutional Neural Network) from scratch**  
   — Built a custom 2D CNN model using Mel Spectrograms

2. **CRNN (Convolutional Recurrent Neural Network)**  
   — Combined CNN + LSTM/GRU to capture both spatial and temporal patterns in audio

3. **AST (Audio Spectrogram Transformer)**  
   — Used a transformer-based model pre-trained on audio data for better performance
   --- got the best result by using AST, i got approx 0.91 on test data

---

## 📊 Evaluation Metric

**Macro F1 Score** (averaged across all 10 genres)

---

## 📁 Dataset

- `genres_stems/` → Clean instrument stems (drums, vocals, bass, others)
- `ESC-50-master/` → Noise samples for augmentation
- `mashups/` → Noisy test files (3020 samples)

---

