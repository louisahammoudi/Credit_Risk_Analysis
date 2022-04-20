# Credit_Risk_Analysis

## Overview of the analysis: 

Overview
The purpose of this analysis was to build and evaluate various machine learning models to evaluate individual customer credit risk. The dataset used to train the models was from LendingClub, "a peer-to-peer lending services company." After being cleaned, the dataset consisted of 68,817 entries, and was heavily unbalanced, with only 0.5% of entries being classified as "high-risk." High-Low Risk Split

The machine learning algorithms used were:

RandomOverSampler
SMOTE
ClusterCentroids
SMOTEENN
BalancedRandomForestClassifier
EasyEnsembleClassifier
The models were run and then evaluated for performance and accuracy at predicting credit risk.

## Results: 

- Naive Random Oversampling results: Our balanced accuracy test it 67%, the precision for the high_risk has a very low positivity at 1% and the recall is 74%
<img width="1382" alt="naive" src="https://user-images.githubusercontent.com/67278193/99189208-2bb20d00-272e-11eb-8616-de6011dece3b.png">

- SMOTE oversampling results: the accuracy score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall
<img width="1286" alt="smote" src="https://user-images.githubusercontent.com/67278193/99189213-2e146700-272e-11eb-87e1-3d7f80ba662a.png">

- Undersampling results: balanced accuracy score is 66.2% overall, the precision is at 99% and the recall is 41%
<img width="1315" alt="undersampling" src="https://user-images.githubusercontent.com/67278193/99189216-31a7ee00-272e-11eb-88d0-de8b0acb1411.png">

- Combination(over and undersampling) results: balanced accuracy score is 54.7% the precision is 99% and the recall is 57% overall
<img width="1355" alt="combination" src="https://user-images.githubusercontent.com/67278193/99189223-34a2de80-272e-11eb-8044-b988f1a57823.png">

- Balanced Random Forest Classifier results: the accuracy score is 77.2% the precision is 99% and the recall is 88%
<img width="1293" alt="random forest" src="https://user-images.githubusercontent.com/67278193/99189228-366ca200-272e-11eb-8f97-78bdacff4a43.png">

- Easy Ensemble AdaBoost Classifier results: the accuracy score is 91.7% the precision is 99% and the recall is 94%
<img width="1353" alt="ensemble" src="https://user-images.githubusercontent.com/67278193/99189232-3a002900-272e-11eb-8077-9695c40fcc83.png">

## Summary: 

In conclusion, credit-risk is a difficult thing to predict, even for advanced machine learning algorithms with 93 columns of data to process. While the Easy Ensemble AdaBoost Classifier model had the highest overall accuracy, this was largely due to the fact that the dataset was so radically unbalanced. Even when it's balanced accuracy and average F-score were above 90%, it's F-score for high-risk prediction was no better than 0.16. In the end, I would advise against using any of these algorithms, as it would put creditors as too great of risk being unable to accurately predict who the high-risk clients/debtors would be.
