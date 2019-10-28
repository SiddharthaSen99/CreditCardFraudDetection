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

The dataset used is the Credit Card Fraud Detection dataset available on Kaggle. You can also download it from the creditcard.csv file uploaded along with the code. The actual dataset consists of 284807 rows and 31 columns. Due to computational costs, only a small fraction(30%) of the dataset has been used.

## Results

This is what the plotted histograms look like :






This is what the correlation matrix looks like :









This is what the final result looks like :












As it is prominent from the results, both the algorithms achieve a high accuracy (99.6% and 99.7%). However, their f1- scores are very low for the invalid transactions. While it is 0.30 for isolation forest, it is an astonishingly low 0.03 for local outlier factor algorithm. This suggests two things:
1. Isolation Forest algorithm is relatively better than Local Outlier Factor algorithm for anomaly detection (in this case, fraud detection)
2. The reason we have been achieving such high accuracies despite having such low f1-scores is solely due to the fact that the number of valid transactions are much more than the number of invalid transactions. This is understandable as in the real world, we can expect more valid transactions than invalid transactions. When the number of invalid transaction become significantly high, both of thee algorithms will not be preferred anymore and the ideal solution in such a scenario would be to use Neural Networks.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYyOTY3NzYyM119
-->