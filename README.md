# Credit Risk Analysis Report

## Overview
The purpose of this analysis is to develop a machine learning model for assessing the credit risk of borrowers using historical lending data. The goal is to build a model that can accurately identify the creditworthiness of loan applicants, distinguishing between healthy loans (0) and high-risk loans (1).

## Model Performance Metrics
- **Balanced Accuracy Score**: The balanced accuracy score provides an overall measure of the model's ability to predict both healthy and high-risk loans while considering class imbalance. A higher score indicates better performance.
- **Precision**: Precision measures the accuracy of high-risk loan predictions. A higher precision means fewer false positives, minimizing the risk of granting loans to potentially risky borrowers.
- **Recall**: Recall, or sensitivity, assesses the model's ability to correctly identify high-risk loans among all actual high-risk loans. A higher recall means fewer false negatives, reducing the chance of missing potentially risky borrowers.
- **F1-Score**: The F1-Score is the harmonic mean of precision and recall, offering a balanced measure of the model's accuracy for both classes.

## Model Evaluation
- The logistic regression model was trained on the original data and achieved a balanced accuracy score of .95, demonstrating good performance in predicting both healthy and high-risk loans.
- The precision, recall, and F1-Score for high-risk loans were .85, .91, and .88, respectively, indicating that the model effectively identifies risky borrowers with minimal false positives.
- For healthy loans, the precision, recall, and F1-Score were 1.00, .99, and 1.00, respectively, reflecting the model's accuracy in identifying low-risk borrowers while maintaining a balanced performance.

## Recommendation
- The logistic regression model trained on the original data shows promising results, with balanced accuracy and reasonable precision and recall scores for both classes. It can be recommended for use by the company, considering its ability to identify high-risk loans without overly impacting the approval of healthy loans.

## Resampling and Model Evaluation
- To address class imbalance, a resampling technique (RandomOverSampler) was applied, creating a balanced dataset.
- The logistic regression model trained on the resampled data maintained its ability to predict both healthy and high-risk loans effectively.
- The balanced accuracy score, precision, recall, and F1-Score for both classes improved after resampling, confirming the model's capability to handle class imbalance.

## Final Recommendation
- Based on the improved performance after resampling, it is recommended to use the logistic regression model trained on resampled data for credit risk assessment. This model demonstrates balanced and reliable prediction capabilities for both healthy and high-risk loans, minimizing the risk of lending to potentially risky borrowers.

The logistic regression model, particularly when trained with oversampled data, proves to be a valuable tool for the company in making informed decisions regarding loan approvals, reducing the likelihood of lending to high-risk borrowers, and maintaining a balanced approach towards healthy loans.
