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
- Oversampling the minority class of high_risk features, the Balanced Accuracy Score is 65% which is a *satisfactory* metric for sensitivity and specificity.
- The precision is 1% with a sensitivity of 62% for the high_risk class.
- The F1 score which measures precision and sensitivity is a poor 2%.


#### SMOTE
![Credit_Risk_Analysis "SMOTE_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_bas.png)
![Credit_Risk_Analysis "SMOTE_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_cm.png)
![Credit_Risk_Analysis "SMOTE_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTE_ClassR.png)
- Synthetic minority oversampling of high_risk features, the Balanced Accuracy Score is 64%, which is a *satisfactory* metric. 
- The precision is 1% with a sensitivity of 63% for the high_risk class. 
- The F1 score is a poor 2%.
- Results are almost identical to the RandomOverSampler.


#### ClusterCentroids
![Credit_Risk_Analysis "ClusterC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_bas.png)
![Credit_Risk_Analysis "ClusterC_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_cm.png)
![Credit_Risk_Analysis "ClusterC_ClsR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/ClusterC_ClsR.png)
- Undersampling the majority class of low_risk features, the Balanced Accuracy Score is 64%, which is a *satisfactory* metric. 
- The precision is 1% with a sensitivity of 60% for the high_risk class. 
- The F1 score is a poor 1%.
- The overall results are poor compared to the Oversampling techniques, RandomOverSampler and SMOTE. 


#### SMOTEEN
![Credit_Risk_Analysis "SMOTEEN_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_bas.png)
![Credit_Risk_Analysis "SMOTEEN_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_cm.png)
![Credit_Risk_Analysis "SMOTEEN_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/SMOTEEN_ClassR.png)
- Combines oversampling and undersampling in a two-step process, the Balanced Accuracy Score is 52%, which is a *bad* score. 
- The precision is 1% with a sensitivity of 72% for the high_risk class. 
- The F1 score is a poor 2%. 
- Although the recall/sensitivity score increased signficantly, the Balanced Accuracy Score decreased. Precision is more important for credit risk analysis, so this improvement is not necessarily a desired goal. 


#### BalancedRandomForestClassifier
![Credit_Risk_Analysis "BRFC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC_bas.png)
![Credit_Risk_Analysis "BRFC_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC_cm.png)
![Credit_Risk_Analysis "BRFC_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC_ClassR.png)
- This Ensemble learning model runs efficiently on large datasets and combines multiple models. The Balanced Accuracy Score is 79%, which is a *GOOD* score. 
- The precision is 4% with a sensitivity of 67% for the high_risk class. 
- The F1 score is an improved 7%.
- Thus far, this model has shown improvement in the areas aforementioned. 
- Shown below are the features sorted by rank used in this model.
![Credit_Risk_Analysis "BRFC_Features_Sorted"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/BRFC_Features_Sorted.png)


#### EasyEnsembleClassifier
![Credit_Risk_Analysis "EasyEnsembleABC_bas"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/EasyEnsembleABC_bas.png)
![Credit_Risk_Analysis "EasyEnsembleABC_cm"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/EasyEnsembleABC_cm.png)
![Credit_Risk_Analysis "EasyEnsembleABC_ClassR"](https://github.com/Ninax3/Credit_Risk_Analysis/blob/main/EasyEnsembleABC_ClassR.png)
- The Ensemble learning model with ADA boosters to created balanced datasets has a Balanced Accuracy Score of 93%, which is a *Very Good* score.
- The precision is 7% with a senstivity of 91% for the high_risk class. 
- The F1 score is an improved 14% and the best of all the models in this analysis.  

## Summary 
Overall the Ensemble models outperformed the Resampling models for the goal of identifying high_risk credit customers. Part of the challenge is the imbalanced classes and for which none of these models are highly accurate in identifying high_risk credit customers. However, the best machine learning model for the features in the dataset is the EasyEnsembleClassifier. Recommendations include:
1) Using the EasyEnsembleClassifier model as a baseline, but not a rule of law for determining credit worthiness. 
2) Further exploration is recommended to include other features (variables) which may improve the model's performance. 
