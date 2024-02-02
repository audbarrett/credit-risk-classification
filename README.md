## Overview of the Analysis

* The purpose of this analysis is to train and evaluate a model based on loan risk.
* A dataset of historical lending activity from a peer-to-peer lending services company is used to build a model that can identify the creditworthiness of borrowers.

## Results

* Machine Learning Model 1 (using original data):
  * Description of Model 1 Accuracy, Precision, and Recall scores:
    * This logistic regression model of the original data appears to do a nearly perfect job predicting healthy loans (1.00 f1-score) and a strong job predicting unhealthy loans (0.88 f1-score). The scores for the model overall are as follows:
      * Balanced Accuracy Score: 95.2%
      * Precision (Macro Avg): 92%
      * Recall (Macro Avg): 95%

* Machine Learning Model 2 (using oversampled data):
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    * This logistic regression model of the oversampled data still predicts healthy loans at a nearly perfect rate (1.00 f1-score) and its ability to predict unhealthy loans is higher than with the unbalanced data (0.91 f1-score). This leads to higher averages for the model. The scores for the model overall are as follows:
      * Balanced Accuracy Score: 99.37%
      * Precision (Macro Avg): 92%
      * Recall (Macro Avg): 99%

## Summary

* The machine learning model using oversampled data shows stronger scores than the model using unbalanced data. Most notably, its ability to predict un-healthy loans is higher than that of the first model. I would recommend this model for that reason.
* A lending company would most likely want to prioritize a model that predicts unhealthy loans as accurately as possible. While it could be detrimental to a company to mark a healthy loan as unhealthy, it would likely be more costly and detrimental to mismark an unhealthy loan as healthy.

## Instructions:
1. Clone repo to local device.
  * copy HTTPS link from repo
  * in terminal, use following command: `git clone` + [paste HTTPS]

![Alt text](/screenshot_1.png?raw=true)

2. Open python file in Jupyter Notebook
  * Natigate to file in terminal
  * Use following command: `jupyter notebook`

![Alt text](/screenshot_2.png?raw=true)

3. Run all cells in Jupyter Notebook

![Alt text](/screenshot_3.png?raw=true)

## Credits
Code completed with help from AskBCS Learning Assistant. Following code was shared:
` !pip uninstall scikit-learn --yes
  !pip uninstall imblearn --yes
  !pip install scikit-learn==1.2.2
  !pip install imblearn `
