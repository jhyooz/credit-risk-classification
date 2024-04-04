# Credit Risk Analysis Report
## Overview of the Analysis

The purpose of this analysis is to test and recommend a machine learning model that predicts loans to be either high risk or healthy depending on the information provided.

* The data used in the training of the model contains the following information:
  * Borrower Income
  * Debt to Income ratio
  * If the borrower has any derogatory marks
  * Interest rate of the loan
  * Loan size
  * Loan Status
  * Number of accounts
  * Total Debt
  
The model was able to predict:
  * the number of each loan status:
    * Healthy Loan: 18,765 instances 
    * High Risk Loan: 619 instances 
  * the loan status variable consists of two classes:
    * Healthy Loan: No default (Majority of borrowers)
    * High Risk Loan: Could default (Minority of borrowers)


## Stages of the machine learning process 

**Stage 1**: Process the Data: split the data into features (X) and labels/variables set (y). Then the data was spit again into a training set and a testing set.

**Stage 2**: Selected a Model: Used a Logistic Regression model and evaluated the model's performance

**Stage 3**: Trained the Model: we used training data to train the Logistic Regression model

**Stage 4**: Evaluated the Model: Generated a report to evaluate the model's use of the training data by looking at metrics such as accuracy and precision. The confusion matrix shows that the model correctly classified a majority of loans.

## Logisitic Regression Model
I used the Logistic Regression as we only need two outcomes (0 - Healthy/1 - High Risk). The model was fitted to the training data, then I used the testing data (X_test) to make predictions. To evaluate the model's performance I created a classification report and confusion matrix.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Logistic Regression Model:
  * Class 0 (Healthy)
    * F1 score: 100%
    * Precision: 100%
    * Recall score: 99%
  * Class 1 (High Risk)
    * F1 score: 88%
    * Precision: 85%
    * Recall score: 91%


## Summary

The logistic regression model shows excellent performance in predicting loan defaults, with a 99% F1-score accuracy with balanced precision and recall scores. It excels particularly in identifying low-risk loans, with high precision and recall. While still strong in predicting high-risk loans, with 85% precision and 91% recall, there is still room for improvement. Overall, the model's accuracy, precision, and recall make it the recommended choice for credit risk assessment. Ongoing monitoring and optimization could further enhance its predictive capabilities.