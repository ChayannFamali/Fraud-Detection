# Fraud-Detection
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.
Credit Card Fraud Detection is an actual banking task. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
It contains only numerical input variables which are the result of a PCA transformation.
Fraudulent transactions have a distribution more even than valid transactions.
As expected, there is no notable correlation between features V1-V28.
Then we brought all the data to a normal distribution, and then eliminated the imbalance of classes using the ADASYN algorithm (this is necessary to prevent the process of retraining). 3 algorithms were used as learning models: lightgbm, catboost and random forest. All of them showed themselves perfectly. Feature importance graphs are also constructed, which show the significance of a particular variable.
The dataset is available at the following link: https://www.kaggle.com/mlg-ulb/creditcardfraud
