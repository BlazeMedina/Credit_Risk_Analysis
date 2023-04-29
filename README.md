# Credit_Risk_Analysis

## Overview of the analysis


In this project, I use Python to build and evaluate several machine learning models to predict credit risk.  I used the following models from two different techniques:

* Resampling Technique
	1) Naive Random Sampling (RandomOverSample)
	2) SMOTE Oversampling
	3) ClusterCentroids Undersampling
	4) Combination of Over and Under Sampling (SMOTEEN)
* Ensemble Learners Technique
	1) Balanced Random Forest Classifier
	2) Easy Ensemble AdaBoost Classifier

Using these models, we will evaluate their performance make a recommendation on which should be used to predict credit risk.

## Results

- **Resampling**
	-  **Naive Random Oversampling**
		- Balanced accuracy score: 64.8%
		- Precision score: 99%
		- Recall score: 59%
		- F-Measure: 74%
	- **SMOTE Oversampling**
		- Balanced accuracy score: 66.3%
		- Precision score: 99%
		- Recall score: 69%
		- F-Measure: 81%
	- **Undersampling ClusterCentroids** 
		- Balanced accuracy score: 55.4%
		- Precision score: 99%
		- Recall score: 40%
		- F-Measure: 56%
	- **Combination (SMOTEEN)** 
		- Balanced accuracy score: 64.8%
		- Precision score: 99%
		- Recall score: 58%
		- F-Measure: 72%
- **Ensemble Learners**
	-  **Balanced Random Forest Classifier**
		- Balanced accuracy score: 78.9%
		- Precision score: 99%
		- Recall score: 87%
		- F-Measure: 93%
	- **Easy Ensemble AdaBoost Classifier**
		- Balanced accuracy score: 93.2%
		- Precision score: 99%
		- Recall score: 94%
		- F-Measure: 97%

##  Screenshots

**Naive Random Oversampling**

![Naive Random Oversampling](https://github.com/BlazeMedina/Credit_Risk_Analysis/blob/main/Images/Naive_Random_Oversampling.png)

**SMOTE Oversampling**

![SMOTE Oversampling](https://github.com/BlazeMedina/Credit_Risk_Analysis/blob/main/Images/SMOTE_Oversampling.png)

**ClusterCentroids Undersampling**

![ClusterCentroids Undersampling](https://github.com/BlazeMedina/Credit_Risk_Analysis/blob/main/Images/Undersampling_ClusterCentroids.png)

**Combination (Over and Under) Sampling**

![Combination (Over and Under) Sampling](https://github.com/BlazeMedina/Credit_Risk_Analysis/blob/main/Images/Combination_Over_Under_Sampling.png)

**Balanced Random Forest Classifier**

![Balanced Random Forest Classifier](https://github.com/BlazeMedina/Credit_Risk_Analysis/blob/main/Images/Balanced_Random_Forest_Classifier.png)

**Easy Ensemble AdaBoost Classifier**
![Easy Ensemble AdaBoost Classifier](https://github.com/BlazeMedina/Credit_Risk_Analysis/blob/main/Images/Easy_Ensemble_AdadBoost_Classifier.png)
## Summary
**F-Measure**  = (2 * Precision * Recall) / (Precision + Recall)
The F-Measure combines precision and recall a single score that seeks to balance both concerns, it is a popular metric for imbalanced classification.

The first four models use resampling techniques.  The highest F-Measure of the four models is 81% for the SMOTE Oversampling technique.  The last two models used ensemble learners.  The Balanced Random Forest Classifier had an F-Measure 93%.  The Easy Ensemble AdaBooster Classifier had an F-Measure 97%.

It is clear that **Easy Ensemble AdaBooster Classifier** model is the superior one for determining credit risk with the provided data.
