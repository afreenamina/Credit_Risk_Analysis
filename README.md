# Credit_Risk_Analysis

### Overview of the analysis:

We are analysing credit card credit dataset from LendingClub, a peer-to-peer lending services company for credit card risk by evaluating differnt methods of machine learning models.

Below are the Machine Learning Models used in this analysis - 
  * RandomOverSampler
  * SMOTE Oversampling
  * ClusterCentroids Undersampling
  * SMOTEENN (Over and Under) Sampling
  * BalancedRandomForestClassifier 
  * EasyEnsembleClassifier

### Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

#### RandomOverSampler

* Balanced accuracy score is 64 % 

* Imbalanced Classification Report - 
    * Precision - Precision for high_risk is only 0.01 which is much lower than 1.0 of low_risk.
    * Recall - High Risk and Low risk recall values are almost in-line with each other with 0.62 and 0.66 respectively.

![Random Oversampling](https://user-images.githubusercontent.com/92698873/155941734-d2829c00-5eaa-40a3-af1f-651ff7a3f038.png)

#### SMOTE Oversampling

* Balanced accuracy score is 62 % 

* Imbalanced Classification Report - 
    * Precision - Precision for high_risk is only 0.01 which is much lower than 1.0 of low_risk.
    * Recall - High Risk and Low risk recall values are almost in-line with each other with 0.62 and 0.63 respectively.

![2_SMOTE](https://user-images.githubusercontent.com/92698873/155941760-86d2b244-de55-4010-88cc-e217d0ab28cc.png)

#### ClusterCentroids Undersampling

* Balanced accuracy score is 52 %.

* Imbalanced Classification Report - 
    * Precision - Precision for high_risk is only 0.01 which is much lower than 1.0 of low_risk.
    * Recall - High Risk recall value is 0.61 and Low risk recall value is 0.45

![3_Undersampling](https://user-images.githubusercontent.com/92698873/155941795-cc9c06e8-3746-4a5d-b393-07864c4d4973.png)

#### SMOTEENN (Over and Under) Sampling

* Balanced accuracy score is 62 %.

* Imbalanced Classification Report - 
    * Precision - Precision for high_risk is only 0.01 which is much lower than 1.0 of low_risk.
    * Recall - High Risk and Low risk recall values are almost in-line with each other with 0.66 and 0.60 respectively.

![4_ Combination](https://user-images.githubusercontent.com/92698873/155941810-3130d1aa-c62d-4da2-8826-df8fcdd05a01.png)

#### BalancedRandomForestClassifier 

* Balanced accuracy score is 78 %.

* Imbalanced Classification Report - 
    * Precision - Precision for high_risk is only 0.03 which is much lower than 1.0 of low_risk.
    * Recall - High Risk recall value is 0.68 and Low risk recall value is 0.90

![5_Balanced Random Forest Classifier](https://user-images.githubusercontent.com/92698873/155941831-9ec0cc09-85e3-4e69-b5de-f3423bf809cf.png)

#### EasyEnsembleClassifier

* Balanced accuracy score is 93 %.

* Imbalanced Classification Report - 
    * Precision - Precision for high_risk is only 0.07 which is lower than 1.0 of low_risk.
    * Recall - High Risk and Low risk recall values are almost in-line with each other with 0.91 and 0.94 respectively.

![6_AdaBoost](https://user-images.githubusercontent.com/92698873/155941857-7f093960-32dd-4cd9-bc1e-0407b45dae3d.png)

### Summary: 

From the above anlysis, I could recommend using EasyEnsembleClassifier model, as it has an accuracy score of 94% which is very impressive. And EasyEnsembleClassifier Sensitivity(recall) values is much higher for both low_risk and high_risk as High Sensitive data tend to be aggressive and they do a good job of detecting the intended targets.
