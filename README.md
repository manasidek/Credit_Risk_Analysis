# Credit_Risk_Analysis

## Overview

- The purpose of this analysis is to evaluate the performance of machine learning models that reduce bias to determine whether they should be used to predict credit risk. Credit risk is an inherently unbalanced classification problem due to good loans outnumbering risky loans, so it was necessary to use different techniques to sample data, and train and evaluate models for such unbalanced classes.

## Results

### Scripts

1. Resampling [resample](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)

2. Ensemble [ensemble](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)

### Data

- The features data frame is:

![X_describe](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/X_describe.png)

- The target vector is:

![target](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/target.png)

### Resampling Models

- Random Over Sampling

	- Balanced accuracy score is 66.49%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 73% and for low risk is 60%

![acc_ROS](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/acc_ROS.png)

![class_ROS](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/class_ROS.png)


- SMOTE Oversampling

	- Balanced accuracy score is 66.23%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 63% and for low risk is 69%

![acc_SMOTE](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/acc_SMOTE.png)

![class_SMOTE](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/class_SMOTE.png)

- Undersampling (Cluster Centroids)

	- Balanced accuracy score is 54.47%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 69% and for low risk is 40%

![acc_cc](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/acc_cc.png)

![class_cc](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/class_cc.png)

- Combination (Over and Under) Sampling (SMOTEENN)

	- Balanced accuracy score is 63.89%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 70% and for low risk is 57%

![acc_een](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/acc_een.png)

![class_een](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/class_een.png)

### Ensemble Models

- Balanced Random Forest Classifier

	- Balanced accuracy score is 78.87%

	- Precision score for high risk is 0.03 and for low risk is 1.00
	
	- Recall rate for high risk is 70% and for low risk is 87%

![acc_BRFC](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/acc_BRFC.png)

![class_BRFC](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/class_BRFC.png)

- Features in descending order:

![features](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/features.png) 

- Easy Ensemble AdaBoost Classifier

	- Balanced accuracy score is 93.16%

	- Precision score for high risk is 0.09 and for low risk is 1.00
	
	- Recall rate for high risk is 92% and for low risk is 94%

![acc_ada](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/acc_ada.png)

![class_ada](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/class_ada.png)

## Summary

- Random Over Sampling

![cm_ROS](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/cm_ROS.png)

- SMOTE Oversampling

![cm_SMOTE](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/cm_SMOTE.png)

- Undersampling (Cluster Centroids)

![cm_cc](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/cm_cc.png)

- Combination (Over and Under) Sampling (SMOTEENN)

![cm_een](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/cm_een.png)

- Balanced Random Forest Classifier

![cm_BRFM](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/cm_BRFC.png)

- Easy Ensemble AdaBoost Classifier

![cm_ada](https://github.com/manasidek/Credit_Risk_Analysis/blob/main/Images/cm_ada.png)



