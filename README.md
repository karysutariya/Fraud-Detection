# Bigdata

According to Federal Trade Commission of the U.S.A, in 2021, consumers have lost more than $5.8 billion[1]. Many people lose their life savings in these frauds. Therefore, we are trying to develop a Fraud Detection system. This system could be of great use to multiple parties to potentially identify and take necessary actions in order to stop the theft of money or other assets. Many businesses, including banks, insurance companies, and other third party payment applications can use this system to prevent theft. The advantages of fraud detection and prevention include the ability to prevent fraudsters from stealing money when customers make online transections. This seemingly helps to ensure the safety and legitimacy of the transactions made.

The following research inquiries are addressed in our project:
1. How to identify that a transaction is fraud or not?
2. What are the characteritics of fraud transaction based on historical data?
3. Which model is perfect to identify fraud and prevent it before happening?
4. Is it possible to achieve 100% recall?

Dataset: IEEE-CIS Fraud dataset[2]

Description of Dataset:
Dataset is divided into 5 files which are as per below.
1. sample_submission.csv
2. test_identity.csv
3. test_transaction.csv
4. train_identity.csv
5. train_transaction.csv

train_transaction.csv and train_identity.csv - These files contain the data which will be used to train the model on.
test_transaction.csv and test_identity.csv - Files are needed to find out accuracy of models.
sample_submission.csv - a sample submission file.

In this Project, we are investigating a prediction about the likelihood that an online transaction is fraudulent, as indicated by the binary target “isFraud”. 

Fetures of dataset:
The categorical features in this data set are:
TRANSACTION: ProductCD, card1 - card6, addr1, addr2, P_emaildomain, R_emaildomain, M1 - M9.
CATEGORICAL: DeviceType, DeviceInfo, id_12 - id_38

The model that would fit the right is the statistical classification model. The category of supervised machine learning includes classification models and when 

This problem can be solved easily with supervised classification algorithm as per thoeries (threfore, will use other algorithm to test the thoeries). A classification model receives varies inputs, it produces a catagarised output. We have also made sure our project uses various algorithms to show the comparative analysis. We have used three algorithms such as Logistic Regression, RandomForest, Boosting (XGBoost).

Our group will prepare the data by cleaning and preprocessing it before applying it to the machine learning models. That is, take care of any missing data and encoding and get rid of extraneous and pointless features.

Extra information:
“Random forest has a higher true and false positive rate as the number of explanatory variables increases in a dataset, but logistic regression works better when the number of noisy variables is less than or equal to the number of explanatory variables.Gradient-boosted decision trees and other gradient-boosted models are typically trained with XGBoost. When compared to gradient-boosted decision trees, random forests use a different training approach but the same model representation and inference.”

Reference:  
[1] https://www.ftc.gov/news-events/news/press-releases/2022/02/new-data-shows-ftc-received-28-million-fraud-reports-consumers-2021-0

[2] https://www.kaggle.com/competitions/ieee-fraud-detection/data
