# Module 12 Report 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Purpose of the analysis.
I am using various techniques to train and evaluate a model based on loan risk. 

* Explain what financial information the data was on, and what you needed to predict.
I am using a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The variable I am using the logistic regression model predict is "loan_status" which has two options, both the 0 (healthy loan) and 1 (high-risk loan).


* Describe the stages of the machine learning process you went through as part of this analysis.
The stages of the machine learning process I went through as part of the analysis are to:
1) Split the data into training and test sets
2) Create a logistic regression model with the original data 
3) Evaluate the model's performance
4) Predict a logistic regression model using resampled training data
5) Evaluate the model's performance with the resampled training data

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
I create a logistic regression model with the original data looking at loan status, and then I saved the prdictions on the testing data lebels by using the testing feature data (X_test) and the fitted model. I evaluated the model's performance by looking at the accuracy score and generating a confusion matrix and classification report. Then, I resampled the data and created a new logistic regression model, and evaluated it in a similar way.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
- Healthy Loans
    - When the model predicts healthy loans, it is correct 100 percent of the time.
    - Out of all actual healthy loan instances, the model correctly identified 99 percent of the time. 
- High-risk Loans
    - When the model predicts high-risk loans, it is correct 85 percent of the time. 
    - Out of all actual high-risk loan instances, the model correctly identified 91 percent of the time. 
- The model was accurate 99 percent across all classes. 
  

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
- Healthy Loans
    -  When the model predicts healthy loans, it is correct 100 percent of the time. 
    - Out of all actual healthy loan instances, the model correctly identified 99 percent of the time.
    
- High-risk Loans
    - When the model predicts high-risk loans, it is correct 84 percent of the time. 
    - Out of all actual high risk loan instances, the model correctly identified 99 percent of the time. 
- The model was accurate 99 percent across all classes
    



## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The resampled model tends to perform best in comparison to the original model because it has a higher recall score. If all actual high risk loan instances, the model correctly identified 99 percent of the time, compared to the original model at 91 percent of the time. 
The overall prediction score was lower by 1 percent for the high-risk loans using model 2 however. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Yes, if we are trying to predict the 0s, or healthy loans, then Model 1 is better. 
If we are trying to predict the 1s, or high-risk loans, then Model 2 is better. 

If you do not recommend any of the models, please justify your reasoning.
