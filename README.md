# 17_Credit_Risk_Analysis
Module 17 Challenge Credit Risk Analysis for Supervised Machine Learning and Credit Risk

## Overview of the analysis: 
This exercise was to apply machine learning to solve a real-world challenge of credit card risk.  I employed different techniques to train and evaluate models with unbalanced classes.  There was a total of six algorithms used to evaluate the data given 
- Random Oversampling using `RandomOverSampler`
- Oversampling using `SMOTE`
- Undersampling using `ClusterCentroids`
- Combination of over- and undersampling using `SMOTEEN`
- Ensemble Classifier `BalancedRandomForestClassifier`
- Ensemble Classifier `EasyEnsembleClassifier`

## Results: 

### Accuracy Score

![Deliverable 1 Accuracy Score](/images/D1AccuracyScore.png)

![Deliverable 2 Accuracy Score](/images/D2AccuracyScore.png)

![Deliverable 3 Accuracy Score](/images/D3AccuracyScore.png)


### Confusion Matrix 

![Deliverable 1 Confusion Matrix](/images/D1ConfusionMatrix.png)

![Deliverable 2 Confusion Matrix](/images/D2ConfusionMatrix.png)

![Deliverable 3 Confusion Matrix](/images/D3ConfusionMatrix.png)

### Imbalanced Classification Report

![Deliverable 1 Imbalanced Classification Report](/images/D1Classification.png)

![Deliverable 2 Imbalanced Classification Report](/images/D2Classification.png)

![Deliverable 3 Imbalanced Classification Report](/images/D3ClassificationReport.png)

## Summary: 
The results above show the differences that can be found with varying precision and sensitivity for the different methods.  All methods have a high (1.00) precision for prediction of `low_risk`. However, in all cases the precision for `high_risk` is extremely low.  With all but the `Easy Ensemble Classifier` also having a not great scores for predicting `high_risk` sensitivity(recall).  This is reflected in the low `F1 scores` for `high_risk` as well.   For all these reasons I would not recommend any of the models to accurately predict credit risk.
