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
![Credit_Risk_Analysis "RandomOverS_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/RandomOverS_cm.png)
![Credit_Risk_Analysis "RandomOverSamp_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/RandomOverSamp_ClassR.png)

#### SMOTE
![Credit_Risk_Analysis "SMOTE_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_bas.png)
![Credit_Risk_Analysis "SMOTE_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_cm.png)
![Credit_Risk_Analysis "SMOTE_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_ClassR.png)

#### ClusterCentroids
![Credit_Risk_Analysis "ClusterC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_bas.png)
![Credit_Risk_Analysis "ClusterC_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_cm.png)
![Credit_Risk_Analysis "ClusterC_ClsR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_ClsR.png)

#### SMOTEEN
![Credit_Risk_Analysis "SMOTEEN_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_bas.png)
![Credit_Risk_Analysis "SMOTEEN_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_cm.png)
![Credit_Risk_Analysis "SMOTEEN_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_ClassR.png)

#### BalancedRandomForestClassifier
![Credit_Risk_Analysis "BRFC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC_bas.png)
![Credit_Risk_Analysis "BRFC"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC.png)
![Credit_Risk_Analysis "BRFC_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC_ClassR.png)

#### EasyEnsembleClassifier
![Credit_Risk_Analysis "EasyEnsembleABC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/EasyEnsembleABC_bas.png)
![Credit_Risk_Analysis "EasyEnsembleABC_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/EasyEnsembleABC_cm.png)
![Credit_Risk_Analysis "EasyEnsembleABC_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/EasyEnsembleABC_ClassR.png)

## Summary 
