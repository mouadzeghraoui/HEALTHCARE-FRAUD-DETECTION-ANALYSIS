# Health Care Fraud Detection
## Problem Statement :

Health care fraud is a crime that involves misrepresenting information,  concealing information, or deceiving a person or entity in order to  receive benefits, or to make a financial profit. Both individuals and  healthcare providers commit health care fraud, in a number of different  ways.

**Healthcare Fraud =** submission of fraudulent claims by medical facilities to steal money from insurance companies.

Fraud claims come in different forms such as:

- Using insurance that belongs to someone else
- Failing to remove someone no longer eligible from a policy
- Providing false information in order to receive medical coverage
- Duplicating claims for the same or different patients
- Providing a service that is not covered under a patient’s insurance policy, then billing for a service that is covered

Health care Fraud  is a serious crime that affects everyone and should concern everyone. According to the National Health Care Anti-Fraud Association (NHCAA), the financial lose due to healthcare fraud is more than $100 billion every year, and have a lot of consequences such as: 

- Reduce benefits & coverage
- Increased cost of providing insurance benefits

Source : 

-  https://www.nhcaa.org/resources/health-care-anti-fraud-resources/the-challenge-of-health-care-fraud/
- https://legaldictionary.net/health-care-fraud/

## Goal : 

The Goal in this project is to **understand the behavior of potential fraud providers**, and **discover** the **important parameters** that can help us to to that, and finnally to **build a predictive model** that can  **flag the potential fraud providers** based on the **claims fields**

## Data Source : 

The dataset includes information about:

- Beneficiary like **Age, Race, Country, State, Gender**
- Inpatient/outpatient claims informations such as the **amount, Medical codes, Physician ID**
- Label (**Fraud** or **Not Fraud**)

## Exploratory Data Analysis

In this part, we merged our Training datasets by our unique IDs, for both providers and patients, and we generate a Data Report, to check the data description,  missing values, correlations .... 

All the features that have 100% missing values for all the observations were removed, and the others we need to investigate more, before we delete them.

After that we ran some initial data analysis, to understand the relationship between our features, and between our features and our target variable "PotentialFraud".

## Modelling strategy

In this part I train and Evaluate my Machine Learning models.

I have used Supervised Machine Learning algorithms to classify Fraudulent behavior of Healthcare providers.

1. Logistic Regression Classifier: In order to check linear behavior between dependent and independent variables
2. Random Forest Classifier : In order to check no linearity between variables, also Random Forrest has the power of handle large data set with higher dimensionality and identify most significant variables




## Model Evaluation 

Random forrest model:

```
Accuracy Train :  0.8235604860010565
Accuracy Test :  0.8176216882316697

AUC         : 0.8610437761637267
F1-Score Train 0.5984984984984984
F1-Score Validation :  0.5843205574912892
```

## Conclusion

By improving this model, It will help in predicting Provider fraud, to help Insurance companies and Government to take decision against fraudulent health provider and also to improve health of economy.





