# 📘 Deep Learning Assignment 6

## Encoder–Decoder Models: With vs Without Attention

👩‍💻 **Student:** Nirjara More
🎓 **PRN:** 202301100049
📚 **Subject:** Deep Learning

---

## 📌 Overview

This assignment focuses on understanding and implementing **Sequence-to-Sequence (Seq2Seq) models** using:

* Encoder–Decoder architecture
* Comparison between:

  * ❌ Without Attention (Baseline)
  * ✅ With Attention (Bahdanau Attention)

The task performed is:

> **Converting English number words into digit format**
> Example: `"twenty three" → "23"`

---

## 🧠 Concepts Covered

* Sequence-to-Sequence Learning
* Encoder–Decoder Architecture
* GRU (Gated Recurrent Unit)
* Attention Mechanism (Bahdanau Attention)
* Teacher Forcing
* BLEU Score Evaluation

---

## 📂 Files in this Assignment

* 📓 Notebook: 
* 🐍 Python Code: `encoder_decoder_assignment_06.py`
* 📄 Report: 

---

## ⚙️ Model Architecture

### 🔹 Encoder

* Embedding Layer
* GRU Layer
* Outputs hidden states for each timestep

### 🔹 Decoder (Without Attention)

* Uses only final encoder hidden state
* Suffers from **information bottleneck**

### 🔹 Decoder (With Attention)

* Uses **Bahdanau Attention**
* Dynamically focuses on relevant input tokens
* Improves performance significantly

---

## 📊 Results Summary

| Metric        | Without Attention | With Attention |
| ------------- | ----------------- | -------------- |
| Accuracy      | 89.2%             | 100%           |
| BLEU Score    | ~89%              | 100%           |
| Training Loss | Higher            | Lower          |
| Context       | Fixed             | Dynamic        |

---

## 🔍 Key Insights

* Attention removes the **fixed context bottleneck**
* Helps capture **long-range dependencies**
* Provides **interpretability through attention weights**
* Improves both **accuracy and learning efficiency**

---

## 📈 Visualizations

* Training Loss Curve
* Performance Comparison Graph
* Attention Heatmaps

---

## 🚀 How to Run

```bash
pip install torch numpy matplotlib
python encoder_decoder_assignment_06.py
```

OR open the notebook in Google Colab and run all cells.

---

## 🌍 Real-World Applications

* Machine Translation
* Text Summarization
* Speech Recognition
* Chatbots & NLP Systems

---

## 📚 References

* Bahdanau et al. (2015) – Neural Machine Translation
* Vaswani et al. (2017) – Attention is All You Need
* IJRAR 2024 – Seq2Seq with Attention

---

## ✅ Conclusion

The experiment clearly shows that **Attention is a crucial improvement** over traditional Encoder–Decoder models.
It enhances performance, interpretability, and scalability in sequence learning tasks.

---

✨ *This assignment demonstrates the practical importance of attention mechanisms in modern deep learning.*

