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
