# Credit Risk Analysis

## Overview

### Purpose

The purpose of this analysis is to apply machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, different techniques are employed to train and evaluate models with unbalanced classes. Libraries such as imbalanced-learn and scikit-learn are used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms, and the data is undersampled using the ClusterCentroids algorithm. Furthermore, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm is used as well. Next, two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, are compared to predict credit risk. Finally, the performance of these models is evaluated to recommend on whether they should be used to predict credit risk.

<p float="left">
  <img src="Images/loan.png" width="400" height="350" />
  <img src="Images/loan1.png" width="400" height="350" />
</p>

<p>&nbsp;</p>

## Results

### Dataset and Files

The analysis is based on the following: 

* Credit card credit dataset from LendingClub: [LoanStats_2019Q1](LoanStats_2019Q1.csv.zip)
* Resampling Models and the SMOTEENN algorithm to Predict Credit Risk: [credit_risk_resampling](credit_risk_resampling.ipynb)
* Ensemble Classifiers to Predict Credit Risk: [credit_risk_ensemble](credit_risk_ensemble.ipynb)

### Software and Application

* Python 3.7.9 
* Jupyter Notebooks 6.1.4

### Outcomes 

Six machine learning models were used to evaluate the credit card credit dataset from LendingClub to determine which is better at predicting credit risk. These six machine learning models are the following:

* Oversampling  - RandomOverSampler
* Oversampling  - SMOTE
* Undersampling - ClusterCentroids
* Combinatorial - SMOTEENN
* Ensemble Classifiers - BalancedRandomForestClassifier
* Ensemble Classifiers - EasyEnsembleClassifier

Below is a brief summary of the performance of all six machine learning models.

* **Oversampling  - RandomOverSampler**

![Random_Oversampling](Images/Random_Oversampling.png)
<p>&nbsp;</p>

* **Oversampling  - SMOTE (Synthetic Minority Oversampling Technique)**

![SMOTE](Images/SMOTE.png)
<p>&nbsp;</p>

* **Undersampling - ClusterCentroids**

![ClusterCentroids](Images/ClusterCentroids.png)
<p>&nbsp;</p>

* **Combinatorial - SMOTEENN (SMOTE and Edited Nearest Neighbors (ENN))**

![SMOTEENN](Images/SMOTEENN.png)
<p>&nbsp;</p>

* **Ensemble Classifiers - BalancedRandomForestClassifier**

![Forest](Images/Forest.png)
<p>&nbsp;</p>

* **Ensemble Classifiers - EasyEnsembleClassifier**

![Easy](Images/Easy.png)
<p>&nbsp;</p>

## Summary

Machine learning is a very powerful tool that can handle and analyze risk on large datasets. In this analysis, 6 different machine learning models were used on the same dataset to predict credit risk, although each model has its own strengths and weaknesses. With that stated, the EasyEnsembleClassifier model had the best outcome. It is found that the EasyEnsembleClassifer model had an accuracy rate of 93.2% and a 9% precision rate when predicting "High Risk" applications. The recall rate is at 92% while the F1 score was at 16%. And so, it is recommended to use the EasyEnsembleClassifier model to predict credit risk.

In conclusion, using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms, and the data is undersampled using the ClusterCentroids algorithm. Furthermore, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm is used as well. Next, two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, are compared to predict credit risk. Finally, the performance of these models is evaluated to recommend on whether they should be used to predict credit risk.

<p float="left">
  <img src="Images/loan2.png" width="500" height="300" />
</p>

