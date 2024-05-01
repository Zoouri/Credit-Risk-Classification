# Credit-Risk-Classification



## Overview of the Analysis


The purpose of this analysis was to build and evaluate machine learning models to address given challenge of loan prediction, focusing on financial outcome. This section describes the overall approach, types of financial data used and the steps taken to develop, train and evaluate machine learning models. 

## Purpose of the Analysis

The goal was to predict the financial capacity of the creditworthiness of borrowers which would help determine and predict the risk-classification of the loan (high or low risk). This prediction provides valuable insights for financial decision-making and risk management. the analysis was conducted on financial data provided as a CSV file.

## Financial information

The data contained various financial records such as the intendent `size of the loan`, `interest rate`, `borrower income`, `debt to income`, `number of accounts`, `derogatory marks`, `total debt` and `loan status`. This data is used to further develop machine learning to help and determine suitability of the borrower considering all the above factors.

## Variable
The variable that was tried to be predicted was `loan status` where:
* Class 0 (healthy loan)
* Class 1 (high-risk loan)

## Stages of Machine Learning 

 * Splitting data into labels and features, witht he loan status as 0 - low risk and 1 - high risk.
 * The data was then divided into trainign and testing dataset.
 * Logistic Regression model was created (having only 2 binary options for loan status).
 * The model was subsequently fitted into the training data.
 * Predictions were generates.
 * Evaluation of the model using accuracy, precision and recall scores.


## Results

* Accuracy
    The model receives accuracy of 0.99, meaning that it correctly classifies 99% of all instances.

* Precision
    - Healthy Loan (Class 0): The precision for this class is 1.00, indicating that all instances predicted as healthy loans are indeed healthy loans.
    - High-risk Loan (Class 1): The precision is 0.87, suggesting that 87% of instances are predicted as high-risk loans are actually high-risk.

* Recall
    - Healthy Loan (Class 0): The recall for this class is 1.0, indicating that all the moel correctly identifies 100% of actual healthy loans.

    - High-risk Loan (Class 1): The recall is 0.89, meaning that 89% of actua; high-risk loans are correctly identified by the model.

    These metrics provide a comprehensive overview of the LogisticRegression model's performance in terms of accuracy, precision and recall for both healthy and high-risk loans.


## Summary

The logistic regression model demonstrates excellent performance in predicting healhy loans, with a precision of 1.0 and a recall of 1.0. However, when it comes to high-risk loans, the model's accuracy is slightly lower, with precision of 0.87 and recall of 0.89.

The lower precision and recall predicting risky loans could be due to the imbalanced nature of the dataset. The test data for class 1 comprises only 2500 instances, which is significantly lower compared to the 75036 instances for class 0. This imbalance suggests that the model has fewer high-risk loas data to learn from, impacting its ability to accurately predict this class. An increaase in high-risk data in the training set and could potentially improve model's performance.


When considering the classification of loans, preventing high-risk loans it is crucial, as the financial loss from a single defaulted loan can far exceed the gains from issuing the loan. Thus, improving the prediction of risky loans should be a key focus. Depsite it is limitations, the overall accuracy of the model remains high, at 99%.
