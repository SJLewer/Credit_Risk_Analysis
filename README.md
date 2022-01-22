# Credit_Risk_Analysis

## Overview of Analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  This analysis employs different techniques to train and evaluate models to predict credit risk.

_Techniques_:
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
 ### NAIVE RANDOM OVERSAMPLING
  ![Naive Random OverSmplg Summary](https://user-images.githubusercontent.com/90986041/150651949-b5a05be8-f155-4ddd-9de2-93eeb7571034.png)
 * This model may not be the best for identifying riksy loans because the accuracy, 0.657, is low and the precision (.01), recall (0.71), and low f1 score (0.02) for predicting high risk are not good enough to state that the model will be good at classifying high credit risk.

 ### SMOTE
  ![SMOTE Summary](https://user-images.githubusercontent.com/90986041/150651956-7508225a-fb98-4f4d-8ef4-ab5945fa87fd.png)
* This model did not outperform the random oversampler.  It may not be the best for identifying riksy loans because the accuracy, 0.657, is low and the precision (0.01), recall (0.63), and low f1 score (0.02) for predicting high risk are not good enough to state that the model will be good at classifying high credit risk.

 ### UNDERSAMPLING WITH CLUSTER CENTROIDS
  ![UnderSampling ClusterCentroid Summary](https://user-images.githubusercontent.com/90986041/150651961-a7a54ff0-633c-4b65-be2c-3236f91e5984.png)
* This model may not be the best for identifying risky loans because the accuracy, 0.544, is low and the precision (0.01), recall (0.69), and low f1 score (0.01) for predicting high risk are not good enough to state that the model will be good at classifying high credit risk.
 
 ### COMBINED APPROACH WITH SMOTEENN
  ![OverUnder Sampling SMOTEENN Summary](https://user-images.githubusercontent.com/90986041/150651977-68ffafe6-3bcf-4e45-b47f-ef9547dd4a2c.png)
* This model showed improvement over the previous models.  However, it may not be the best for identifying risky loans because the accuracy, 0.688, is low and the precision (0.01), recall (0.80), and low f1 score (0.02) for predicting high risk are not good enough to state that the model will be good at classifying high credit risk.

 ### BALANCED RANDOM FOREST CLASSIFIER
   ![Balanced Random Classifier Summary](https://user-images.githubusercontent.com/90986041/150651991-211666cc-8ab7-4c01-a864-7368fbe72e45.png)
* This model may not be the best for identifying risky loans.  While the accuracy, 0.789, is higher than the previous models, the precision (0.03), recall (0.70), and low f1 score (0.06) for predicting high risk are not good enough to state that the model will be good at classifying high risk.

 ### EASY ENSEMBLE ADABOOST
  ![Easy Ensemble AdaBoost Summary](https://user-images.githubusercontent.com/90986041/150652004-d886b960-d155-4291-b3ac-00612cbfd3fa.png)
* This model showed improvement over the previous models.  The accuracy score (0.932) and recall score (0.92) are high.  However, the precision score (0.09) is low.  The low f1 score (0.16) depicts the pronounced imbalance between the recall and precision scores.  
 
## Summary/Recommendation:
As described above, none of the results solidly support a statement that any of the models will be good at predicting credit risk.  Further model refinement is needed.  As an example, use the ranked features list created from the Random Forest Classifier model to identify features with the most impact (see link below).  Drop the irrelevant features and re-evaluate the models.

 * Features list excerpt: https://github.com/SJLewer/Credit_Risk_Analysis/blob/main/Sorted%20Features.png
___
## Resources:
_Data Sources_: Credit card dataset from LendingClub, a peer-to-peer lending services company

_Python Scripts_: 

_Analyst_: S. Lewer
