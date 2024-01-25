# Credit-Scoring-Analytics

## 📝 Overview
Banks and financial institutions employ diverse business strategies. Typically, public banks aim to minimize business risk by exclusively considering loan applicants with high credit scores for lending. On the other hand, private banks seek to maximize profits, necessitating the identification of optimal credit score tolerances. This optimization process is a key focus of analytics within the industry. New entrants, in contrast, often adopt a more inclusive approach, considering applicants regardless of whether they have a low credit score or no credit history at all. 

This analysis not only aids in making informed decisions regarding loan applications but also offers insights into the delicate balance between profitability and market expansion in the dynamic landscape of financial operations.
##  👨‍💻 Analysis 
### 1. Problem Statement
The objective is to construct an in-house risk model for subprime mortgages (a type of loan granted to low credit scores applicant ), optimizing profit for a bank. The profit structure involves a gain of $100 from a good customer and a loss of $500 from a bad customer. The dataset overview can be found here: [Credit Scoring Dataset](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/1.%20Credit%20Scoring.csv):
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
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/4.png) 

Logistic regression is selected for final modelling methods to predict the likelihood of loan repayment as it has the higest classification accuracy (84.93%)

![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/5.png)

Actual outcome, predicted target, probability of good loans and bad loans are are incorporated into a fresh dataset and then exported to a CSV file.
### 5. Decision Making
Decile methodology is employed for evaluating and determining the approval or rejection of new loan applications, with a focus on optimizing profitability or achieving broader market penetration. The process involves partitioning 750 observations into 10 equal segments after arranging them in descending order based on the probability of good loans.

Within each segment,  the count of bad and good loans, the minimum probability of good loans, cumulative number for good and bad loans are computed using a Pivot Table. Given that a bad loan incurs a loss of $500 and a good loan contributes a profit of $100, the profitability for each segment is derived.

Notably, the analysis reveals that the profit attains its zenith when the minimum probability of good loans reaches 87.31%. Therefore, to maximize profit, it is imperative for banks to set the threshold for the probability of good loans higher than 87.31%. Conversely, if the strategic goal is to expand market presence, the probability of good loans should be maintained at a level higher than 83.75%. 
![](https://github.com/Rui-Huang-dotcom/Credit-Scoring-Analytics/blob/main/image/6.png)




