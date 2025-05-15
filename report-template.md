# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

The logistic regression model performed exceptionally well, achieving an overall accuracy of 0.99. It demonstrated near-perfect precision and recall for predicting healthy loans (`0`), and strong performance in identifying high-risk loans (`1`), with a precision of 0.84 and a recall of 0.94.

This means the model correctly identified most high-risk loans while maintaining a low false-positive rate. In a financial context where the cost of missing a high-risk loan can be significant, the high recall for the `1` class is especially valuable.

Given these results, the logistic regression model is recommended for deployment, particularly in scenarios where identifying high-risk loans is a priority. While other models could potentially improve performance further, this model provides a strong and reliable baseline.
