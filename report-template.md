# Module 20 Report 

## Overview of the Analysis
The purpose of this analysis was to evaluate whether a logistic regression model could accurately classify loan applicants as either high risk or healthy based on financial data.

The dataset included the following features:
- Loan size
- Interest rate
- Borrower income
- Debt-to-income ratio
- Number of accounts
- Derogatory marks
- Total debt

The target variable was `loan_status`, where:
- `0` = Healthy loan
- `1` = High-risk loan

The machine learning process involved the following steps:
- Importing and cleaning the dataset
- Separating features (X) and labels (y)
- Splitting the data into training and testing sets
- Training a logistic regression model
- Evaluating its performance
- Applying `RandomOverSampler` to improve prediction on imbalanced classes

## Results

### Model 1: Logistic Regression (Original Data)
- **Accuracy**: 99%
- **Precision**: 
  - 0: 100%
  - 1: 84%
- **Recall**:
  - 0: 99%
  - 1: 94%

### Model 2: Logistic Regression (Resampled Data)
- **Accuracy**: 99%
- **Precision**: 
  - 0: 100%
  - 1: 84%
- **Recall**:
  - 0: 99%
  - 1: 99%

## Summary

Both models performed with high accuracy, but Model 2 showed a stronger ability to correctly identify high-risk loans. Since these are the most important cases to flag in a lending scenario, the second model is the better choice.

The improved performance can be attributed to resampling, which helped balance the dataset and reduce bias in prediction.
