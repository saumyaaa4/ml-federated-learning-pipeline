# 🧠 Federated Learning-Based Distributed Model Training

## 📌 Project Overview

This project implements a privacy-preserving federated learning pipeline using TensorFlow Federated. Multiple clients train models locally on their own data, while a central server aggregates model updates using Federated Averaging.

The system achieves **~96.7% global accuracy on the MNIST dataset**, demonstrating effective distributed deep learning without sharing raw data.

---

## 🚀 Key Features

- Multi-client distributed training simulation  
- Local model training on each client  
- Secure weight aggregation using Federated Averaging  
- Privacy-preserving architecture (no raw data sharing)  
- Accuracy improvement across federated rounds  
- Modular and scalable design  

---

## 🏗 System Architecture

1. Data is partitioned across multiple clients  
2. Each client trains a local TensorFlow model  
3. Model weights are sent to a central server  
4. Server aggregates weights (Federated Averaging)  
5. Global model is updated and redistributed  
6. Process repeats for multiple federated rounds  

---

## 📊 Results

- Final Global Accuracy: **96.7%**
- Improved accuracy across 5 federated rounds
- Stable convergence during training

### 📈 Federated Convergence

![Federated Convergence](images/convergence_plot.png)

### 🔍 Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

---

## 🛠 Tech Stack

- Python  
- TensorFlow  
- TensorFlow Federated  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

## ▶️ How to Run

```bash
pip install -r requirements.txt
python federated_learning.py
