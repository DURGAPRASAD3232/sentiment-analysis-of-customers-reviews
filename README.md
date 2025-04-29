#  Sentiment Analysis of Amazon Fine Food Reviews

This repository contains the code and results for the MSc Data Science Final Project titled:  
**"Sentiment Analysis of Customer Reviews Using Machine Learning"**  
Student: *Durga Prasad Gollapudi*  
University of Hertfordshire | Module: 7PAM2002  
Supervisor: *Calum Morris*

 Submitted on: 29 April 2025  
🔗 GitHub: [https://github.com/DURGAPRASAD3232/sentiment-analysis-of-customers-reviews](https://github.com/DURGAPRASAD3232/sentiment-analysis-of-customers-reviews)

---

##  Overview

This project applies traditional **machine learning** and modern **deep learning** techniques to classify customer sentiments (positive/negative) based on the **Amazon Fine Food Reviews** dataset.

**Models evaluated:**
- Naïve Bayes
- Logistic Regression
- Support Vector Machine (SVM)
- Long Short-Term Memory (LSTM)

---

##  Objectives

- Preprocess and clean customer review data.
- Implement and compare ML & DL sentiment classifiers.
- Evaluate models using **Accuracy, Precision, Recall, and F1-score**.
- Address class imbalance using **SMOTE**.
- Extract insights using visualizations and confusion matrices.
- Explore real-world applications in e-commerce.

---

##  Dataset

- Source: [Kaggle - Amazon Fine Food Reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)
- Size: 568,000+ reviews
- Target: Binary sentiment classification  
  - **Positive (1)** = Score ≥ 4  
  - **Negative (0)** = Score ≤ 2  
  - **Neutral reviews (score = 3)** were removed

---

##  Methodology

###  Preprocessing
- Lowercasing, punctuation removal
- Stopword removal, lemmatization
- TF-IDF and Word2Vec embeddings
- SMOTE for class balancing

###  Models Implemented
| Type              | Model                |
|-------------------|----------------------|
| Machine Learning  | Naïve Bayes, Logistic Regression, SVM |
| Deep Learning     | LSTM (RNN-based)     |

###  Hyperparameter Tuning
- Grid Search (ML models)
- Learning rate, batch size, early stopping (LSTM)

---

##  Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

###  Results Summary

| Model                   | Accuracy | Precision | Recall | F1-Score |
|------------------------|----------|-----------|--------|----------|
| Naïve Bayes            | 0.87     | 0.87      | 1.00   | 0.93     |
| Logistic Regression    | 0.88     | 0.91      | 0.88   | 0.89     |
| SVM                    | 0.91     | 0.91      | 0.91   | 0.91     |
| Logistic + SMOTE       | 0.89     | 0.91      | 0.89   | 0.90     |
| LSTM                   | 0.91     | 0.91      | 0.91   | 0.91     |

> **Conclusion**: SVM and LSTM outperformed other models in accuracy and contextual understanding.

---

## Visualizations

- Sentiment Distribution Bar Charts
- Word Clouds (Positive & Negative)
- Confusion Matrices
- Review Length Analysis
- Model Metric Comparison Charts

---

##  Key Insights

- **LSTM** shows excellent performance in capturing context and long-term dependencies.
- **SVM** is highly effective on sparse text vectors (TF-IDF).
- **SMOTE** significantly improves recall for minority class (negative reviews).
- Sentiment models can drive **real-time decision-making** in e-commerce (product feedback, brand management, customer service).

---

## Folder Structure
sentiment-analysis-of-customers-reviews/
├── data/
│   ├── reviews.csv                    # Raw dataset (filtered if needed)
│   └── processed_reviews.csv          # Cleaned and labeled binary sentiment data
│
├── notebooks/
│   ├── 1_preprocessing_eda.ipynb      # Data cleaning, EDA, word clouds
│   ├── 2_ml_models.ipynb              # Naïve Bayes, Logistic Regression, SVM
│   ├── 3_lstm_model.ipynb             # LSTM implementation and evaluation
│   └── 4_model_comparison.ipynb       # Metric plots and comparative evaluation
│
├── models/
│   ├── svm_model.pkl                  # Trained SVM model
│   ├── lstm_model.h5                  # Trained LSTM model
│   ├── tfidf_vectorizer.pkl           # TF-IDF vectorizer for ML models
│   └── tokenizer.pickle               # Tokenizer used for LSTM
│
├── results/
│   ├── confusion_matrix_svm.png
│   ├── confusion_matrix_lstm.png
│   ├── model_metrics_comparison.png
│   ├── wordcloud_positive.png
│   └── wordcloud_negative.png
│
├── utils/
│   ├── preprocessing.py               # Text cleaning and tokenization functions
│   ├── visualizations.py              # Word cloud, confusion matrix, charts
│   └── model_utils.py                 # Training, evaluation, and saving helpers
│
├── report/
│   └── final_project_report.pdf       # MSc Final Project Report (optional)
│
├── sentiment_.py                      # Main script to run complete pipeline
├── README.md                          # Project overview and documentation
├── requirements.txt                   # List of Python dependencies
└── LICENSE                            # License file (MIT recommended)



