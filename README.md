# Supervised_Learning_Challenge

## Imported the following imports and dependancies:

- import numpy as np
- import pandas as pd
- from pathlib import Path
- from sklearn.metrics import balanced_accuracy_score
- from sklearn.metrics import confusion_matrix
- from imblearn.metrics import classification_report_imbalanced
- from sklearn.linear_model import LogisticRegression
- from imblearn.over_sampling import RandomOverSampler

## The Analysis.
- The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.

- This analysis is done by using various techniques to train and evaluate models with imbalanced classes.

- This analysis used a logistic regression model to compare two versions of dataset i.e original dataset and resampled data

- The data is lending data that is in  in csv form that I used pandas library to read and predict: * high risk loans '1' and * healthy loans '0'

- For the analysis I ;
* Checked the balance of y/target values with value_counts
* Split  data into training and testing data with train_test_split
* Created a model with LogisticRegression().
* Trained the model with model.fit().
* Made predictions with model.predict().
* Evaluated the model with balanced_accuracy_score().
* Calculated the metrics for our model with classification_report_imbalanced
* Resampled data to fit model and make predictions with RandomOverSampler 


## Model 1 predictions:
       pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.99      0.99      1.00      0.99      0.99     18765
          1       0.84      0.99      0.99      0.91      0.99      0.99       619

avg / total       0.99      0.99      0.99      0.99      0.99      0.99     19384


## Model 2 predictions:
        pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.99      0.99      1.00      0.99      0.99     18765
          1       0.84      0.99      0.99      0.91      0.99      0.99       619

avg / total       0.99      0.99      0.99      0.99      0.99      0.99     19384


## Conclusion:

