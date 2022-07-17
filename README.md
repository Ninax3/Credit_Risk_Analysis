# Credit Risk Analysis - A comparison of machine learning techiniques

## Overview 
The Lending Club, a lending company, has provided a credit card risk dataset to build training & testing datasets, to analyze and recommend a machine learning model to identify high-risk customers for credit risk. The following machine learning models/techniques are applied and evaluated:

1. **RandomOverSampler** algorithm *(resampling; oversample)*
2. **SMOTE** algorithm *(resampling; oversample)*
3. **ClusterCentroids** algorithm *(resampling; undersample)*
4. **SMOTEEN** algorithm *(resampling; combination of oversample and undersample)*
5. **BalancedRandomForestClassifier** *(ensemble; undersample bootstrap sample)*
6. **EasyEnsembleClassifier** *(ensemble; undersample with balance boosted learners)*

## Results

#### RandomOverSampler
![Credit_Risk_Analysis "RandomOverSampling_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/RandomOverSampling_bas.png)

![Credit_Risk_Analysis "RandomOverSamp_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/RandomOverSamp_ClassR.png)

#### SMOTE
![Credit_Risk_Analysis "SMOTE_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_bas.png)

![Credit_Risk_Analysis "SMOTE_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_ClassR.png)

#### ClusterCentroids
![Credit_Risk_Analysis "ClusterC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_bas.png)


#### SMOTEEN

![Credit_Risk_Analysis "SMOTEEN_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_cm.png)
![Credit_Risk_Analysis "SMOTEEN_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_ClassR.png)

#### BalancedRandomForestClassifier


#### EasyEnsembleClassifier

## Summary 
