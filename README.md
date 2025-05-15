# Module 20 Report 

## Overview of the Analysis

The purpose of this analysis was to apply supervised machine learning techniques to predict whether a loan is high-risk (`1`) or healthy (`0`). The data included various financial features such as loan size, interest rate, and borrower information.

The goal was to train classification models to accurately predict the risk level of loans based on these financial indicators. The primary variable of interest was the `loan_status`, a binary feature where `0` indicates a healthy loan and `1` indicates a high-risk loan. The dataset was imbalanced, with many more healthy loans than high-risk loans, which influenced model evaluation.

The machine learning process included:
- Cleaning and preprocessing the data
- Splitting the data into training and testing sets
- Training a `LogisticRegression` model
- Using a confusion matrix and a classification report to evaluating model performance using metrics such as accuracy, precision, recall, and F1-score


## Results

* **Machine Learning Model 1: Logistic Regression**
    * **Accuracy Score:** 0.99  

    * **Class 0 (Healthy Loan):**
      - Precision: 1.00  
      - Recall: 0.99  
      - F1-score: 1.00  
      - Support: 18,765  

    * **Class 1 (High-Risk Loan):**
      - Precision: 0.84  
      - Recall: 0.94  
      - F1-score: 0.89  
      - Support: 619  

    * **Overall Metrics:**
      - **Macro Average:**
        - Precision: 0.92  
        - Recall: 0.97  
        - F1-score: 0.94  
      - **Weighted Average:**
        - Precision: 0.99  
        - Recall: 0.99  
        - F1-score: 0.99  


## Summary

The logistic regression model performed very well, achieving an overall accuracy of 0.99. It demonstrated near-perfect precision and recall for predicting healthy loans (`0`), and strong performance in identifying high-risk loans (`1`), with a precision of 0.84 and a recall of 0.94.

This means the model correctly identified most high-risk loans while maintaining a low false-positive rate. In a financial context where the cost of missing a high-risk loan can be significant, the high recall for the `1` class is especially valuable.

Given these results, the logistic regression model is recommended for deployment, particularly in scenarios where identifying high-risk loans is a priority. While other models could potentially improve performance further, this model provides a strong and reliable baseline.
