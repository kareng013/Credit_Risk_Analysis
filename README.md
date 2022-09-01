# Credit Risk Analysis

## Overview of Analysis


In this challenge we'll employ different techniques to train and evaluate models that are built to identify risky loans through resampling.
Utilizing the credit card dataset from LendingClub, we'll be oversampling, undersampling, and using a combination approach to evaluate which model is the best to identify risk with precision. Lastly, we'll compare Balanced Random Forest classifier and Easy Ensemble classifier to predict credit risk. After evaluating all models, we'll make a decision on which model to utilize and make recommendations on to predict credit risk. 


## Results

### Deliverable 1: Using Resampling models to predict credit risk 

1. Naive Oversampling
    - Balanced accuracy score: 65.3%
    - High risk precision is 1% with a recall of 62%

![Naive_Oversampling](https://github.com/kareng013/Credit_Risk_Analysis/blob/main/Images/Naive%20Oversampling%20Results.png)

2. SMOTE Oversampling
    - Balanced accuracy score: 65.5%
    - High risk precision is 1% with a recall of 64%

![SMOTE_Oversampling](https://github.com/kareng013/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Oversampling%20Results.png)

3. Undersampling 
    - Balanced accuracy score: 51%
    - High risk precision is 1% with a recall of 59%

![Undersampling](https://github.com/kareng013/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)

4. Combination (OVer and Under) Sampling
    - Balanced accuracy score: 63.7%
    - High risk precision is 1% with a recall of 70%

![Combination_Sampling](https://github.com/kareng013/Credit_Risk_Analysis/blob/main/Images/Combination%20Sampling%20Results.png)

### Deliverable 2: Use SMOTEENN Algorithm to predict credit risk

5. Balanced Random Forest Classifier
    - Balanced accuracy score: 78.8%
    - High risk precision is 4% with a recall of 67%

![Random_Forest](https://github.com/kareng013/Credit_Risk_Analysis/blob/main/Images/Balanced%20Random%20Forest%20Results.png)

6. Easy Ensemble AdaBoost Classifier
    - Balanced accuracy score: 92.5%
    - High risk precision is 7% with a recall of 91%

![Ensemble_AdaBoost](https://github.com/kareng013/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20AdaBoost%20Results.png)

## Summary

In Summary, all six models had a low risk precision score of 1% with a recall rate of 59-91%. This means there was a large number of false positives and labelled more applicants as high risk while they were actually low risk. This could tarnish a companies ability to gain a customer base if they are continuously rejecting customers on this basis. 
The model with the highest recall was Easy Ensemble Classifier, and is the closest and best model used to detect high risk applicants. However, the risk precision is extremely low. 

Based on these results, my recommendation would be not to use any of these models as they all have a very low risk precision with a large number of false positives. 