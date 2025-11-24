---

# About this Project IS-6812 | Group 5 
Thomas Beck | Whitney Bullock | Caleb Call 
This repository contains highlights from our practice capstone project.  Our project focused on leveraging machine learning models to solve the real-world business problem for Home Credit.  The proejct will showcase the complete workflow from understanding the business problem, to completing exploratory data analysis, building of four different predictive models, and evaluating results.  The project demonstrates business value to Home Credit, being able to analyze their incomplete data, draw insights, and produce business use cases to better predict if a customer will default on the loan.  

---
## Highlights 
- Business Problem

- Solution to Business Problem
  
- Personal Contribution

- Business Value of Solution

- Difficulties During Project

- Key Takeaways 


## Business Problem 
Home Credit’s operational model is fundamentally about financial inclusion. Loans are provided to populations with little or no credit history—groups often rejected by traditional banks. This creates a risk assessment challenge: evaluating repayment likelihood without standard credit scores.

The core issue is information asymmetry. Strict approval criteria exclude creditworthy applicants, failing the corporate mission. Lenient criteria result in financial losses from defaults.

The goal is not merely prediction accuracy, as only 8% of the population defaults. A basic model could achieve 92% accuracy simply by approving every applicant, but this fails to manage risk. Instead, applicants must be ranked by default likelihood using AUC-ROC. This approach identifies specific “invisible risk” cases for further review.

## Solution to Business Problem 
To address Home Credit's need for reliable and responsible lending decisions, our project will develop a machine learning model to use as a risk assessment to predict whether a customer is likely to default on a loan.  By anlayzing various variables provided in the loan-application process our models will quantify the customer's repayment capability when standard credit history is limited. 


## Business Value of Solution 
There are four objectives in our solution to add value to the business: 

- Maximize Customer Base

- Minimize Financial Risk

- Empower Financial Freedom

- Enhance Operation Efficiency 

By accurately predicting customer's likelihood of defaulting on a loan with limited credit history Home Credit can make more informed lending decisions.  This will enable Home Credit to responsibly extend credit to a broader range of customers while reducing their risk of default.  Our solution supports responsible lending for Home Credit and financial inclusion for it's customers, who generally are underserved.  A bi-product of the decision tree model is the ability generate automated approval / rejection processes based on specific loan application responses.  Overall, our predictive models empower Home Credit to balance financial inclusion with risk mitigation, strengthening Home Credit's customer reach and sustainability.  

## Difficulties During Project 
The main difficulty during the project was combatting class imbalance. Only about 8% of the target variable represented loan defaults, which caused the models to be biased toward predicting non-defaulters. To address this challenge the decision tree model weighted the minority class 5:1 during training, helping the model pay more attention to the defaulting class.  Additional, cross-valiation techniques were applied to improve model performance to ensure more robust and generalized predictions. These measures to handle class imbalance highlighted the importances of careful processing, evaluation, and tuning for predictive models.  

## Key Takeaways 
This practice project provided valuable experience for the team to work with real-world data.  It allowed the opporunity to gain key learnings from true data that is messy, missing values, imbalanced, and imperfect.  Working on real world data highlighted the need for data cleaning and the time spent upfront in the process to clean the data and understand the variables will pay dividends later on.  Spending time during EDA will help identify which features are important and which features just add noise.  By selecting the right features we are able to improve the models learning ability and more accurately predict defaulters. The final takeaway I have from the project is appreciating the iterative process of experimenting with different models and tuning parameters to determine the best-performing solution for the dataset to develop a good model.  

## Project Conclusion 
The analysis identified external credit scores as the most robust predictors of default risk. Higher scores strongly correlate with lower risk. Age and employment history provide secondary predictive value, while demographic factors like gender and income show negligible utility in isolation.

The Gradient Boosting model (XGBoost) demonstrated superior performance (AUC 0.742) compared to Logistic Regression, Decision Trees, and Random Forests. It is recommended that Home Credit utilize this model to prioritize the riskiest applicants (e.g., the top 10%) for manual review, thereby optimizing resource allocation and minimizing potential defaults.
