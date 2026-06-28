# Amazon Alexa Customer Review Sentiment Analysis (Lesson 10)

## Project Overview

This project focuses on sentiment analysis using Amazon Alexa customer reviews. The goal is to classify customer reviews as either **positive** or **negative** based on the review text.

In this notebook, I use Natural Language Processing (NLP) and Machine Learning techniques to clean, process, analyze, and predict customer sentiment. Multiple models are trained and compared to determine which model performs best.

This assignment demonstrates data preprocessing, feature engineering, model training, model evaluation, visualization, and advanced NLP methods.

---

## Student Information

**Student Name:** Alyssa Iapalucci  
**Lesson:** Lesson 10 
**Google Colab Notebook Link:** [Paste your Google Colab link here]  
**GitHub Repository Link:** [Paste your GitHub repository link here]  

---

## Objective

The objective of this project is to build machine learning models that can accurately predict customer sentiment from Amazon Alexa product reviews.

The project includes:

- Data cleaning and preprocessing
- Data visualization
- Feature engineering using text vectorization
- Training multiple machine learning models
- Model evaluation and comparison
- Feature importance analysis
- Word embedding visualization
- BERT sentiment analysis
- Predicting sentiment on new text input

---

## Dataset

This project uses the Amazon Alexa Reviews dataset.

The dataset contains the following columns:

- **rating** — Customer star rating
- **date** — Date of the review
- **variation** — Product version/type
- **verified_reviews** — Written customer review
- **feedback** — Sentiment label

Sentiment labels:
- **1 = Positive**
- **0 = Negative**

**Dataset file used:**

`amazon_alexa.tsv`

**Dataset source:** Public Amazon Alexa Reviews dataset from :contentReference[oaicite:0]{index=0}

---

## Libraries Used

This project uses the following Python libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- gensim
- transformers

---

## Installation Requirements

Install all required libraries before running the notebook:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn gensim transformers
Project Workflow
1. Import Libraries

The notebook begins by importing all necessary libraries for:

Data analysis
Data visualization
Machine learning
NLP processing
Model evaluation
2. Load Dataset

The dataset is loaded into Google Colab using Google Drive.

Example:

from google.colab import drive
drive.mount('/content/drive')

df = pd.read_csv('/content/amazon_alexa.tsv', sep='\t')
3. Data Cleaning

The data cleaning process includes:

Checking for missing values
Removing null values
Removing unnecessary columns:
date
rating

This helps simplify the dataset for sentiment analysis.

4. Data Visualization

Visualizations are created to better understand the data:

Sentiment distribution countplot
Product variation vs rating barplot

These graphs help identify patterns in customer feedback.

5. Feature Engineering

Text data is transformed into numerical data using:

TF-IDF Vectorization

Used as the main feature extraction method.

Bag of Words (CountVectorizer)

Used as an additional feature engineering method.

These methods convert text into machine-readable format for model training.

6. Train-Test Split

The dataset is split into:

80% training data
20% testing data

This allows the models to train on one portion and test on unseen data.

7. Machine Learning Models

The following machine learning models are trained:

Logistic Regression

A linear classification model.

Includes hyperparameter tuning using GridSearchCV.

Support Vector Machine (SVM)

Used for classification with a linear kernel.

Random Forest Classifier

An ensemble model used to improve prediction performance.

8. Model Evaluation

Each model is evaluated using:

Accuracy Score
Classification Report
Precision
Recall
F1-score
Confusion Matrix

Confusion matrices are visualized using heatmaps.

9. ROC Curve Analysis

ROC curves are created to compare model performance.

This helps evaluate the trade-off between true positive rate and false positive rate.

Models compared:

Logistic Regression
SVM
Random Forest
10. Feature Importance

Feature importance is extracted from the Random Forest model.

This identifies the top words that influence sentiment predictions.

A bar graph displays the most important features.

11. Word2Vec

Word2Vec is used to create word embeddings from the review text.

This allows words to be represented as vectors.

12. t-SNE Visualization

t-SNE reduces Word2Vec vectors into 2D space for visualization.

This helps show relationships between words in the dataset.

13. BERT Sentiment Analysis

A pre-trained BERT model is used for simple sentiment analysis testing.

This demonstrates modern NLP transformer-based analysis.

Example:

from transformers import pipeline

bert = pipeline("sentiment-analysis")
print(bert("I love this Alexa device!"))
14. New Prediction Function

A custom function is created to test new customer reviews.

Example:

predict_sentiment("This product is amazing")

Expected output:

Positive
How to Run the Notebook
Option 1: Run in Google Colab
Open the notebook file:
Lesson_10_Assignment_AI.ipynb
Upload the dataset file:
amazon_alexa.tsv
Mount Google Drive:
from google.colab import drive
drive.mount('/content/drive')
Verify the dataset path:
/content/amazon_alexa.tsv
Run all notebook cells in order.
