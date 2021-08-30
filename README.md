# Credit_Risk_Analysis

## Overview of Project

### Purpose
The purpose of this analysis to find the results from a unbalanced data. 
We need to balance the data before analysing to eliminate the biases. 


## Results

### Using Random oversampling 
1. The difference in data points between low risk and high risk is 51k with data points in low risk being high.
2. Using oversampling we increased the data points for high risk to match low risk. 
![](./Images/RandomOversampling_ConfusionMatrix.PNG)

3. Imbalanced classification report
![](./Images/RandomOversampling_ImbalancedClassificationReport.PNG)

4. The accuracy score is 0.605141273224779

### Using SMOTE oversampling 
1. Using SMOTE oversampling technique we increased the data points for high risk to match the low risk. 
![](./Images/SMOTE_ConfusionMatrix.PNG)

2. Imbalanced classification report using oversampling. 
![](./Images/SMOTE_ImbalancedCLassificationReport.PNG)

3. Accuracy score is 0.6282240935571483


Looking at the output data, both the methods of oversampling the data generates almost similiar results. 
The difference in true positive values is only 3. Also the difference between the accuracy score is only 2%.

### Using Cluster Centroids algorithm for undersampling
1. In this method, the low risk data points are undersampled to 255 from 51357

2. Confusion Matrix
![](./Images/UnderSampling_ConfusionMatrix.PNG)

3. Imbalanced classification report
![](./Images/Undersampling_ImbalancedClassificationReport.PNG)

4. Accuracy score is 0.6282240935571483

### Using combined algorithm : SMOTEENN
1. Confusion Matrix
![](/Images/SMOTEENN_confusionMatrix.PNG)

2. Imbalanced classfication report
![](/Images/SMOTE_ImbalancedCLassificationReport.PNG)

3. Accuracy score is 0.5470624091174319




### Using Balanced Random Forest Classifier
1. This technique uses many decision trees. It establishes outcome based on predictions of decision trees. 

2. Confusion Matrix
![](./Images/BalancedRandomForestClassifier_confusionMatrix.PNG)

3. Accuracy score is 0.7814373765816665

4. Imbalanced classfication report
![](./Images/BalancedRandomForestClassifier_ImbalancedClassificationReport.PNG)

### Using Easy Ensemble AdaBoost Classifier

1. Confusion Matrix
![](./Images/adaboost_confusionMatrix.PNG)

2. Accuracy score is  : 0.9178773283613644

3. Imbalanced classification report
![](./Images/adaboost_imbalancedClassificationReport.PNG)

## Summary
1. Out of all the methods, the accuracy score of decision trees was much higher. 
2. All the 4 resampling methods had almost same accuracy score. 
3. Both the oversampling methods(random and SMOTE) have nearly equivalent accuracy score. 
3. AdaBoost classfier is the model recommended to use having accuracy score of 0.917. 
