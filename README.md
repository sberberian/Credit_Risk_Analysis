# Credit_Risk_Analysis

## Overview
  These analyses utilize machine learning to assess credit card risk. The following classification reports explain the capabilities of various models in predicting low and high risk loans. 

## Results 

### Undersampling
![undersample](images/undersample.png)

* The recall for predicting high and low risk are very close but precision for low risk indicates that there are no false positives.

### Naive Oversampling
![naiveoversample](images/naiveoversample.png)

* The naive oversampling results are rather similar to those of the undersampling. The precision for low risk is also a noteworthy 1.00. 

### SMOTE Oversampling 
![smoteoversample](images/smoteoversample.png)

* The precision is consistent and the recall is still around 0.6.

### Combination (Over and Under) Sampling 
![combosample](images/combosample.png)

*  The precision continues the same but the recall for high risk loan has jumped a bit and the low risk dropped a little. 

### Balanced Random Forest Classifier 
![balancedrandomforest](images/balancedrandomforest.png)

* As a model oriented on eliminating bias, this model shows the first alteration in the the precision for high risk loans, which has increased. The recall for high risk has decreased slightly compared to the combination sampling model, but the low risk loans has risen tremendously. 

### Easy Ensemble AdaBoost Classifier 
![easyensemble](images/easyensemble.png)

* The easy ensemble model has the highest precision of all models for high risk loans and record recalls for both high and low risk loans.

## Summary 
  It's clear that, regardless of the model, there is complete certainty that the loans tagged as low risk truly are low risk yet the certainty for tagging high risk loans are extremely low. In the case of this endeavor, however, sensitivity is the more important measure. It'd be safer to have a more sensitive model that accidentally tags low risk as high risk than to miss identifying a high risk loan. Of all the models, the easy ensemble adaboost classifier was the most suitable for this scope since it had not only the greatest recall but the greatest precision for high risk loans as well. I would still not recommend using this model either. It's wonderful to have such high sensitivity but with the precision being as low as it is means the model is ultimately not very useful. 
