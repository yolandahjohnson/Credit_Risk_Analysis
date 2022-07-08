# Credit_Risk_Analysis
 
## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. 

I will employ different techniques such as the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I'll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results

## Resampling Models to Predict Credit Risk

### Oversampling RandomOverSampler
- Balanced accuracy score: 66%
- High risk precision score: 1% 
- Low risk precision score: 100%
- High risk recall score: 63%
- Low risk recall score: 68%

![RandomOverSampler](https://user-images.githubusercontent.com/100816778/177925934-8f423078-4c89-4974-9b2c-4eb5f79d73ea.png)

### SMOTE Oversampling
- Balanced accuracy score: 63%
- High risk precision score: 1% 
- Low risk precision score: 100%
- High risk recall score: 61%
- Low risk recall score: 65%

![SMOTE Oversampling](https://user-images.githubusercontent.com/100816778/177928395-74c8e912-802b-4c60-8280-a829b45158c8.png)
