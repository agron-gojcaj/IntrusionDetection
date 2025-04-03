# 🚨 Intrusion Detection System (IDS) using PyTorch

This project implements a deep learning-based Intrusion Detection System (IDS) using the **NSL-KDD dataset**, a widely used benchmark for evaluating intrusion detection models.

The model is trained to classify network connections as either **normal** or **malicious (attack)** using a **binary classification** approach with **PyTorch**.

---

## 📁 Dataset

The project uses the `kdd_train.csv` and `kdd_test.csv` versions of the NSL-KDD dataset, with 42 features including both numeric and categorical attributes.

- Download the original dataset from [NSL-KDD Repository](https://www.unb.ca/cic/datasets/nsl.html) or use the included CSV files.

---

## 🧠 Model Overview

The model is a **feedforward neural network** with:

- Input Layer (41 features)
- Two Hidden Layers with ReLU activation and Dropout
- Output Layer with Sigmoid activation (for binary classification)

---

## 🧪 Requirements

- Python 3.7+
- PyTorch
- Pandas
- NumPy
- Scikit-learn
