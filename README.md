# Credit_Risk_Analysis
 
## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. 

I will employ different techniques such as the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I'll oversample the data using the Random Over Sampler and SMOTE algorithms, and undersample the data using the Cluster Centroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I'll compare two new machine learning models that reduce bias, Balanced Random Forest Classifier and Easy Ensemble Classifier, to predict credit risk.

## Results

## Resampling Models to Predict Credit Risk

### Oversampling Random Over Sampler
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

### Cluster Centroids Undersampling
- Balanced accuracy score: 63%
- High risk precision score: 1% 
- Low risk precision score: 100%
- High risk recall score: 60%
- Low risk recall score: 43%

![ClusterCentroids](https://user-images.githubusercontent.com/100816778/177928920-26dc9615-b9bb-4e63-b733-c46d06b178f3.png)

### SMOTEENN Sampling
- Balanced accuracy score: 52%
- High risk precision score: 1% 
- Low risk precision score: 100%
- High risk recall score: 74%
- Low risk recall score: 58%

![SMOTEENN](https://user-images.githubusercontent.com/100816778/177928943-1e33e392-c47d-497c-920d-8b73164a6a32.png)

### Balanced Random Forest Classifier
- Balanced accuracy score: 79%
- High risk precision score: 4% 
- Low risk precision score: 100%
- High risk recall score: 67%
- Low risk recall score: 91%

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/100816778/177929238-23a70251-c6e8-43f3-9edd-e0aa56235c66.png)

### Easy Ensemble Classifier
- Balanced accuracy score: 93%
- High risk precision score: 4% 
- Low risk precision score: 100%
- High risk recall score: 67%
- Low risk recall score: 91%

![EasyEnsembleClassifier](https://user-images.githubusercontent.com/100816778/177929420-1db4e7fc-0a5c-4f6d-9f33-ed5ef24b146b.png)

## Summary
The goal of this analysis is to identify the model that will most accurately predict if a loan is high risk or not. The top three models with the best high risk recall scores are:
- SMOTEENN Sampling 74%
- Easy Ensemble Classifier 67%
- Balanced Random Forest Classfier 67%

To further analyze these three models, their balanced accuracy score was taken into account:
- SMOTEENN Sampling 52%
- Easy Ensemble Classifier 93%
- Balanced Random Forest Classfier 79%

Overall, the Easy Ensemble Classifier is the best model that was used, showing a 93% balanced accuracy scoreand a 67% high risk recall score. The Balanced Random Forest Classifier was the next best performing model, showing a balanced accuracy score of 79% and a 67% high risk recall score. 

I would recommend using the Easy Ensemble Classifier model to predict high risk loans.



