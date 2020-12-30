# WriteADataScienceBlogPost

Author: Angelina Espinoza-Limon

IMPORTANT NOTE: The complete dataset is more than 100 Mb, then I've just uploaded part of it, but the complete dataset can be obtained from: https://www.kaggle.com/ntnu-testimon/paysim1

LINK TO POST IN MEDIUM.COM: https://angelina-espinoza-limon.medium.com/can-you-guess-that-mostly-fraud-occur-in-large-amounts-of-money-not-precisely-1b748b777a6b

This project communicate the insights about the data analysis for Project 1 for the Data Science specialization in Udacity.

This project presents the CRISP-DM process for the financial data analysis in order to identifyering what is the behaviour of the variables, which affect the identification of suspicious transactions from raw data. Several business questions are defined to guide the analysis that will be answered through this analysis. Thereafter, it is firstly analysed the data to find out which variables are mostly affecting the fraud detection, and then to model a suitable machine learning algorithm. This analysis include to perform a bias-variance trade-off to evaluate the model precision, through the AUPRC error score curve. 

The dataset to be used in this analysis is a synthetic dataset [1] which has been created with an agent-based simulator based on "a sample of real transactions extracted from the logs of a mobile money service implemented in an African country" [1].

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


References: 
[1] E. A. Lopez-Rojas , A. Elmir, and S. Axelsson. "PaySim: A financial mobile money simulator for fraud detection". In: The 28th European Modeling and Simulation Symposium-EMSS, Larnaca, Cyprus. 2016.

Acknowledgements: Jesin Fahad in Kaggle (https://www.kaggle.com/jesyfax/predicting-fraud-in-financial-payment-services)for her excellent data and ML analysis, from which I've learnt a lot.
