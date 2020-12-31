# WriteADataScienceBlogPost

Author: Angelina Espinoza-Limon

LINK TO THE POST IN MEDIUM.COM: https://angelina-espinoza-limon.medium.com/can-you-guess-that-mostly-fraud-occur-in-large-amounts-of-money-not-precisely-1b748b777a6b

Project Motivation:

This project communicates the insights about the data analysis for the identification of fraud based on synthetic financial data. 

The dataset to be used in the analysis has been created with an agent-based simulator based on "a sample of real transactions extracted from the logs of a mobile money service implemented in an African country" [1] (reference of this data is found at the end of this readme file).

This project follows the CRISP-DM process for the financial data analysis in order to identify what is the behaviour of the variables, which affect the identification of suspicious transactions from raw data. Several business questions are defined to guide the analysis that will be answered through this analysis. Thereafter, it is firstly analysed the data to find out which variables are mostly affecting the fraud detection, and then to model a suitable machine learning algorithm. This analysis include to perform a bias-variance trade-off to evaluate the model precision, through the AUPRC error score curve. 


Files in this repository:

1) PS_20174392719_1491204439457_log-full.csv

This file contains part of the dataset that is used in the Jupyter notebook code. The complete dataset is more than 100 Mb, and this can be obtained from the next link: 

Link to data: https://www.kaggle.com/ntnu-testimon/paysim1

2) FraudulentTransactionsDetection-v1.ipynb

This file contains the Jupyter Notebook code with the analysis about the identification of fraud based on synthetic financial data. 


The Jupyter notebook follows the following CRISP-DM steps:

CRISP-DM for Identifying Fraudulent Transactions

1. Business Understanding
2. Data Understanding
2.1 Data Gathering
2.2 Data Cleaning
2.3 Managing Missing Values
2.4 Analysing the Data
3. Data Preparation
3.1 Data Removal
3.2 Data Imputation
3.3 Feature Engineering
4. Modeling
4.1 Model Selection
4.2 Model Training and Testing
4.3 Model Visualization
5. Evaluation
5.1 Bias-variance tradeoff
6. Deployment
7. Conclusion

Some results from the analysis:

1. The fraudulent transactions inherently produces skew data, due to the proportion of non-fraudulent transactions is much bigger. This imbalance in the collected data makes challenging to establish machine learning models, so it must be implemented methods to tackle this, such as the AUPRC error curve to score the error in predictions, or using decision trees to manage the imbalanced data.

2. The transacted money in large amounts is not the main concern in money laundering, but the short-amount ones. The proportion found of this transaction types is much bigger.

3. Fraudulent transactions can occurred in either types, cash out or transfer, which means that fraudsters are using not only payment methods, but also transactions through financial institutions. The analysis identifies this result.

4. It is possible to identify a pattern which can be an indicator of fraudulent transactions. See the code analysis.

5. It is possible to provide a method to predict if a transaction is suspicious, by the means of training ML algorithms, which allows to adjust the parameters to get precise results.

References: 
[1] E. A. Lopez-Rojas , A. Elmir, and S. Axelsson. "PaySim: A financial mobile money simulator for fraud detection". In: The 28th European Modeling and Simulation Symposium-EMSS, Larnaca, Cyprus. 2016.
Link to data: https://www.kaggle.com/ntnu-testimon/paysim1

Acknowledgements: Jesin Fahad in Kaggle (https://www.kaggle.com/jesyfax/predicting-fraud-in-financial-payment-services)for her excellent data and ML analysis, from which I've learnt a lot.
