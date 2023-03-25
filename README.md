# Overview of the Analysis

## Credit Risk Classification Report 


The purpose of this analysis is to build, train and evaluate a Logistic regression model that identify the credit worthiness of a borrower.

We will be using a dataset of historical lending activity from a peer-to peer lending serviced company to predict the status of loans as healthy or high-risk .

Our target , 'loan_status' is imbalanced. the reason is that healthy loans  out number risky loans.


* 0 (Healthy)  75036
* 1  (High-Risk)   2500

We will test our model on two versions of the dataset using the original dataset, Then, using resample the data .

First, we Split the Data into Training and Testing Sets. Then, Create a Logistic Regression Model with the Original Data. Finally, Predict a Logistic Regression Model with Resampled Training Data.

For both cases, we will get the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report to determin which model preformce better. 

# Results

## Machine Learning Model 1: Original Data

###  Healthy Loans 
* Precision: 1.00
* Recall: 0.99

###  High-Risk Loans
* Precision: .85
* Recall: 0.91


## Machine Learning Model 2: Resampled data

###  Healthy Loans 
* Precision: 1.00
* Recall: 0.99

###  High-Risk Loans
* Precision: .84
* Recall: 0.99

## Summary

 The model trained with resampled data preformed the best over original data. While both model had identical precision and recall for healthy loan, the 2nd model was better identifying actual instances for high risk loans. 

Performance does depend on the problem were solving. in this case it would be ideal for the lending company to use the model that contains higher recall as you want to correctly identify the loans that are actually High-risk over misidentifying false positive for High-Risk.

In general, a high precision and recall indicates that the model is performing well on both classes. In this case, the model(2) performance is quite good, particularly for healthy loans. 
