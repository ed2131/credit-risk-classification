# Credit Risk Analysis Project

## Overview of the Analysis

The purpose of this analysis was to develop a machine learning model capable of predicting credit risk in a peer-to-peer lending scenario. Using historical lending activity data from a peer-to-peer lending services company, the goal was to identify the creditworthiness of borrowers. This task is crucial in the financial industry to minimize the risk of loan defaults.

The dataset contained information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable was `loan_status`, representing whether a loan is high-risk (`1`) or healthy (`0`).

During the analysis, the following stages of the machine learning process were undertaken:
1. **Data Preprocessing**: The dataset was split into features (X) and the target variable (y). The features included all columns except for `loan_status`, and the target variable was solely `loan_status`.
2. **Model Selection and Training**: A Logistic Regression model was chosen due to its effectiveness in binary classification tasks. 
3. **Model Evaluation**: The model's performance was evaluated using a confusion matrix and classification report, focusing on metrics such as accuracy, precision, recall, and F1-score.

## Results

For the Logistic Regression model, the following results were obtained:

* **Logistic Regression Model**:
  * **Accuracy**: The model achieved a high overall accuracy of 99%, indicating excellent performance in classifying loans.
  * **Precision and Recall for Healthy Loans (0)**: Both metrics were nearly 100%, demonstrating outstanding ability in identifying healthy loans.
  * **Precision and Recall for High-Risk Loans (1)**: Precision was 86%, and recall was 91%, showing strong, but slightly lesser performance compared to healthy loans. This indicates that the model is quite reliable in identifying high-risk loans, though not as perfect as for healthy loans.
  * **F1-Score**: The F1-score for high-risk loans was 88%, balancing between precision and recall.

## Summary

The Logistic Regression model showed excellent performance in predicting loan status, with particularly strong results for healthy loans and commendable performance for high-risk loans. The high accuracy and balanced precision and recall suggest that the model is well-suited for both identifying potential defaulters and minimizing false alarms.

Given the results, I recommend the Logistic Regression model for predicting credit risk in this context. Its high accuracy and balanced precision and recall for both classes make it a reliable tool in a financial setting, where correctly identifying both healthy and high-risk loans is crucial.

However, it's important to consider the slightly lower precision for high-risk loans, which might be an area for improvement. In future analyses, exploring models or techniques better suited for imbalanced datasets, such as SMOTE (Synthetic Minority Over-sampling Technique) or ensemble methods, could further enhance performance, especially for the minority class (high-risk loans).
