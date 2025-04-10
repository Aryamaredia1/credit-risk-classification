# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to evaluate different machine learning models to predict loan risk, identifying whether a loan applicant is likely to be a high risk (1) or healthy (0). The financial data included various borrower features, and our goal was to classify each loan into one of the two risk categories.

We analyzed the target variable, where 0 indicated a healthy loan and 1 indicated a high risk loan. The distribution was imbalanced, with the majority of loans labeled as healthy (value_counts showed many more 0s than 1s).

The machine learning process involved data preprocessing, splitting the data into training and testing sets, training a model using LogisticRegression, and evaluating the model's performance using accuracy, precision, recall, and F1 score metrics.

## Results

Machine Learning Model 1: Logistic Regression

Accuracy: 99%

Precision (0 - healthy): 1.00

Recall (0 - healthy): 0.99

Precision (1 - high risk): 0.84

Recall (1 - high risk): 0.94

F1-score (1 - high risk): 0.89


## Summary

The logistic regression model performs very well overall, with a strong accuracy (99%) and excellent performance in identifying healthy loans. It also performed well in identifying high risk loans, achieving a recall of 0.94, which means it correctly identifies most of the high-risk cases.

Since the goal of the analysis is likely to minimize the approval of high risk loans, recall for label 1 (high risk) is especially important. Based on this, the logistic regression model is a strong candidate, though further improvements could be made to increase its precision for high risk predictions.