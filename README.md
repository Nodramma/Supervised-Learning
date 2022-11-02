# Credit Risk Analysis Report

## Overview of the Analysis


* The purpose of this analysis is to describe the results and conclusions obtained using machine learning models.

* For the testing I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers

* The dataset originaly contained imbalanced information where for 75036 examples of healthy loans there were only 2500 examples of default ones. 

* Initially I created the lables 'y' for loan-status and 'X' for other features of the data, then I separated the provided information on training and testing sets. I create a Logistic Regression Model, fit model with original training data. I saved the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. After that I evaluated the model’s performance by: Calculating the accuracy score of the model, generate a confusion matrix and printing the classification report.
* Then for the model 2 I used Rendon Oversampling Method to resample the original training data and equalize the samples of healty and default loans data. The resumpled training data was again used to train Logistic Regression model. The results of predictions of the new resumpled model were evaluated in the same manner.  

* For the analysis I utilized Logistic Regression - method for predicting binary outcomes from data using sigmoid function, where the function converts continuous data on the borrower to a percentage probability of being a 'good credit borrower' if the probability is above a certain freshhold.
* For the resumpling I used Random Overesumpling Method. This method creates more instances of a class label by randomly celecting minority class instances and adding additional samples.


## Results


* Machine Learning Model 1:
  * Accuracy - 0.95
  * Precision: for good loans - 1, for bad - 0.84 
  * Recall:  for good loans - 0.99, for bad - 0.91.



* Machine Learning Model 2:
  * Accuracy - 0.99
  * Precision: for good loans - 1, for bad - 0.85 
  * Recall:  for good loans - 0.99, for bad - 0.99.

## Summary

* From the results optained from analysis of machine learning models processing given imbalanced data, we may conclude that it is beneficional to use the resumpling of the training data for balancing of the positive and negative training samples. The resumpling helped to improve accuracy of the predictions overall as well as increased the rate of the recall of default loans.

* In our case the correct prediction of unhealthy loans is important because mistakes can cause significant loses.

