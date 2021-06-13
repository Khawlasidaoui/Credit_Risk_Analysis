# Credit_Risk_Analysis

## Overview

Apply machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, different techniques are used to train and evaluate models with unbalanced classes.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the data from the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm to see if that is better. Also reduce bias using two other ML models, BalancedRandomForestClassifier and EasyEnsembleClassifier. The performance of these models will be evaluated whether they should be used to predict credit risk.

## Results

### Oversampling

- Naive Random Oversampling
![image](https://user-images.githubusercontent.com/79415699/121817723-0ef0a000-cc51-11eb-879d-984f7932b825.png)


- SMOTE
![image](https://user-images.githubusercontent.com/79415699/121817742-2a5bab00-cc51-11eb-8498-87f927275210.png)


### Undersampling

- Cluster Centroids
![image](https://user-images.githubusercontent.com/79415699/121817757-3ba4b780-cc51-11eb-89bc-1e8140b1dee6.png)


### Combination (Over and Under) Sampling

- SMOTEENN
![image](https://user-images.githubusercontent.com/79415699/121817764-4f501e00-cc51-11eb-8bc9-f8b22f957a13.png)


### Ensemble Learners

- Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/79415699/121817781-727acd80-cc51-11eb-96db-340c28aaaa49.png)


- Easy Ensemble AdaBoost
![image](https://user-images.githubusercontent.com/79415699/121817794-7dcdf900-cc51-11eb-9b82-d444e08b53bf.png)


## Summary

Easy Ensemble AdaBoost Classifier is the most effective ML model providing the best f1 score which balances accuracy and precision to consider the score. Precision is found to be low for all the models. 

Recommendation would be to use the Easy Ensemble AdaBoost Classifier as it classified the most true positives. 
