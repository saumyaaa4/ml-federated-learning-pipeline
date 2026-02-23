# Privacy-Preserving Federated Learning Pipeline (MNIST)

![Python](https://img.shields.io/badge/Python-3.10-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## Project Overview
This project implements a **federated learning pipeline** where multiple clients train ML models **locally**, and a server aggregates updates to build a **global model**.  
It is **privacy-preserving**, meaning raw data **never leaves clients**.  
Achieves **~91% global accuracy** on MNIST (handwritten digits).  

---

## Key Features
- Federated learning with **local client training & server aggregation**
- **Privacy-preserving:** raw data never shared
- Predictive model for **MNIST digit recognition**
- **Scalable & modular** for multiple clients or datasets
- Visualizations to track training progress
- Optional: deployable for **real-world ML applications**

---

## Tech Stack
- Python, TensorFlow, TensorFlow Federated  
- NumPy, Matplotlib  
- Jupyter Notebook / VS Code  
- Git & GitHub  

---

## Results

- Global model accuracy: **~91%**  
- **10 clients** training locally  
- Federated Averaging (FedAvg) used for weight aggregation  

*Example Accuracy Plot:*  
![Model Accuracy](images/accuracy_plot.png)

*Example MNIST Prediction GIF:*  
![Training Demo](images/training_demo.gif)

---

## How to Run

1. Clone the repository:

```bash
git clone <your-repo-link>
cd federated-learning-pipeline


2.Install dependencies:

pip install -r requirements.txt


3.Run the main Python script:

python src/federated_learning.py


4.Or run the Jupyter notebook for step-by-step execution:

jupyter notebook notebooks/federated_mnist.ipynb

## Author
**Saumya Bhagat** – B.Tech CSE (Data Science) | Python, ML, AI, Data Analysis  
[GitHub](https://github.com/saumyaaa4) | [LinkedIn](www.linkedin.com/in/saumya-bhagat-2b629b290)  
