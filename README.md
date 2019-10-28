# CreditCardFraudDetection

## Introduction

Credit Card Fraud Detection is one of the major applications of Machine Learning in the modern world. Amongst the millions of credit card transactions taking place all over the world every day, it is not possible to determine manually which ones are valid and which ones are not. Thus, we try to train our Machine Learning model with sufficient data and apply certain algorithms to help make predictions regarding the validity of transactions. In other words, we are trying to detect anomalies, or transactions that are unusual, and labelling them as "Invalid" or "Fraud".

## Algorithms Used

Although in the real world, due to improved efficiency and higher complexity Neural Networks are the preferred choice, in this project I have taken a different approach. Rather, two different approaches. The algorithms used in this project are Isolation Forest and Local Outlier Factor for anomaly detection. Both these have been implemented separately and their efficiencies have been compared at the end. More information on these algorithms can be found on the scikit learn website.

Isolation Forest :  (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.IsolationForest.html)
Local Outlier Factor : (https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.LocalOutlierFactor.html) 

## Requirements

    Python : 3.7.3 (default, Mar 27 2019, 22:11:17)
    [GCC 7.3.0]
    Numpy : 1.16.2
    Matplotlib : 3.0.3
    Seaborn : 0.9.0
    Scipy : 1.2.1
    Sklearn : 0.20.3
    
  

These can be checked easily by importing the required libraries, and checking their versions in a similar way as shown in Cell 1. 

## Dataset

The dataset used is the Credit Card Fraud Detection dataset available on Kaggle. You can also download it from the creditcard.csv file uploaded along with the code. 




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3Njg4MTgwMTgsODQxNzY2MTcyXX0=
-->