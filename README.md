# Credit Card Fraud Detection 🏦🔍
**Author: Prathamesh Bhamare**
**Linkedin: https://www.linkedin.com/in/prathamesh-bhamare-7480b52b2/**
**If you find this project useful, feel free to fork it, submit a pull request, or give it a ⭐ star! 🚀**

This repository contains an end-to-end implementation of **Credit Card Fraud Detection** using various machine learning classifiers. The dataset used is highly imbalanced, so **SMOTE (Synthetic Minority Over-sampling Technique)** has been applied to balance the classes. Several classification models are trained and evaluated to identify fraudulent transactions.

---

## 📌 Dataset
The dataset used is **[Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)**.  
- The dataset contains transactions made by credit cards in September 2013 by European cardholders.
- It has **284,807 transactions**, where only **0.172% are fraudulent (Class = 1)**.
- Features are numerical and anonymized for confidentiality, except **Time** and **Amount**.

---

## 🔬 Steps Covered in the Notebook

### 1️⃣ **Exploratory Data Analysis (EDA)**
- Visualizing class imbalance.
- Distribution of transaction amounts and time.
- Checking summary statistics.

### 2️⃣ **Data Preprocessing**
- Dropping unnecessary columns (`Time`).
- Applying **log transformation** on `Amount` to normalize distribution.
- Splitting dataset into train & test sets.
- Applying **SMOTE** to handle class imbalance.

### 3️⃣ **Model Training & Evaluation**
The following models were trained and evaluated:
1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**
4. **XGBoost Classifier**
5. **LightGBM Classifier**
6. **Support Vector Classifier (SVC)**

Evaluation metrics used:
- **Accuracy**
- **Recall** (Important for fraud detection)
- **F1 Score**
- **Precision**
- **Confusion Matrix**

---

## 📊 Model Performance Summary
| Model                 | Accuracy | Recall | F1-Score | Precision |
|----------------------|-----------|---------|----------|------------|
| Logistic Regression  | 97.48% | 91.66% | 10.93% | 5.81% |
| Decision Tree        | 99.74% | 77.08% | 50.51% | 37.56% |
| Random Forest       | 99.95% | 82.29% | 85.40% | 88.76% |
| XGBoost             | 99.93% | 83.33% | 81.21% | 79.20% |
| LightGBM            | 99.85% | 84.37% | 66.12% | 54.36% |
| Support Vector Machine | 98.36% | 89.58% | 15.56% | 8.52% |

---

## 🛠️ Requirements
- Python 3.8+

- NumPy

- Pandas

- Scikit-learn

- Matplotlib

- Seaborn

- Imbalanced-learn

- XGBoost

- LightGBM

---

## 📜 Observations:
- The dataset is highly imbalanced (fraud cases are very rare).

- SMOTE effectively balanced the data, improving model performance.

- XGBoost and Random Forest performed the best in terms of recall and overall accuracy.

---

## 🚀 How to Run
### **1. Clone the Repository**

git clone https://github.com/yourusername/Credit-Card-Fraud-Detection.git

### **2. Change to the Directory**
cd Credit-Card-Fraud-Detection

---
