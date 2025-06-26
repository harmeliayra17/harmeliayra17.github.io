---
title: "Fake News Detection using Various Machine Learning Models"
date: 2025-05-21 00:00:00 +0800
categories: [Machine Learning Project]
tags: [Machine Learning, Fake News, Text Classification, NLP, Python]
image: /assets/img/fake-banner.png
---

# Fake News Detection using Various Machine Learning Models

This project compares the performance of several machine learning models in detecting fake news based on text data. The dataset used is a combination of real and fake news articles.

## 🧠 Models Used

Each model is trained using a pipeline that includes `TfidfVectorizer` and the respective classifier:

1. **Logistic Regression**
2. **Support Vector Machine (SVM)**
3. **Random Forest**
4. **XGBoost**

Each model is evaluated using a manual testing dataset (real & fake news), and the evaluation results are recorded.

## 📈 Model Evaluation Results

Below is the comparison of model performance based on *Accuracy*, *Precision*, *Recall*, and *F1 Score*.

<img src="/assets/img/compare_output.png" alt="Model Comparison" width="400"/>

### 🏆 Key Takeaways:
- **SVM** and **Logistic Regression** show the most stable and high performance overall.
- **Random Forest** achieves high *precision*, but has a lower *recall*.
- **XGBoost** fails to predict the real news class (label 1), resulting in significantly lower overall performance.

## 📊 Detailed Evaluation (Classification Reports & Confusion Matrices)

### 🔍 Logistic Regression
<img src="/assets/img/output_lgs.png" alt="Logistic Regression Confusion Matrix" width="400"/>

### 🔍 Support Vector Machine (SVM)
<img src="/assets/img/output_svm.png" alt="SVM Confusion Matrix" width="400"/>

### 🔍 Random Forest
<img src="/assets/img/output_rf.png" alt="Random Forest Confusion Matrix" width="400"/>

### 🔍 XGBoost
<img src="/assets/img/output_xgb.png" alt="XGBoost Confusion Matrix" width="400"/>

---
