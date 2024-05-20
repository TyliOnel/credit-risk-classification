# Credit Risk Classification

## Overview

In this module, the task was to develop a supervised learning model to assess the creditworthiness of loan applicants. By using subsets of the original dataset, we were able to thoroughly understand the Logistic Regression Model. The initial data was divided into a (y) label with “0” indicating a good loan applicant and “1” indicating a risky loan applicant. By removing the “loan status” column, we created an (x) label with features including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. Once the data was properly structured, the regression model was trained using x_train and y_train. The model's prediction accuracy was then tested using the x_test subset, allowing the model to predict test outcomes (y).

Factors considered in the analysis included data on:

    - The size of the loan
    - Its interest rate
    - The borrower's income
    - The debt to income ratio
    - The number of accounts the borrower held
    - Derogatory marks against the borrower
    - The total debt

## Results

The logistic regression model predicts healthy, low-risk loans with 100% precision and high-risk loans with 87% precision. The average accuracy of this model is 94%.
    - Accuracy score: 94%
    - Precision score: 93% (an average--in predicting low-risk loans, the model was 100% precise, though the model was only 87% precise in predicting high-risk loans)
    - Recall score: 95% (an average--the model had 100% recall in predicting low-risk loans, but 89% recall in predicting high-risk loans)
    
## Summary of Results:
1. Best Performing Model:

    - The logistic regression model performs exceptionally well with a balanced accuracy of 94%. This high balanced accuracy indicates strong overall performance across both low-risk and high-risk loans.

2. Performance Dependence on Problem Context:

    - If predicting low-risk loans accurately is crucial (e.g., minimizing false positives for low-risk loans), this model is ideal due to its 100% precision for low-risk predictions.
    - If predicting high-risk loans accurately is more important (e.g., identifying potential defaults), the model still performs well with an 87% precision, although there are some false positives.

## Recommendation:

Use the logistic regression model:
- It provides robust performance across both classes.
- The high balanced accuracy ensures reliable predictions in diverse scenarios, making it a strong candidate for most loan risk assessment tasks.

If the problem prioritizes identifying high-risk loans, consider additional models or techniques to improve precision for high-risk predictions while maintaining overall balanced accuracy.
