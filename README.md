# 🧠 Sentiment Analysis of Amazon Fine Food Reviews

This repository contains the code and results for the MSc Data Science Final Project titled:  
**"Sentiment Analysis of Customer Reviews Using Machine Learning"**  
Student: *Durga Prasad Gollapudi*  
University of Hertfordshire | Module: 7PAM2002  
Supervisor: *Calum Morris*

📅 Submitted on: 29 April 2025  
🔗 GitHub: [https://github.com/DURGAPRASAD3232/sentiment-analysis-of-customers-reviews](https://github.com/DURGAPRASAD3232/sentiment-analysis-of-customers-reviews)

---

## 📌 Overview

This project applies traditional **machine learning** and modern **deep learning** techniques to classify customer sentiments (positive/negative) based on the **Amazon Fine Food Reviews** dataset.

**Models evaluated:**
- Naïve Bayes
- Logistic Regression
- Support Vector Machine (SVM)
- Long Short-Term Memory (LSTM)

---

## 🎯 Objectives

- Preprocess and clean customer review data.
- Implement and compare ML & DL sentiment classifiers.
- Evaluate models using **Accuracy, Precision, Recall, and F1-score**.
- Address class imbalance using **SMOTE**.
- Extract insights using visualizations and confusion matrices.
- Explore real-world applications in e-commerce.

---

## 🗃️ Dataset

- Source: [Kaggle - Amazon Fine Food Reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)
- Size: 568,000+ reviews
- Target: Binary sentiment classification  
  - **Positive (1)** = Score ≥ 4  
  - **Negative (0)** = Score ≤ 2  
  - **Neutral reviews (score = 3)** were removed

---

## 🛠️ Methodology

### 🔄 Preprocessing
- Lowercasing, punctuation removal
- Stopword removal, lemmatization
- TF-IDF and Word2Vec embeddings
- SMOTE for class balancing

### 🤖 Models Implemented
| Type              | Model                |
|-------------------|----------------------|
| Machine Learning  | Naïve Bayes, Logistic Regression, SVM |
| Deep Learning     | LSTM (RNN-based)     |

### 🔧 Hyperparameter Tuning
- Grid Search (ML models)
- Learning rate, batch size, early stopping (LSTM)

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 📊 Results Summary

| Model                   | Accuracy | Precision | Recall | F1-Score |
|------------------------|----------|-----------|--------|----------|
| Naïve Bayes            | 0.87     | 0.87      | 1.00   | 0.93     |
| Logistic Regression    | 0.88     | 0.91      | 0.88   | 0.89     |
| SVM                    | 0.91     | 0.91      | 0.91   | 0.91     |
| Logistic + SMOTE       | 0.89     | 0.91      | 0.89   | 0.90     |
| LSTM                   | 0.91     | 0.91      | 0.91   | 0.91     |

> **Conclusion**: SVM and LSTM outperformed other models in accuracy and contextual understanding.

---

## 📊 Visualizations

- Sentiment Distribution Bar Charts
- Word Clouds (Positive & Negative)
- Confusion Matrices
- Review Length Analysis
- Model Metric Comparison Charts

---

## 🧠 Key Insights

- **LSTM** shows excellent performance in capturing context and long-term dependencies.
- **SVM** is highly effective on sparse text vectors (TF-IDF).
- **SMOTE** significantly improves recall for minority class (negative reviews).
- Sentiment models can drive **real-time decision-making** in e-commerce (product feedback, brand management, customer service).

---

## 📁 Folder Structure



