## Credit Risk Analysis

## Overview
We are using different algorithms from the imbalanced-learn and scikit-learn libraries in order to accurately assess which loans are riskier for banks to lend credit to.

We will determine from the classification reports generated after each algorithmic test whether the model itself is the most sensitive in predicting credit risk.

The reason that sensitivity value will be used to determine credit risk is because it is preferable for a model to detect loans which might be risky, even if it meant that there were false positives. The model should ideally not miss any loans which are risky upon close examination by the bank.

## Summary

* Naive Random Oversampling results: 
    ..- Balanced accuracy test: 64.9%
    ..- Precision for the high_risk: 1%
    ..- Recall: 65%

![Random Oversampling](https://github.com/namin1993/Credit_Risk_Analysis/blob/acc0a5a4e3b1a47a9d778aee6ebc06416bdb7ad9/Screenshots/Random_Oversampling.png)


* SMOTE Oversampling results: 
    ..- Balanced accuracy test: 61.6%
    ..- Precision for the high_risk: 1%
    ..- Recall: 64%

![SMOTE Oversampling](https://github.com/namin1993/Credit_Risk_Analysis/blob/acc0a5a4e3b1a47a9d778aee6ebc06416bdb7ad9/Screenshots/SMOTE_Oversampling.png)


* Cluster Centroids Undersampling results:
    ..- Balanced accuracy test: 52.5%
    ..- Precision for the high_risk: 1%
    ..- Recall: 45%

![Cluster Centroids Undersampling](https://github.com/namin1993/Credit_Risk_Analysis/blob/acc0a5a4e3b1a47a9d778aee6ebc06416bdb7ad9/Screenshots/ClusterCentroids_Undersampling.png)


* SMOTEENN Sampling results:
    ..- Balanced accuracy test: 63.2%
    ..- Precision for the high_risk: 1%
    ..- Recall: 56%

![SMOTEENN Sampling](https://github.com/namin1993/Credit_Risk_Analysis/blob/acc0a5a4e3b1a47a9d778aee6ebc06416bdb7ad9/Screenshots/SMOTEENN_Sampling.png)


* Balanced Random Forest Sampling results:
    ..- Balanced accuracy test: 99.9%
    ..- Precision for the high_risk: 83%
    ..- Recall: 100%

![Balanced Random Forest](https://github.com/namin1993/Credit_Risk_Analysis/blob/acc0a5a4e3b1a47a9d778aee6ebc06416bdb7ad9/Screenshots/Balanced_Random_Forest.png)

* AdaBoost Sampling results:
    ..- Balanced accuracy test: 100%
    ..- Precision for the high_risk: 100%
    ..- Recall: 100%

![AdaBoost](https://github.com/namin1993/Credit_Risk_Analysis/blob/acc0a5a4e3b1a47a9d778aee6ebc06416bdb7ad9/Screenshots/AdaBoost.png)


## Results

The first 4 models involved oversampling, undersampling, and creating a balanced combination of both in order to predict which loans from the dataset were categorized at the highest risk.

The AdaBoost and Random Forest ensemble models repeatedly sample or divide the test dataset into several samples respectively in order to accurately predict loan risk.

Judging by the overall balance of Accuracy, Precision, and Recall percentages, the AdaBoost Classifier algorithm is the best algorithm to select since all results come to 100%.
