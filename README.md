# 🚨 Intrusion Detection System (IDS) using PyTorch & Scikit-learn

This project implements an **Intrusion Detection System (IDS)** using the **NSL-KDD dataset**, a benchmark dataset for evaluating network-based intrusion detection models. The system combines both **deep learning (PyTorch)** and **machine learning (scikit-learn)** models for comparative analysis.

---

## 📁 Dataset

The project uses the processed `kdd_train.csv` and `kdd_test.csv` versions of the **NSL-KDD dataset**, containing 42 features per instance (both numerical and categorical).

- **Target variable**: `normal` (label 0) or `attack` (label 1)
- **Categorical features** are label-encoded
- **Features are scaled** using `MinMaxScaler`

> 🔗 Download the original dataset from the [NSL-KDD Repository](https://www.unb.ca/cic/datasets/nsl.html)

---

## 🧠 Models Included

### 1. **SimpleNN (PyTorch)**

- Feedforward neural network:
  - Input layer (41 features)
  - Two hidden layers with **ReLU** activation and **Dropout**
  - Output layer with **Sigmoid** activation for binary classification

### 2. **Random Forest Classifier (Scikit-learn)**

- Ensemble-based traditional classifier
- Handles both categorical and numerical data
- Fast and accurate for tabular data

### 3. **Support Vector Machine (SVM) (Scikit-learn)**

- Kernel-based classifier
- Trained on a subset of the dataset due to computational cost
- Effective in high-dimensional spaces

---

## 📊 Evaluation Metrics

Each model is evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

Bar plots are generated to visually compare model performance across these metrics.

---

## 🧪 Requirements

- Python 3.7+
- PyTorch
- Pandas
- NumPy
- Scikit-learn
