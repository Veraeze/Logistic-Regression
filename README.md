# Logistic-Regression
# Customer Satisfaction Prediction

This project builds a logistic regression model to predict customer satisfaction based on e-commerce customer behavior data.

## Use Case

Predict whether a customer is satisfied (`Satisfied`) or not (`Neutral`/`Unsatisfied`) using features like:

- Age
- Gender
- City
- Membership Type
- Total Spend
- Items Purchased
- Average Rating
- Discount Applied
- Days Since Last Purchase

## Dataset
Source: kaggle's e-commerce customer behavior dataset
Columns used:
 - Customer ID
 - Gender
 - Age
 - City
 - Membership Type
 - Total Spend
 - Items Purchased
 - Average Rating
 - Discount Applied
 - Days Since Last Purchase
 - Satisfaction Level (target variable)

## Approach

- Cleaned and preprocessed dataset.
- Encoded ordinal, binary, and categorical variables.
- Converted `Satisfaction Level` into binary target:
  - `Satisfied` → 1
  - `Neutral` or `Unsatisfied` → 0
- Split data into training and testing sets.
- Trained Logistic Regression using sklearn pipeline.
Evaluated model with:
  - Accuracy
  - Confusion Matrix
  - Classification Report
  - ROC Curve
  - Feature Importance

## Results

- Accuracy: ~98.6%
- Excellent precision, recall and f1-score.





#  Spam Email Detection using Logistic Regression

This project applies Logistic Regression to detect spam emails using the UCI Spambase Dataset (https://archive.ics.uci.edu/ml/datasets/spambase). 
It demonstrates data preprocessing, model training, evaluation, and basic visualization.


##  Dataset Summary

- Source: UCI Machine Learning Repository - Spambase
- Rows: 4601 emails
- Columns: 57 features + 1 target column
- Target Variable: `spam`
  - `1` = Spam
  - `0` = Not Spam


##  Features

The dataset contains 57 features including:
- Word frequency features (e.g., `word_freq_make`, `word_freq_address`, etc.)
- Character frequency features (e.g., `char_freq_$`, `char_freq_!`)
- Capital letter run features:
  - `capital_run_length_average`
  - `capital_run_length_longest`
  - `capital_run_length_total`


##  Project Goal

To build a binary classification model that accurately classifies emails as spam or not spam using logistic regression.

##  Workflow

1. Load Data: `.data` file was read using Pandas, and column names were parsed from the `.names` file.
2. Preprocessing:
   - Features scaled using `StandardScaler`.
   - Data split into training and test sets.
3. Modeling:
   - Logistic Regression with scaled features.
4. Evaluation:
   - Accuracy: 91.96%
   - Confusion Matrix
   - Precision, Recall, F1-Score


##  Model Performance

- Accuracy: 91.96%
- Confusion Matrix:
[[506  25]
[ 49 341]]
- Notes:
1. Strong precision and recall for both classes.
2. Balanced model performance.
