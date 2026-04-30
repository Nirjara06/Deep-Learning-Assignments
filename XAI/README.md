# 📘 Deep Learning Assignment 6

## Explainable AI (XAI): Enhancing Transparency in Machine Learning

👩‍💻 **Student:** Nirjara More
🎓 **PRN:** 202301100049
📚 **Subject:** Deep Learning

---

## 📌 Overview

This assignment focuses on **Explainable Artificial Intelligence (XAI)** — a crucial area in modern machine learning that improves model transparency, interpretability, and trust.

Traditional models often behave like **black boxes**, making decisions without clear reasoning. This assignment explores techniques to make these decisions understandable.

---

## 🎯 Objectives

* Understand the importance of interpretability in AI
* Apply XAI techniques to analyze model predictions
* Visualize feature contributions and decision behavior
* Study the trade-off between accuracy and explainability

---

## 📂 Files in this Assignment

* 📓 Notebook: 
* 📄 Report: XAI_Report_202301100049.pdf

---

## 📊 Dataset Used

* **Breast Cancer Wisconsin Dataset**

  * 569 samples
  * 30 numerical features
  * Binary classification:

    * Malignant (0)
    * Benign (1)

This dataset is widely used for medical classification tasks and helps demonstrate real-world applicability of XAI.

---

## ⚙️ Model Used

* **Random Forest Classifier**

  * Ensemble of decision trees
  * Reduces overfitting
  * Provides built-in feature importance
  * Works efficiently with SHAP

---

## 🧠 XAI Techniques Applied

### 🔹 1. Feature Importance

* Identifies most influential features globally
* Helps understand overall model behavior

### 🔹 2. SHAP (SHapley Additive Explanations)

* Based on game theory
* Provides:

  * Global explanations (feature impact)
  * Local explanations (individual predictions)
* Highly reliable and consistent

### 🔹 3. LIME (Local Interpretable Model-Agnostic Explanations)

* Explains individual predictions
* Uses simple local models
* Easy to interpret

---

## 📈 Visualizations Included

* Class distribution plots
* Feature distributions
* Correlation heatmap
* SHAP summary plots
* SHAP dependence plots
* Feature importance comparison
* LIME explanations
* Attention-style explanation plots

---

## 📊 Results Summary

* ✅ **Accuracy:** >97%
* ✅ **ROC-AUC:** >0.99
* ✅ **Stable cross-validation performance**

### 🔍 Key Insights:

* Features like **worst perimeter, worst concave points, mean concave points** are most important
* SHAP provides more reliable feature importance than traditional methods
* LIME helps explain individual predictions clearly

---

## ⚠️ Limitations

* LIME explanations may vary (stochastic nature)
* SHAP assumes some feature independence
* Dataset size is relatively small
* Correlated features can affect interpretation

---

## 🚀 How to Run

```bash id="xai123"
pip install numpy pandas matplotlib scikit-learn shap lime
jupyter notebook
```

Then open and run:

```
XAI_Assignment_202301100049.ipynb
```

---

## 🌍 Real-World Applications

* Healthcare diagnosis systems
* Financial fraud detection
* Autonomous systems
* Risk assessment models

---

## 📚 References

* SHAP Documentation
* LIME Research Paper
* Breast Cancer Dataset (Scikit-learn)

---

## ✅ Conclusion

This assignment demonstrates how XAI techniques:

* Improve **trust and transparency**
* Help understand **model decision-making**
* Detect **biases and inconsistencies**

👉 Combining **SHAP (global + local)** and **LIME (local)** provides a powerful framework for explainable machine learning.

---

✨ *Explainability is not optional anymore — it is essential for responsible AI.*

