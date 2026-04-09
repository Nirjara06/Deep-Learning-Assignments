# Lab Assignment 04 — NLP Pipeline for Text Classification

**Name:** Nirjara More
**PRN:** 202301100049
**Batch:** A1
**Group Members:** Nirjara, Sneha, Vaishnavi, Disha
**Course:** Deep Learning
**Date of Submission:** 09-04-2026

---

## 📌 Overview

This assignment builds a complete **Natural Language Processing (NLP) pipeline from scratch and using libraries**, applied to the **20 Newsgroups Dataset** (`talk.religion.misc` category). The goal is to classify text messages as **Religious** or **General** using various NLP techniques and classification models.

---

## 📂 Dataset

| Property | Details |
|---|---|
| **Name** | 20 Newsgroups Dataset |
| **Category Used** | `talk.religion.misc` |
| **Source** | `sklearn.datasets.fetch_20newsgroups` |
| **Task** | Binary Classification (Religious vs General) |
| **Additional File** | `list.csv` (local label mapping) |

---

## 🔧 NLP Pipeline

### 1. 🧹 Preprocessing — From Scratch
- Manual Tokenizer (lowercasing, punctuation removal)
- Manual Stopword Removal
- Manual Stemmer (suffix stripping)
- Manual Feature Extraction (has_number, has_url, word_count, etc.)

### 2. 📚 Preprocessing — Using Libraries (NLTK)
- NLTK Tokenization
- NLTK Stopword Removal
- Porter Stemmer
- WordNet Lemmatizer with POS tagging

### 3. 🏷️ POS Tagging
- Scratch rule-based POS Tagger
- NLTK POS Tagger
- POS distribution comparison (Religious vs General)

### 4. 🏷️ Named Entity Recognition (NER)
- Scratch NER (rule-based with keyword lists)
- SpaCy NER (`en_core_web_sm`)
- Entity distribution comparison across classes

### 5. 📐 Text Vectorization
- **Word2Vec** (trained from scratch using Gensim, Skip-gram, 100-dim)
- Word similarity & sentence vectors
- Stemming vs Lemmatization comparison

### 6. 🔢 N-Grams
- From scratch N-gram generator
- NLTK `FreqDist` N-grams
- sklearn `CountVectorizer` N-grams
- Top bigrams visualization per class

### 7. 📏 Text Similarity
- Scratch Cosine Similarity
- TF-IDF Cosine Similarity (sklearn)

### 8. 🤖 Classification Models
- **Manual Naive Bayes** (implemented from scratch)
- **sklearn Naive Bayes** (CountVectorizer & TF-IDF)
- **Logistic Regression** (CountVectorizer & TF-IDF)
- **SVM** (CountVectorizer & TF-IDF)
- **Word2Vec + Logistic Regression**

---

## 📊 Evaluation Metrics

- Accuracy
- F1 Score
- Precision & Recall
- Confusion Matrix
- Classification Report

---

## 📊 Visualizations

- Label distribution plots
- Message length & word count distributions
- POS tag comparison bar charts
- NER entity distribution plots
- Top bigrams bar charts
- Training loss/accuracy curves
- Confusion matrices (all models)
- Model comparison bar chart (Accuracy & F1)

---

## 🛠️ Requirements

```bash
pip install numpy pandas matplotlib seaborn scikit-learn nltk gensim spacy
python -m spacy download en_core_web_sm
```

> Run on **Google Colab**. Place `list.csv` in `/content/` before running.

---

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/drive/1ZNqLIMF21-OSQFdnWyq_e7zLy3EsJ4yF#scrollTo=RD2nkvrNjO4T)
2. Upload `list.csv` to `/content/`
3. Run all cells sequentially (`Runtime → Run all`)

---

## 📁 Files

```
├── NirjaraMore_202301100049_Ass04.ipynb   # Main assignment notebook
├── list.csv                               # Label mapping file
└── README.md                              # This file
```

---

## 📝 Declaration

I, Nirjara More, confirm that the work submitted in this assignment is my own and has been completed following academic integrity guidelines.
