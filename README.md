# Customer Churn Prediction

## Overview
Predict customer churn for a telecom company using a neural network. Achieves **78.5% test accuracy**.

---

## Dataset
- **Features**: 20 attributes (demographics, services, billing).
- **Target**: `Churn` (0 = retained, 1 = left)

---

## Preprocessing
- Dropped `customerID`.
- Encoded categorical features (`Yes`/`No` → `1`/`0`).
- Scaled numerical features (`MinMaxScaler`).
- One-hot encoded `InternetService`, `Contract`, `PaymentMethod`.

---

## Model
**3-Layer Neural Network** (TensorFlow/Keras):
- Input Layer (26 neurons, ReLU)
- Hidden Layer (15 neurons, ReLU)
- Output Layer (1 neuron, Sigmoid)

**Training**:
- Optimizer: Adam
- Epochs: 10
- Train/Test Split: 80/20

---

## Results
- **Accuracy**: 78.5%
- **Precision/Recall**:
  - Class 0: 0.82 / 0.89
  - Class 1: 0.66 / 0.52

---

## Quick Start
1. Install dependencies:
   ```bash
   pip install pandas numpy tensorflow scikit-learn matplotlib seaborn
