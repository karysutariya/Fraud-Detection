# SOEN 6111 Project Summary

## Fraud Detection In Banking or e-commerce:

Fraud detection is a series of actions used to stop the theft of money or other assets. Many businesses, including banking and insurance, use fraud detection. According to Federal Trade Commission of the U.S.A, in 2021, consumers have lost more than $5.8 billion[1]. Forging checks or utilizing credit cards that were stolen are two examples of banking fraud.The advantages of fraud detection and prevention include the ability to prevent fraudsters from taking the credit card numbers or loyalty points linked to your customers' accounts. As a result, you give customers a better experience.

### DATASET AND ITS CHARACTERISTICS:

Dataset: IEEE-CIS Fraud dataset[2]

In this Project, we are investigating a prediction about the likelihood that an online transaction is fraudulent, as indicated by the binary target “isFraud”. 

Description of Dataset: Dataset is divided into 5 files which are as per below.
1) sample_submission.csv
2) test_identity.csv
3) test_transaction.csv
4) train_identity.csv
5) train_transaction.csv

train_transaction.csv and train_identity.csv:- These files contain the data which will be used to train the model on. 

test_transaction.csv and test_identity.csv: - Files are needed to find out accuracy of models. 

sample_submission.csv - a sample submission file.

The categorical features used for these data sets are:
TRANSACTION: ProductCD, card1 - card6, addr1, addr2, P_emaildomain, R_emaildomain, M1 - M9.
CATEGORICAL: DeviceType, DeviceInfo, id_12 - id_38

### RESEARCH QUESTIONS:

The following research inquiries are addressed in our project:

1) Which class of models is applied to the dataset?
2) What all models are considered and how does each model perform compared to others?
3) Can we predict if the recall value is as close as possible?


The model that would fit right, is the parametric statistical classification model. The category of supervised machine learning includes classification models and when a classification model receives an input, it produces an output that categorizes the input.

We have also made sure our project uses various algorithms to show the comparative analysis. We have compared three algorithms such as RandomForest, Boosting (XGBoost), Logistic Regression.

Random forest has a higher true and false positive rate as the number of explanatory variables increases in a dataset, but logistic regression works better when the number of noisy variables is less than or equal to the number of explanatory variables. Gradient-boosted decision trees and other gradient-boosted models are typically trained with XGBoost. When compared to gradient-boosted decision trees, random forests use a different training approach but the same model representation and inference.

Our group will prepare the data by cleaning and preprocessing it i.e taking care of any missing data, encoding and get rid of extraneous and pointless features, which will be done through Spark Dataframes. This cleaned data will be then applied to the machine learning models for further processing.


Reference:
[1] Jay Mayfield. (February 22, 2022). New Data Shows FTC Received 2.8 Million Fraud Reports from Consumers in 2021. https://www.ftc.gov/news-events/news/press-releases/2022/02/new-data-shows-ftc-received-28-million-fraud-reports-consumers-2021-0
[2] IEEE Computational Intelligence Society. (2020). IEEE-CIS Fraud Detection. https://www.kaggle.com/competitions/ieee-fraud-detection/data

