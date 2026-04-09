# Lab Assignment 02 — Pretrained Model Implementation (EfficientNet / MobileNetV2)

**Name:** Nirjara More
**PRN:** 202301100049
**Batch:** A1
**Course:** Deep Learning

---

## 📌 Overview

This assignment implements **transfer learning** inspired by the research paper **"EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks"** (Tan & Le). A **MobileNetV2** pretrained on ImageNet is fine-tuned on the **Rice Leaf Disease Dataset** to classify rice plant diseases.

---

## 📄 Reference Paper

| Field | Details |
|---|---|
| **Title** | EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks |
| **Authors** | Mingxing Tan, Quoc V. Le |
| **Key Idea** | Compound scaling of depth, width, and resolution for efficient CNNs |

---

## 📂 Dataset

| Property | Details |
|---|---|
| **Name** | Rice Leaf Disease Dataset |
| **Source** | [Kaggle](https://www.kaggle.com/datasets/vbookshelf/rice-leaf-diseases) |
| **Format** | Image folders per class |
| **Split** | 80% Train / 20% Validation |
| **Image Size** | 224 × 224 |
| **Batch Size** | 32 |

---

## 🧠 Model Architecture

```
Input (224×224×3)
        ↓
MobileNetV2 (pretrained on ImageNet) — Frozen Base
        ↓
Global Average Pooling
        ↓
Dense + Dropout
        ↓
Softmax Output (N classes)
```

- **Base Model:** MobileNetV2 (weights = ImageNet, top excluded)
- **Base Layers:** Frozen (used as feature extractor)
- **Optimizer:** Adam (lr = 0.00001)
- **Loss:** Categorical Cross-Entropy
- **Epochs:** 8

---

## 📋 Tasks Covered

| Task | Description |
|---|---|
| **Task 1** | Research paper selection, dataset preparation & visualization |
| **Task 2** | Model implementation, feature map visualization, fine-tuning |
| **Task 3** | Evaluation — Accuracy, Precision, Recall, F1-Score, Confusion Matrix |

---

## 📊 Results

| Metric | Our Model (MobileNetV2) | EfficientNet Paper (ImageNet) |
|---|---|---|
| Accuracy | ~46–53% (validation) | ~97%+ |
| Precision (macro) | 0.50 | Higher |
| Recall (macro) | 0.46 | Higher |
| F1-Score (macro) | 0.44 | Higher |

> The gap is expected — the original paper trains on ImageNet (1000 classes, millions of images), while this implementation uses a small domain-specific dataset with limited samples.

---

## 📊 Visualizations

- Sample images from each disease class
- Original vs preprocessed image comparison
- Feature maps from first 4 convolutional layers
- Training & Validation Accuracy/Loss curves
- Confusion Matrix
- Classification Report

---

## 🛠️ Requirements

```bash
pip install tensorflow scikit-learn matplotlib numpy
```

> This notebook is designed for **Google Colab**. Upload `RiceLeafDiseasesDataset.zip` to `/content/` before running.

---

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/drive/1B8_T64ruuO8BgDc3se3csVqk3Gbs88o0#scrollTo=SHIWMSYKbLMk)
2. Upload `RiceLeafDiseasesDataset.zip` to `/content/`
3. Run all cells sequentially (`Runtime → Run all`)

---

## 📝 Declaration

This work was completed by Nirjara More following academic integrity guidelines.
