# Amazon Alexa Customer Review Sentiment Analysis (Assignment 10)

## Project Overview
This project performs sentiment analysis on Amazon Alexa customer reviews using machine learning techniques. The goal is to classify reviews as either **positive** or **negative** based on the review text and related features.

We apply natural language processing (NLP) techniques and supervised learning models to build and evaluate a sentiment classification system.

---

## Dataset
The dataset used in this project contains Amazon Alexa product reviews and includes the following key features:

- `rating` – Star rating given by the customer
- `verified_reviews` – Text review written by the customer
- `variation` – Product variation of Alexa device
- `feedback` – Sentiment label (1 = positive, 0 = negative)

Source: Public Amazon Alexa Reviews dataset (commonly available on Kaggle)

---

## Objective
To build a machine learning model that can accurately predict customer sentiment from review text.

---

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Handling missing values
- Removing duplicates (if any)
- Cleaning text data (lowercasing, removing punctuation, stopwords)
- Encoding categorical variables

### 2. Feature Engineering
- Text vectorization using:
  - Bag of Words (CountVectorizer)
  - TF-IDF (optional improvement)
- Converting text into numerical features for ML models

### 3. Model Building
Machine learning models used:
- Logistic Regression
- Random Forest Classifier

### 4. Model Evaluation
- Accuracy score
- Confusion matrix
- Precision, recall, and F1-score
- Classification report

### 5. Visualization
- Sentiment distribution plots
- Confusion matrix heatmap
- Feature importance (Random Forest)

---

## Machine Learning Models

### Logistic Regression
A baseline linear model used for binary classification.

### Random Forest Classifier
An ensemble learning method used to improve prediction accuracy and reduce overfitting.

---

## 📈 Results
The models are evaluated using standard classification metrics:

- Accuracy Score
- Precision / Recall / F1-score
- Confusion Matrix

Final model performance may vary depending on preprocessing and feature engineering choices.

---

## Technologies Used

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- NLTK
- Matplotlib
- Seaborn

---
