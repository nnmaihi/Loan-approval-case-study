# Loan-approval-case-study
### Case Study Context
Company A is a financial institution that provides personal loan products. At present, loan approvals are done manually, and the company wants to streamline this process by automating it. To achieve this, they are gathering data on loan approvals from the previous year. The aim is to extract valuable insights and establish rules from this dataset that can be used to automate the loan approval process

Business Questions
**Question 1:**
Visualize the following and give description.
- CIBIL Score distribution between approved and rejected loans
- Education distribution between approved and rejected loans
- Income distribution between approved and rejected loans

**Question 2:**
Visualize the relationship between income and loan amount for approved loans. Do you think the loan amount is directly proportional to the income level? Why or why not? 

**Question 3:**
If you were to include one more factor to predict loan outcomes, what specific factor would you choose to add, and what is the rationale behind this choice?

### Dataset Description
| Variable  | Description |
| ------------- | ------------- |
| loan id | Unique ID for each loan application |
| no of dependents | Number of dependents of the applicant |
| education | Applicant's education level |
| self employed | 	Whether the applicant is self-employed |
| income annum | Annual income of the applicant |
| loan amount | Amount of the loan requested |
| loan term | Term of the loan in months |
| cibil_score | Applicant's CIBIL score (credit score) |
| residential_asset_value |	Values of residential asset owned by the applicant |
| commercial_asset_value | Values of commercial asset owned by the applicant |
| luxury_asset_values | Values of luxury asset owned by the applicant |
| bank_asset_values | Values of bank asset owned by the applicant |
| loan_status |	Whether the loan was approved or rejected |

### Answer
**Question 1:** 
- CIBIL Score Distribution: Higher CIBIL scores improve approval chances.
- Education Distribution: ducation level does not significantly impact loan approval. 
- Income Distribution: There is no strong relationship between higher income and loan approval.

**Question 2:**
The relationship between income and loan amount for approved loans appears to be positively correlated, indicating that applicants with higher incomes are eligible for, or tend to request, larger loan amounts, yet it is not the only determinant of loan amount.

**Question 3:**
Create new features based on existing data to enhance the predictive power of the models:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM
- Suport Vector Classifier
Then assess the models to define the best model and deploy "Feature Importance" function to define the best features for each model.
Based on the performance of 5 best models, in addition to the "cibil_score" feature that brings the best efficiency in prediction, you can consider the new feature "loan_to_income_ratio"
