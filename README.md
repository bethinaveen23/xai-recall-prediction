# 🧠 Explainable Recall Prediction System

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/ML-XGBoost%20%7C%20RandomForest%20%7C%20SVM-green)
![Deep Learning](https://img.shields.io/badge/DL-CNN%20%7C%20LSTM-orange)
![Explainable AI](https://img.shields.io/badge/XAI-SHAP%20%7C%20LIME-red)
![Status](https://img.shields.io/badge/Status-Research%20Project-success)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Overview

This project focuses on predicting whether a user will recall a learned concept using behavioral interaction data from adaptive learning systems.

Unlike traditional models that act as black boxes, this system emphasizes **interpretability alongside accuracy**, ensuring that predictions are understandable and aligned with real-world learning behavior.

---

## ❓ Problem Statement

Adaptive learning platforms need to predict when a user is likely to forget information.

Most machine learning models:

* Provide high accuracy
* But fail to explain **why** predictions are made

This project bridges that gap using Explainable AI techniques.

---

## ⚙️ Approach

### 🔹 Data Processing

* Large-scale user–lexeme interaction dataset
* Sampled to ~5000 instances for efficient computation
* Applied encoding, scaling, and missing value handling

---

### 🔹 Models Implemented

#### Classical Machine Learning:

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)
* XGBoost

#### Deep Learning:

* Multi-Layer Perceptron (MLP)
* 1D Convolutional Neural Network (CNN)
* Long Short-Term Memory (LSTM)
* CNN + LSTM Hybrid
* Autoencoder + Random Forest

---

### 🔹 Explainable AI (XAI)

* **SHAP (SHapley Values)** → Global feature importance
* **LIME** → Local prediction explanations
* **PDP & ICE** → Feature behavior analysis

---

## 📊 Results

| Model         | Accuracy | ROC-AUC |
| ------------- | -------- | ------- |
| Random Forest | ~0.968   | ~0.993  |
| XGBoost       | ~0.970   | ~0.994  |
| CNN + LSTM    | ~0.968   | ~0.993  |

---

## 🔍 Key Insights

* `history_correct` → Strong positive influence on recall
* `delta` (time gap) → Negative impact on memory retention
* `session_correct` → Improves recall prediction confidence

These align with real-world learning behavior and cognitive theories.

---

## 📈 Outputs

### 🔹 SHAP Summary Plot

![SHAP](outputs/shap_plots/shap_summary_rf.png)

---

### 🔹 Confusion Matrix

![Confusion Matrix](outputs/confusion_matrix/confusion_matrix_rf.png)

---

### 🔹 Feature Importance

![Feature Importance](outputs/graphs/feature_importance_rf.png)

---

### 🔹 Model Comparison

![Model Comparison](outputs/graphs/model_comparison.png)

---

## 🧪 Tech Stack

* **Languages:** Python
* **Libraries:** Pandas, NumPy, scikit-learn
* **ML Models:** Random Forest, XGBoost, SVM
* **Deep Learning:** TensorFlow / Keras
* **Explainability:** SHAP, LIME
* **Visualization:** Matplotlib, Seaborn

---

## 📂 Project Structure

```plaintext id="structure_block"
xai-recall-prediction/
│
├── data/
├── notebooks/
├── src/
├── outputs/
│   ├── shap_plots/
│   ├── confusion_matrix/
│   └── graphs/
│
├── requirements.txt
└── README.md
```

---

## 🚀 Future Work

* Deploy as a Streamlit web application
* Build interactive explainability dashboards
* Explore transformer-based sequence models
* Improve real-time prediction capabilities

---

## 👤 Author

**Bethi Naveen Kumar**
🔗 LinkedIn: https://www.linkedin.com/in/naveen-kumar-23109i

---

## ⭐ Final Note

This project focuses not only on building accurate machine learning models, but on understanding their behavior and ensuring their decisions are transparent and meaningful in real-world applications.
