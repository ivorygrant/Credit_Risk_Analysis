# Results of Analysis

## Overview

The purpose of this analysis is to experiment with Logistic Regression and Ensemble algorithms, in conjunction with Oversampling and Undersampling techniques.

## Results

Please refer to the accompanying notebooks for code used. The following list summarizes the results of the analysis:

### Logistic Regression 

#### Naive Random Oversampling

* Balanced Accuracy Score:

![](images/naive_random_oversampling_bas.png)

* Classification Report

![](images/naive_random_oversampling_cr.png)

#### SMOTE

* Balanced Accuracy Score:

![](images/smote_oversampling_bas.png)

* Classification Report

![](images/smote_oversampling_cr.png)

#### Undersampling

* Balanced Accuracy Score:

![](images/undersampling_bas.png)

* Classification Report

![](images/undersampling_cr.png)

#### SMOTEENN

* Balanced Accuracy Score:

![](images/smoteenn_bas.png)

* Classification Report

![](images/smoteenn_cr.png)

### Ensemble Algorithms

#### Balanced Random Forest

* Balanced Accuracy Score:

![](images/brf_bas.png)

* Classification Report

![](images/brf_cr.png)

#### Easy Ensemble AdaBoost

* Balanced Accuracy Score:

![](images/eea_bas.png)

* Classification Report

![](images/eea_cr.png)

## Discussion

Based on the analysis above, I would recommend the use of Easy Ensemble AdaBoost classifier. This model received the highest accuracy score. The precision for this model comes in at 0.07, meaning that if the transaction is fraudulent, there is actually a very low chance that it is indeed fraudulent. However, the recall/sensitivity of this model is 0.90, meaning that of all fraudulent transactions, the model was able to correctly recognize 90% of those transactions. This combined with the high accuracy score is why I would recommend this model.