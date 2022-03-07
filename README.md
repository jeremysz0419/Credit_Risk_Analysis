# Credit_Risk_Analysis

## Analysis Overview
For this analysis, we utilized Python to build several machine learning models toe predict credit risks based on our data of people's profiles and credit history. 
For this analysis we performed the following:
  - oversampling using the RandomOverSampler and SMOTE algorithm 
  - Undersampling using the ClusterCentroids algorithm
  - Under and oversampling using the ClusterCentroids algorithm
  - Using multiple machine learning models to reduce skews and bias with BalancedRandomForestClassifier and EasyEnsembleClassifier algorithm


## Resources
- Data Source: LoanStats.csv
- Software: Python 3.7.9, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results (Balanced Accuracy Scores, Confusion Matrixes and Imbalanced Classification Reports)

### RandomOverSampler model

With our RandomOVerSampler model we received the following results:
  - Balanced Accuracy Score: 65%
  - high risk population: The precision is only around 1% with a sensitivity of 71% and a F1 of 2%.
  - low risk population: The precision is 100% due to the large amount of population and a sensitivity of 60%.
<br><br>

### SMOTE model

With our SMOTE model we received the following results:
- Balanced Accuracy Score: 65%
  - high risk population: The precision is only around 2% with a sensitivity of 61% and a F1 of 2%.
  - low risk population: The precision is 100% due to the large amount of population and a sensitivity of 69%.
<br><br>

### ClusterCentroids model

With our ClusterCentroids model we received the following results:
- Balanced Accuracy Score: 54%
  - high risk population: The precision is only around 1% with a sensitivity of 69% and a F1 of 1%.
  - low risk population: The precision is 100% due to the large amount of population and a sensitivity of 40%.

<br><br>

### SMOTEENN model

- Balanced Accuracy Score: 65%
  - high risk population: The precision is only around 1% with a sensitivity of 72% and a F1 of 2%.
  - low risk population: The precision is 100% due to the large amount of population and a sensitivity of 58%.
<br><br>

### BalancedRandomForestClassifier model

- Balanced Accuracy Score: 78%
  - high risk population: The precision is only around 3% with a sensitivity of 70% and a F1 of 6%.
  - low risk population: The precision is 100% due to the large amount of population and a sensitivity of 87%.
<br><br>

### EasyEnsembleAdaBoost model

- Balanced Accuracy Score: 93%
  - high risk population: The precision increased 9% with a sensitivity of 92% and a F1 of 16%.
  - low risk population: The precision is 100% due to the large amount of population and a sensitivity of 94%.
<br><br>

## Summary
One of the main concerns of using these models is that the precision for most of these models are relatively low. This indicates that while most high risk credit profiles are detected, there are a lot of false positives of low risk profiles marked as high risk. While banks may use this to deter customers with high default risks, it poses a damage to their customer demand as they would turn away a lot of potential loans that are in reality low risk. Therefore, I would recommend the bank to reconsider other methods of detecting high risk default probabilities within their customers. 
