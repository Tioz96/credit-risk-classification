# Module 12 Report Template

## Overview of the Analysis

In this analysis, we aimed to develop and evaluate machine learning models to predict credit risk in a lending dataset. The purpose of this analysis was to build models that can effectively distinguish between healthy loans (label 0) and high-risk loans (label 1). The dataset contained various financial information about loans, and we needed to predict whether a loan is likely to be healthy or at high risk of defaulting.

The analysis consisted of the following stages:

Data preprocessing, including separating features and labels, and exploring the class distribution.
Building a logistic regression model using the original data.
Training and evaluating a logistic regression model with resampled training data to address class imbalance.

## Results

### Logistic Regression Model (Original Data)
Accuracy Score: 0.99
Precision (Healthy Loan - Label 0): 1.00
Recall (Healthy Loan - Label 0): 0.99
Precision (High-Risk Loan - Label 1): 0.85
Recall (High-Risk Loan - Label 1): 0.91

### Logistic Regression Model (Resampled Data)
Balanced Accuracy Score: 0.9936781215845847
Precision (Healthy Loan - Label 0): 1.00
Recall (Healthy Loan - Label 0): 0.99
Precision (High-Risk Loan - Label 1): 0.84
Recall (High-Risk Loan - Label 1): 0.99

## Summary

The logistic regression model trained with the original data demonstrated a high accuracy score. It effectively predicted both healthy loans and high-risk loans, as indicated by the precision and recall scores. However, the model's performance on high-risk loans, while still acceptable, showed room for improvement in terms of precision.

The logistic regression model trained with resampled data showcased a balanced accuracy score that takes class imbalance into account. This model achieved a high recall for both classes, especially for high-risk loans. While the precision for high-risk loans was slightly lower compared to the original model, the balance between precision and recall is notable, making it a reliable choice for identifying high-risk loans.

Considering the importance of identifying high-risk loans to mitigate potential losses, we recommend using the logistic regression model trained with resampled data. This model strikes a better balance between identifying actual high-risk loans and minimizing false positives. However, it's crucial to consider the specific business goals and requirements when choosing the final model.
