# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analaysis was to train a model using Logistic Regression over a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of the borrowers.

* Explain what financial information the data was on, and what you needed to predict.
The data has 77535 rows of loans, with information about the size of the loan (loan_size), interests (interest_rate), borrower_income (borrower_income), debtor to income ratio (debt_to_income), number of accounts (num_of_accounts), derogatory marks (derogatory_marks), the total debt	(total_debt), and the loan status	(loan_status).


* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The variable that was predicted was the load status

* Describe the stages of the machine learning process you went through as part of this analysis.
For the model, I used the Logistic Regression model and tested the accuracy of the predicted loan status on the actual values. After doing this, I used a resampling method with Logistic Regression to improve the accuracy of the predictions.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
The models used to train the machine learning algorithm were Logistic Regression and then a resampling of the data, followed by another Logistic Regression.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
The accuracy was 95%, with a precision of 100% for '0' and 85% for '1'; and recall values of 99% and 91%, respectively. 

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
The accuracy was 99%, with a precision of 100% for '0' and 84% for '1'; and recall values of 99% and 99%, respectively. 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The score for the model increased from 95% to 99%; meaning the model is more accurate when using the resampling method; additionally, there is a higher recall (and by extension, a better f1-score), meaning the model identifies the actual positives better.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
It is important to detect the risk of borrowers defaulting on thier loans, so an accurate model, with a high recall is preferred to better protect the business. 

If you do not recommend any of the models, please justify your reasoning.
The first model, though having a 95% accuracy has a much higher inbalance, given the large amount of '0' on the data; the model with the resampling was better. 
