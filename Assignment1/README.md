# Lab Assignment 01 — Neural Network from Scratch on Iris Dataset

**Name:** Nirjara More  
**PRN:** 202301100049  
**Batch:** A1

---

## 📌 Overview

This assignment implements a **fully connected feedforward neural network from scratch** using only NumPy, without any deep learning frameworks. The model is trained and evaluated on the classic **Iris Species Dataset** to classify flowers into 3 species based on 4 features.

---

## 📂 Dataset

| Property | Details |
|---|---|
| **Name** | Iris Species Dataset (`https://www.kaggle.com/datasets/uciml/iris`) |
| **Samples** | 150 |
| **Features** | 4 (Sepal Length, Sepal Width, Petal Length, Petal Width) |
| **Classes** | 3 (Iris-setosa, Iris-versicolor, Iris-virginica) |
| **Split** | 80% Train / 20% Test (manual, seed=42) |

---

## 🧠 Neural Network Architecture

```
Input Layer   →   Hidden Layer   →   Output Layer
  4 neurons         8 neurons           3 neurons
               (Sigmoid activation)  (Softmax activation)
```

- **Loss Function:** Categorical Cross-Entropy  
- **Weight Init:** Random (scaled)  
- **Feature Scaling:** Min-Max Normalization  
- **Labels:** One-Hot Encoded  

---

## 🔢 Steps Covered

| Step | Description |
|---|---|
| 1 | Import Libraries |
| 2 | Load Dataset |
| 3 | Data Understanding & Exploration |
| 4 | Data Preprocessing (scaling, encoding, train-test split) |
| 5 | Neural Network Architecture Design |
| 6 | Weight Initialization |
| 7 | Activation Functions (Sigmoid, Softmax) |
| 8 | Forward Propagation |
| 9 | Loss Function (Cross-Entropy) |
| 10 | Backpropagation |
| 11 | Gradient Descent (Weight Update) |
| 12 | Training — Batch Gradient Descent (Baseline) |
| 13 | Loss vs Epoch Visualization |
| 14 | Experiments — Learning Rate Comparison |
| 15 | Optimization Techniques (Batch GD, SGD, Mini-Batch GD) |
| 16 | Advanced Optimizers (Momentum, Nesterov) |
| 17 | Full Optimizer Comparison |
| 18 | Evaluation on Test Set |
| — | Summary & Discussion |

---

## 📊 Visualizations

- Scatter plots (feature vs feature, coloured by species)
- Histograms of feature distributions
- Box plots per species
- Sigmoid & its derivative curve
- Softmax demo
- Training Loss vs Epoch
- Learning rate comparison curves
- Optimizer comparison plots

---

## ⚙️ Optimizers Compared

- Batch Gradient Descent
- Stochastic Gradient Descent (SGD)
- Mini-Batch Gradient Descent
- Batch GD + Momentum
- Nesterov Accelerated Gradient (NAG)

---

## 🛠️ Requirements

```bash
pip install numpy pandas matplotlib
```

> The notebook uses `google.colab.files` for dataset upload — run it in **Google Colab** or replace the upload cell with a local `pd.read_csv("Iris.csv")` if running locally.

---

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/drive/1EXQUwFUYAbwz8Ykp_MSIpoQcO_6nBZND)
2. Upload `Iris.csv` when prompted (Step 2), or place it in the same directory.
3. Run all cells sequentially (`Runtime → Run all`).

---

