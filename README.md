# 🧠 Federated Learning-Based Distributed Model Training

## 📌 Project Overview
This project demonstrates a **privacy-preserving federated learning pipeline** for handwritten digit classification using the **MNIST dataset**. Unlike traditional centralized training, federated learning allows multiple clients to train a shared global model **without sharing their raw data**, ensuring data privacy and decentralization.

The system achieves **~96.7% global accuracy on MNIST**, demonstrating effective distributed deep learning across multiple clients while respecting privacy constraints.

### Key Highlights
- Implements **Federated Averaging (FedAvg)** for multi-client training  
- Simulates **heterogeneous (Non-IID) client data** to mirror real-world scenarios  
- Tracks **global and client-specific performance** across training rounds  
- Includes **visualizations of accuracy/loss trends and confusion matrices**  

### Problem Statement
In real-world applications, sharing raw user data is often restricted due to privacy or regulatory concerns. Centralized ML models require all data in one place, which is unsuitable for sensitive datasets. This project addresses the challenge of **training a robust global model while keeping client data private**, simulating real-world federated environments like mobile devices or hospitals.

### Motivation / Why Federated Learning
- Ensures **data privacy** and regulatory compliance  
- Eliminates the need for **centralized data storage**  
- Demonstrates **advanced distributed machine learning concepts**  
- Provides practical experience in **federated optimization, decentralized training, and privacy-preserving AI**

---

## 🚀 Key Features
- Multi-client distributed training simulation  
- Local model training on each client  
- Secure weight aggregation using **Federated Averaging**  
- Privacy-preserving architecture (**no raw data sharing**)  
- Accuracy improvement across federated rounds  
- Modular, scalable, and recruiter-friendly design  

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
- Accuracy progression tracked across 5 federated rounds  
- Stable convergence demonstrated in training

### 📈 Federated Convergence
![Federated Convergence](images/convergence_plot.png)

### 🔍 Confusion Matrix
![Confusion Matrix](images/confusion_matrix.png)

> **Note:** Slight fluctuations in accuracy across rounds are expected due to heterogeneous client data distribution, which mirrors real-world federated learning scenarios.

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
1. Clone the repository:
```bash
git clone <https://github.com/saumyaaa4/ml-federated-learning-pipeline>
cd ml-federated-learning-pipeline

2. Install dependencies:
```bash
pip install -r requirements.txt

3. Run the federated learning pipeline:
```bash
python federated_learning.py

4. (Optional) Open the Jupyter Notebook for visualizations and experimentation:
```bash
jupyter notebook federated_mnist.ipynb
