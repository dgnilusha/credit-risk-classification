# credit-risk-classification report

Overview of the Analysis

The purpose of this analysis is to build and evaluate machine learning models for credit risk assessment. We aim to predict whether a loan is healthy (0) or high-risk (1) based on financial information provided in the dataset. The variables of interest are the "loan_status" labels, which we attempted to predict.

The machine learning process involved the following stages:

Data Preparation: We split the dataset into training and testing sets to train and evaluate our models. Additionally, we performed resampling on the training data to address class imbalance.

Model Building: We used logistic regression as our primary machine learning algorithm. We trained two models: one with the original training data and another with resampled training data using the RandomOverSampler.

Results

Original Logistic Regression Model

Recall for "loan healthy status": 0.99
Precision for "loan risky status": 0.85
Recall for "loan risky status": 0.91
Accuracy: 0.99

                     precision    recall  f1-score   support

loan healthy status 1.00 0.99 1.00 18765
loan risky status 0.85 0.91 0.88 619

           accuracy                           0.99     19384
          macro avg       0.92      0.95      0.94     19384
       weighted avg       0.99      0.99      0.99     19384

Logistic Regression Model with Resampled Training Data

Balanced Accuracy Score: 0.95
Precision for "loan healthy status": 1.00
Recall for "loan healthy status": 0.99
Recall for "loan risky status": 0.99
Accuracy: 0.99

                    precision    recall  f1-score   support

loan healthy status 1.00 0.99 1.00 18765
loan risky status 0.84 0.99 0.91 619

           accuracy                           0.99     19384
          macro avg       0.92      0.99      0.95     19384
       weighted avg       0.99      0.99      0.99     19384

Summary

Both machine learning models, the original logistic regression model, and the logistic regression model with resampled training data, performed exceptionally well in predicting credit risk.

The balanced accuracy scores for both models were high, indicating strong overall performance.

The original model demonstrated an accuracy of 99%, with a precision of 0.85 and a recall of 0.91 for the "loan risky status" class. However, the model trained with resampled data achieved an even higher recall of 0.99 for the "loan risky status" class while maintaining a high overall accuracy of 99%.

The choice of which model to use may depend on the specific business objective. If the priority is to minimize the risk of missing high-risk loans, the model with resampled training data is recommended due to its higher recall. However, both models demonstrate strong predictive capabilities and can be considered for credit risk assessment.

In conclusion, the logistic regression model with resampled training data is preferred for its improved recall on high-risk loans.
