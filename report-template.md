# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

> The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.

> This analysis is done by using various techniques to train and evaluate models with imbalanced classes.

> This analysis used a logistic regression model to compare two versions of dataset i.e original dataset and resampled data

> The data is lending data that is in  in csv form that I used pandas library to read and predict: * high risk loans '1' and * healthy loans '0'

> For the analysis I ;
>> Checked the balance of y/target values with value_counts
>> Split  data into training and testing data with train_test_split
>> Created a model with LogisticRegression().
>> Trained the model with model.fit().
>> Made predictions with model.predict().
>> Evaluated the model with balanced_accuracy_score().
>> Calculated the metrics for our model with classification_report_imbalanced
>> Resampled data to fit model and make predictions with RandomOverSampler 



Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

> Accuracy score for model 1 is 0.9520479254722232
> Precision score for model 1  healthy loans '0' is 1 and for model 1 high risk loans '1' is 0.85 
> Recall score for model 1 healthy loans '0' is 0.99 and for model 1 high risk loans '1' is 0.91



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

> Accuracy score for model 2 is 0.9936781215845847
> Precision score for model 2  healthy loans '0' is 1 and for model 2 high risk loans '1' is 0.84 
> Recall score for model 2 healthy loans '0' is 0.99 and for model 2 high risk loans '1' is 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

> There is a 99.37 % balanced accuracy score with model 2 compared to 95.20 % balanced accuracy score with model 1. Meaning model 2 was much better at detecting  true positives and true negatives. However, there is less precision by 1% with oversampled data(MODEL 2) for the high risk loans.

> Precision for healthy loans is at 100% for both predictions.

> Recall for healthy loans is equal for both models at 99 % however,recall for model 2 high risk loans is more at 99 % compared to model 1 at 91%.



If you do not recommend any of the models, please justify your reasoning.

> I would recommend model 2 as it has higher balanced accuracy and higher recall %.
