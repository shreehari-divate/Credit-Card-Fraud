# Credit Card Fraud Detection

## Description
This is a credit card fraud detection project with dataset having more than 1 lakh entries and 31 columns. It aims to find the best model for detecting the fraudulent transactions. 

## Installation
I have made this project on google colab.
<br>If you want to download and run it on any ide, download .py file from downloads folder and install required libraries before running.

## Dataset Source
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
<br>
## Summary
Credit card transactions are very sensitive and getting the exact information is not possible. Due to this reason columns present here are time, amount, class and some other feature related to transactions which are from V1 to V28.
<br>This dataset is highly imblanced where more than 98% of transactions happend are actual transactions and rest is fraud transactions. This is given by the class column with two unique values 0 for actual transactions and 1 for fraud.
As it is a classification problem I used various algorithms such as logistic regression, SVM, Decision Trees, Random Forests and XGBoost. The imbalance in dataset is solved by oversampling the minority class using SMOTE method.
<br>Recall is our main evaluation metrics here. This is because we need to know if the transaction is normal but model is predicting that it is fraud which is a case of false positive then this would be a huge problem. That's the reason here recall is considered.
## Result
SVM and XGBoost are models having good performance with 92% recall for SVM and 91% recall for XGBoost, thus these models can be used for detection of fraudulent transactions.
