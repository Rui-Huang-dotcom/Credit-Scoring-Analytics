# Credit-Scoring-Analytics

## 📝 Overview

##  👨‍💻 Analysis 
### 1. Problem Statement
The objective is to construct an in-house risk model for subprime mortgages, optimizing profit for a bank. The profit structure involves a gain of $100 from a good customer and a loss of $500 from a bad customer. The dataset overview can be found here: [Credit Scoring Dataset](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/1.%20Credit%20Scoring.csv):
![Credit Scoring Dataset](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/0.png)  
The dataset comprises 3000 records across 30 columns, with the 'Target' variable representing good loans (0) and bad loans (1).
### 2. ETL
Alteryx handles the Extract, Transform, Load (ETL) process, depicted below:
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/1.png)  
The resultant dataset serves as the foundation for subsequent analyses.
### 3. Data Visualisation
Power BI is employed, illustrating 2500 good loans and 500 bad loans.
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/2.png)  
### 4. Data Modelling
Utilizing Logistic Regression, KNN, Decision Tree, SVM, and Random Forest for modeling:
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/3.png) 
Logistic regression is selected for final modelling methods as it has the higest classification accuracy (82.4%)
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/Screenshot%202023-12-21%20at%2015.38.10.png)
### 5. Decision Making
Final decision-making employs the Decile method.
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/4.png) 




