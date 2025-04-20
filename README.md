# Sentiment-analysis
Fine-tuned BERT model for 5-class emotion classification on a custom dataset using Hugging Face Transformers.


# 🧠 BERT Emotion Classifier

This repository contains a fine-tuned [BERT-base-uncased](https://huggingface.co/bert-base-uncased) model for **multi-class emotion classification**. The model is trained using the [Hugging Face Transformers](https://github.com/huggingface/transformers) library on a 5-class emotion dataset.

> **Emotions supported**: `joy`, `sadness`, `fear`, `anger`, `neutral`

---

## 📁 Dataset

The dataset used is a CSV file with two columns:
- `Text`: The input sentence or phrase
- `Emotion`: The target emotion label (string)

📎 Dataset source: [Kaggle - Emotion Dataset by Yash Gupta](https://www.kaggle.com/datasets/yashgupta1161/emotion-dataset)

---

## 🚀 Features

- Fine-tunes BERT on a custom emotion dataset
- Supports 5 emotion categories
- Built with Hugging Face `Trainer` API
- Logs metrics: Accuracy & Weighted F1
- Inference pipeline using `transformers.pipeline`
- Saves model and tokenizer for easy reuse

---

## 🛠 Installation

Install the required dependencies:

```bash
pip install transformers datasets accelerate huggingface_hub
