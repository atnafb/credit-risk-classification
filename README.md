## Overview of the Analysis


** purpose of the analysis - the goal of this analysis to determin if teh logistic regression machin 
learning model can be more accurately predict healty loans versus high risk loans using the orginal dataset of a dataset that is resampled to increase the sie of the minority class.

* The dataset used to perform the analysis consists of information on 77,532 loans. the data includes columns for loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derotatory_mark, total_debt and loan_status.
  the category I was attempting to predict with the anlysis is `Loan_status`.
* The remaining columns were used as features to train the data and inform the predictions.


## The stages of the machine learning process in this analysis included:

* Splitting data into labels and features, with the loan status (healthy or high-risk) being the label and the remaining seven columns as features.
* The data was then split into training and testing data sets.
* A Logistic Regression model from sklearn was created.
* Logistic Regression as a binary classifier was chosen as we are classifying loans as healthy OR high-risk and only those two options.
* The model was then fit with the training data.
* Evaluations are don by calculating and coparing metrics like accuacy score, a confusion matrix and a classification report.

## Machine Learing Methods Utilized 
* The primary model used: `LogesticRegression` model from SKLearn
* Supporting functions: `train_test_split` from SKLearn
* Models are evaluated using the following functions: `confusion_metrix` and `classification_report` from SKLearn


## Results

* Machine Learning Model 1: LogesticRegression
    * Accuracy Scores: 99%
    * Precision Scores:
        * Class 0 or Healty Loans 100%
        * Class 1 or High Risk Loans 84% 
    * Recall scores:
        * Class 0 or Healty Loans 99%
        * Class 1 or High Risk Loans 94% 

## Summary

The model performs well in predicting healthy loans using the original data, achieving a precision of 100% and a recall of 99%. However, while the model is also effective at predicting high-risk loans, 
it is not as accurate as it is with healthy loans. The precision for high-risk loans was 84%, and the recall was 94%.

Given the information, it appears that the Logistic Regression model performs well in predicting both healthy and high-risk loans based on the features used for training.
