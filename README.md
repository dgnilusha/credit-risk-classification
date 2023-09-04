# credit-risk-classification

Overview

The purpose of this analysis is to create and evaluate a logistic regression model for credit risk assessment. We aim to predict whether a loan is healthy (0) or high-risk (1) based on given features. This report provides an analysis of the logistic regression model's performance.

Results:

Classification Report

The classification report for the logistic regression model with the original data is as follows:

                     precision    recall  f1-score   support

loan healthy status 1.00 0.99 1.00 18765
loan risky status 0.85 0.91 0.88 619

           accuracy                           0.99     19384
          macro avg       0.92      0.95      0.94     19384
       weighted avg       0.99      0.99      0.99     19384

Summary

The logistic regression model achieved high accuracy (99%) and F1-scores, indicating strong performance in predicting both healthy and high-risk loans.

Recommendation

Based on the high precision, recall, and F1-scores, I recommend using the logistic regression model for credit risk assessment. The model demonstrates excellent predictive capabilities for identifying healthy and high-risk loans
