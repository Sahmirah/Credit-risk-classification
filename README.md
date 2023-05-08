# Credit Risk Classification 
<br>
In this Challenge, I used various techniques to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Report Analysis
<br>
The purpose of this analysis was to build a model that could accurately predict which loans are healthy vs high-risk based on the creditworthiness of borrowers. In order to accurately portray the data I had to split the data into training and testing sets, evaluate the balanced accuracy score, and create a confusion matrix and a classification report. 

## Results
<br>

* The original data contained 75036 healthy loans and 2500 high-risk loas, which shows that the dataset is imbalanced. 
* With there being more healthy loan data to analyze, the classification report is an inaccurate portrayal of the data.  

-Machine Learning Model 1:
* Original Data Balance Accuracy Score: 0.9473616612158574
* Original Data Confusion Matrix: [[18667, 90],[63, 564]]
* Original Data Classification Report: 
             precision    recall  f1-score   support

           0       1.00      1.00      1.00     18757
           1       0.86      0.90      0.88       627

    accuracy                           0.99     19384
   macro avg       0.93      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

- Machine Learning Model 2:
* Resampled Data Balance Accuracy Score: 0.99483535716044
* Resampled Data Confusion Matrix: [[18653, 104],[3, 624]]
* Resampled Data Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18757
           1       0.86      1.00      0.92       627

    accuracy                           0.99     19384
   macro avg       0.93      0.99      0.96     19384
weighted avg       1.00      0.99      0.99     19384

## Summary
<br>
Based on the results of both machine learning models I believe that the resampled data model is more useful for lenders to incorporate into their business. Both models provided the same precision, however, the resampled data provided a better representation of the recall and f1-score. 
