# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to introduce and apply different types of supervised machine learning techniques:

- Linear Regression and Classification
- Logistic Regression
- Classification Model Validation
- Support Vector Machines (SVM)
- Data Reprocessing
- Decision Trees
- Ensemble Learning and Random Forests
- Bagging and Boosting
- Resolving Class Imblanace

## Results
Legend: 0 = HIGH RISK / 1 = LOW RISK

INSERT HERE
Figure 1. Naive Random Oversampling 

INSERT HERE
Figure 2. SMOTE Oversampling

INSERT HERE
Figure 3. Undersampling: Cluster Centroids

INSERT HERE
Figure 4. Combination (Over and Under) Sampling (SMOTEENN)

INSERT HERE
Figure 5. Balanced Random Forest Classifier

INSERT HERE
Figure 6. Easy Ensemble AdaBoost Classifier

Figure 1 and Figure 2 look almost identical. In these figures, precision is extremely high for low risk and extremely low for high risk showing that tis is not a very good model due to the fact that there are no real cases where we should expect 100% precision for anything. If we ever do then we should be speculative of our data and/or our techniques getting to that point. The sensitivity for both low and high risks are about the same, and show a plausible result. F1 score drops for the high risk and goes up for the low risk, and that is because of the way f1 score is found, takes into account both sensitivity and precision. The accuracy seems to be pretty low as well.

For Figure 3, high risk's precision is extremely low, sensitivity is below average, and f1 score is really low. Low risk's precision is really high, sensitvity is below average, and f1 score is also below average. The accuracy is not much better than the first two figures. Precision is almost identical for both high risk and low risk in the reaminding figures. As for Figure 4's, high risk's sensitivity it is average, but f1 score is still really low. Low risk's sensitivity is below average, but f1 score is average. 

Figure 5, has a much better balanced accuracy compared to any of the other images thus far. The high risk's sensitivity is average and f1 score is really low. Low risk's sensitvity is above average, and the f1 score is even higher.

Figure 6, has the best balanced accuracy score with a ~92.6%. The senistivity for the both high risk and low risk are above average, but the f1 score is low for the high risk and high for the low risk. 

## Summary
In conclusion, the Easy Ensemble AdaBoost Classifier is probrably the best model for us to use given the data that we have when we want high sensitivity.