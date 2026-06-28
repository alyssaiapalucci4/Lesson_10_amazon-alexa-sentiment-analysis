# Amazon Alexa Customer Review Sentiment Analysis (Lesson 10)

## Project Overview

This project uses machine learning and natural language processing (NLP) to analyze Amazon Alexa customer reviews and classify them as **positive** or **negative**. The goal is to compare different models and see which one performs best for sentiment analysis.

For this assignment, I worked through data cleaning, feature engineering, model training, evaluation, and visualization.

---

## Student Information

**Student Name:** Alyssa Iapalucci  
**Google Colab Notebook Link:** https://colab.research.google.com/drive/1Fpa9wy16V4rpgw81-j3bwMe36uQt32dQ?usp=sharing

**GitHub Repository Link:** 

---

---

## Dataset

The dataset used is the Amazon Alexa Reviews dataset.

It includes:

- **rating** – customer rating
- **variation** – product type
- **verified_reviews** – customer review text
- **feedback** – sentiment label (1 = positive, 0 = negative)

Dataset file: `amazon_alexa.tsv`

Source: Public dataset from :contentReference[oaicite:0]{index=0}

---

## Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Gensim
- Transformers

Install required libraries:

```bash

pip install pandas numpy matplotlib seaborn scikit-learn gensim transformers


What the Project Does

1. Data Cleaning
- Checks for missing values
- Removes unnecessary columns

2. Data Visualization

Creates graphs to show:

- Sentiment distribution
- Product variation vs rating

3. Feature Engineering

Converts text into numbers using:

- TF-IDF
= Bag of Words

4. Machine Learning Models

Trains and tests:

- Logistic Regression
- SVM
- Random Forest

5. Model Evaluation

Measures model performance using:

- Accuracy
- Classification report
- Confusion matrix
- ROC curves

6. Advanced NLP

Also includes:

- Word2Vec
- t-SNE visualization
- BERT sentiment testing

7. Custom Prediction

Tests new review text with a prediction function.

Example: predict_sentiment("This product is amazing")

Output: Positive


## How to Run

Open the notebook in Google Colab
Upload the dataset file (amazon_alexa.tsv)

Make sure the file path is: /content/amazon_alexa.tsv

Run all cells in order.

Repository Files
- README.md
- Lesson_10_Assignment_AI.ipynb
- amazon_alexa.tsv


Conclusion

This project helped me understand how sentiment analysis works using machine learning and NLP. I was able to compare different models and use additional tools like Word2Vec and BERT to explore the data further.

