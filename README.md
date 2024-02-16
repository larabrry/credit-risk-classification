# Credit Risk Classification

## Overview of the Analysis
Two machine learning models were built to identify the creditworthiness of borrowers, using a dataset of historical lending activity from a peer-to-peer lending services company.

* The data included factors such as: 
the loan size and it's interest rate; the borrower's income, debt-to-income ratio, number of accounts, total debt, and if there is derogatory marks against him.
* The model needed to predict the status of the loan (whether it's a healthy or a high-risk loan) based on the factors above.
the two machine learning models were built by using the `LogisticRegression` module from <a href=https://scikit-learn.org/stable/index.html>scikit-learn</a> scikit-learn and spliting the dataset into a training and testing sets. The first model had 75,036 healthy loan status and 2500 high-risk datapoints.

In the second logistic regression model, the dataset was resampled using the `RandomOverSampler` module from <a href=https://imbalanced-learn.org/dev/index.html>imbalanced-learn</a>. This equalized the loan status datapoints into 56277 points for each status.


## Results

* Machine Learning Model 1:
  * Accuracy: 99%
  * Precision: 100% for healthy loans, 87% in predicting high-risk loans.
  * Recall scores: 100% for hearlthy loans, 95% for high-risk loans.


* Machine Learning Model 2:
  * Accuracy: 100%
  * Precision: 100% for healthy loans, 87% in predicting high-risk loans.
  * Recall scores: 100%

## Summary

Model 2 preformed better on accuracy and recall. In fact, Model 2 scored 100% on accuracy, precision, and recall for predicting healthy loans, therefore, I would recommend this model for predicting healthy loans. 
However, since it's more important to predict the high-risk loans, neither model scored above 87% in predicting such loans.  



