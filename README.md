# Loan-Tap-case-study

-- Project Overview

This project is based on a business case study from Scaler Academy, focusing on credit risk assessment for LoanTap, an online loan provider. The task is to build a Logistic Regression model to determine whether a personal loan applicant is likely to fully repay or default.
The goal is to support LoanTap’s underwriting process by improving creditworthiness evaluation and reducing Non-Performing Assets (NPAs) while ensuring eligible borrowers are not denied access to credit.

-- Business Context

LoanTap provides flexible personal loans tailored to millennials, salaried individuals, and professionals. The underwriting challenge lies in:
1. Detecting real defaulters with high accuracy.
2. Minimizing false positives (avoiding rejection of good borrowers).
3. Reducing loan defaults and NPAs to maintain profitability.

-- Problem Statement

Given a dataset of borrower attributes, determine if a loan should be extended to an individual. If so, suggest repayment terms in line with business recommendations.

--Columns in Dataset

1. loan_amnt : The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the       loan amount, then it will be reflected in this value.
2. term : The number of payments on the loan. Values are in months and can be either 36 or 60.
3. int_rate : Interest Rate on the loan
4. installment : The monthly payment owed by the borrower if the loan originates.
5. grade : LoanTap assigned loan grade
6. sub_grade : LoanTap assigned loan subgrade
7. emp_title :The job title supplied by the Borrower when applying for the loan.*
8. emp_length : Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years.
9. home_ownership : The home ownership status provided by the borrower during registration or obtained from the credit report.
10. annual_inc : The self-reported annual income provided by the borrower during registration.
11. verification_status : Indicates if income was verified by LoanTap, not verified, or if the income source was verified
12. issue_d : The month which the loan was funded
l3. oan_status : Current status of the loan - Target Variable
14. purpose : A category provided by the borrower for the loan request.
15. title : The loan title provided by the borrower
16. dti : A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the            requested LoanTap loan, divided by the borrower’s self-reported monthly income.
17. earliest_cr_line :The month the borrower's earliest reported credit line was opened
18. open_acc : The number of open credit lines in the borrower's credit file.
19. pub_rec : Number of derogatory public records
20. revol_bal : Total credit revolving balance
21. revol_util : Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
22. total_acc : The total number of credit lines currently in the borrower's credit file
23. initial_list_status : The initial listing status of the loan. Possible values are – W, F
24. application_type : Indicates whether the loan is an individual application or a joint application with two co-borrowers
25. mort_acc : Number of mortgage accounts.
26. pub_rec_bankruptcies : Number of public record bankruptcies
27. Address: Address of the individual

1. Exploratory Data Analysis (EDA)
    1. Distribution of loan amounts, terms, interest rates, and installments.
    2. Univariate analysis for continuous variables.
    3. Count plots for categorical variables.
    4. Bivariate analysis for correlations and relationships.
    5. Key insights documented.

2. Data Preprocessing
    1. Duplicate value checks.
    2. Handling missing values.
    3. Outlier treatment.
    4. Feature engineering (e.g., flag creation for attributes like mort_acc, pub_rec).
    5. Data preparation and scaling.

3. Model Building
     1. Logistic Regression model developed using Scikit-learn / Statsmodels.
     2. Model coefficients displayed with feature names.

4. Model Evaluation
     1. ROC-AUC Curve with business interpretation.
     2. Precision-Recall Curve to evaluate false positive vs false negative tradeoff.
     3. Classification Report (Accuracy, Precision, Recall, F1-score).
     4. Confusion Matrix visualization.

5. Insights & Recommendations
     1. Actionable insights based on model outputs and borrower attributes.
     2. Recommendations for LoanTap to optimize risk vs reward.
  
-- Tech Stack
      1. Python: pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels
      2. Colab Notebook for analysis
   
