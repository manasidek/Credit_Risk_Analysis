# Credit_Risk_Analysis

## Overview

- The purpose of this analysis is to evaluate the performance of machine learning models that reduce bias to determine whether they should be used to predict credit risk. Credit risk is an inherently unbalanced classification problem due to good loans outnumbering risky loans, so it was necessary to use different techniques to sample data, and train and evaluate models for such unbalanced classes.

## Results

### Scripts

	1. Resampling [resample]()

	2. Ensemble [ensemble]()

### Data

- The features data frame is:

![X_describe]()

- The target vector is:

![target]()

### Resampling Models

- Random Over Sampling

	- Balanced accuracy score is 66.49%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 73% and for low risk is 60%

![acc_ROS]()

![class_ROS]()


- SMOTE Oversampling

	- Balanced accuracy score is 66.23%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 63% and for low risk is 69%

![acc_SMOTE]()

![class_SMOTE]()

- Undersampling (Cluster Centroids)

	- Balanced accuracy score is 54.47%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 69% and for low risk is 40%

![acc_cc]()

![class_cc]()

- Combination (Over and Under) Sampling (SMOTEENN)

	- Balanced accuracy score is 63.89%

	- Precision score for high risk is 0.01 and for low risk is 1.00
	
	- Recall rate for high risk is 70% and for low risk is 57%

![acc_een]()

![class_een]()

### Ensemble Models

- Balanced Random Forest Classifier

	- Balanced accuracy score is 78.87%

	- Precision score for high risk is 0.03 and for low risk is 1.00
	
	- Recall rate for high risk is 70% and for low risk is 87%

![acc_BRFC]()

![class_BRFC]()

- Features in descending order:

![features]() 

- Easy Ensemble AdaBoost Classifier

	- Balanced accuracy score is 93.16%

	- Precision score for high risk is 0.09 and for low risk is 1.00
	
	- Recall rate for high risk is 92% and for low risk is 94%

![acc_ada]()

![class_ada]()

## Summary

- Random Over Sampling

![cm_ROS]()

- SMOTE Oversampling

![cm_SMOTE]()

- Undersampling (Cluster Centroids)

![cm_cc]()

- Combination (Over and Under) Sampling (SMOTEENN)

![cm_een]()

- Balanced Random Forest Classifier

![cm_BRFM]()

- Easy Ensemble AdaBoost Classifier

![cm_ada]()



