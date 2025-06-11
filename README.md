# Multimodal Fake News Detection 📰🧠

This project focuses on **fake news detection using multimodal learning** — combining textual and visual information (text + image) to improve the accuracy of detecting misleading or fake content.

## 📌 Project Description

Fake news spreads rapidly through social media, often leveraging emotionally charged text and misleading images. This project uses both **textual data** (article/title) and **visual data** (associated images) to train deep learning models for detecting fake news more effectively than unimodal approaches.

## 🔍 Dataset

We use the **[Mirage-News dataset](https://huggingface.co/datasets/anson-huang/mirage-news)**:
- Contains real and fake news samples.
- Each sample includes:
  - `text`: News content or title.
  - `image`: Corresponding news image.
  - `label`: Ground truth (fake or real).

## 🧠 Models Implemented

- ✅ **CNN (Text-only)**
- ✅ **CNN (Text + Image)**
- ✅ **BERT + CNN (Text + Image)**
- ✅ **BiLSTM (Text-only)**
- ✅ **ResNet + BERT (Multimodal)**

## 🛠 Tech Stack

- **Python**
- **PyTorch**
- **Transformers (Hugging Face)**
- **TorchVision** (for image encoders like ResNet/VGG)
- **scikit-learn**
- **matplotlib / seaborn** (for plots & confusion matrices)

## 🧪 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## 🔐 Secrets Management

The Hugging Face API token is **stored securely in a `.env` file** (not tracked by Git).  
**Ensure you create your `.env` with:**

```env
HF_TOKEN=your_huggingface_token_here
