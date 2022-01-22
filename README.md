# Credit_Risk_Analysis

## Overview of Analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  This analysis employs different techniques to train and evaluate models to predict credit risk.

Techniques:
1. Oversampling models:
    - RandomOverSampler
    - SMOTE
2. Undersample model:
    - ClusterCentroids
3. Combined approach with over- and undersampling
    - SMOTEENN
4. Models that reduce bias:
    - BalancedRandomForestClassifier
    - EasyEnsembleClassifier

## Results:
_Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

 ### NAIVE RANDOM OVERSAMPLING
 ![Naive Random OverSmplg Summary](https://user-images.githubusercontent.com/90986041/150648323-82019edd-6d67-4882-b3e3-52f62f91ca4d.png)

 ### SMOTE
 ![SMOTE Summary](https://user-images.githubusercontent.com/90986041/150648587-3f9ba990-3e95-4921-9571-6883a8a836a5.png)

 ### UNDERSAMPLING WITH CLUSTER CENTROID
 ![UnderSampling ClusterCentroid Summary](https://user-images.githubusercontent.com/90986041/150648644-423b7b21-a087-4672-9684-fb698e5e36c4.png)

 ### COMBINED APPROACH WITH SMOTEENN
 ![OverUnder Sampling SMOTEENN Summary](https://user-images.githubusercontent.com/90986041/150648672-8ff04731-6d1e-43e3-98e7-edd189a617f0.png)

 ### BALANCED RANDOM FOREST CLASSIFIER
 ![Balanced Random Classifier Summary](https://user-images.githubusercontent.com/90986041/150648716-4479164b-1ad2-4a43-82ea-0f67eb01a300.png)

 ### EASY ENSEMBLE ADABOOST
 ![Easy Ensemble AdaBoost Summary](https://user-images.githubusercontent.com/90986041/150648723-a170aff4-e422-449c-8f76-a90e223d7725.png)


 
 
## Summary/Recommendation:
_Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
___
## Resources:
_Data Sources_: Credit card dataset from LendingClub, a peer-to-peer lending services company

_Python Script_: 

_Analyst_: S. Lewer
