# 💬 Toxic Comment Classification using BERT

This project classifies toxic comments using a fine-tuned BERT model with an accuracy of over **95%**. It integrates unlabeled data from the [Jigsaw Toxic Comment Classification Challenge](https://www.kaggle.com/competitions/jigsaw-unintended-bias-in-toxicity-classification) and utilizes a custom API wrapper named `isomina` for training orchestration and evaluation.

---

## 🧠 Model

- Base: `bert-base-uncased`
- Fine-tuned on labeled and pseudo-labeled Jigsaw dataset
- Multi-label classification (`toxic`, `severe_toxic`, `obscene`, `threat`, `insult`, `identity_hate`)
- Trained using custom `isomina` API wrapper for streamlined experimentation and deployment

---

## 📊 Output Examples

| Visualization of Predictions | |
|-----------------------------|--|
| ![output1](assets/output1.png) | ![output2](assets/output2.png) |

---

## 🚀 Features

- >95% validation accuracy
- Semi-supervised training using pseudo-labeling
- BERT fine-tuning pipeline
- Easy experimentation with `isomina` API
- Robust evaluation with ROC AUC, F1, and accuracy metrics

---

## 📁 Dataset

- [Jigsaw Unintended Bias in Toxicity Classification](https://www.kaggle.com/competitions/jigsaw-unintended-bias-in-toxicity-classification)
- Includes labeled and unlabeled data for semi-supervised learning
- Data loading and pre-processing handled in `data_loader.py`

---

## 🔧 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/toxic-comment-bert.git
cd toxic-comment-bert
