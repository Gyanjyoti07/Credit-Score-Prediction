 Credit-Score-Prediction
Project Overview
This project involves predicting the credit score of clients based on a dataset containing various details related to their banking transactions in the USA. The primary objective is to build a model that accurately predicts the credit score based on different attributes of the clients' financial behavior and transaction history.

Dataset
The dataset used in this analysis contains the following columns:

id: Unique identifier for each record.
customer_id: Unique identifier for each customer.
month: The month when the transaction was recorded.
name: Name of the customer.
age: Age of the customer.
ssn: Social Security Number of the customer.
occupation: Occupation of the customer.
annual_income: Annual income of the customer.
monthly_inhand_salary: Monthly in-hand salary of the customer.
num_bank_accounts: Number of bank accounts the customer has.
num_credit_card: Number of credit cards the customer has.
interest_rate:Interest rate applicable to the customer.
num_of_loan: Number of loans the customer has taken.
type_of_loan: Type of loan the customer has taken.
delay_from_due_date: Delay in payment from the due date.
num_of_delayed_payment: Number of delayed payments.
changed_credit_limit: Change in the credit limit.
num_credit_inquiries: Number of credit inquiries.
credit_mix: Mix of different types of credit accounts.
outstanding_debt: Total outstanding debt.
credit_utilization_ratio: Credit utilization ratio.
credit_history_age:Age of the credit history.
payment_of_min_amount:Whether the minimum amount was paid (binary: "yes", "no").
total_emi_per_month:Total EMI (Equated Monthly Installment) per month.
amount_invested_monthly:Amount invested monthly.
payment_behaviour:Payment behavior of the customer.
monthly_balance:Monthly balance of the customer.
credit_score:Credit score of the customer.
Analysis Steps
Data Preparation:

Imported necessary libraries.
Loaded the dataset.
Checked for null values and duplicates.
Removed duplicates.
Preprocessed numerical and categorical columns.
Exploratory Data Analysis (EDA):

Target Variable Distribution: Visualized using a count plot.
Distribution of Numerical Features: Visualized using histograms.
Correlation Matrix of Numerical Features: Visualized using a heatmap.
Distribution of Categorical Features: Visualized using count plots.
Data Preprocessing:

Standardized numerical features using StandardScaler.
One-hot encoded categorical features using OneHotEncoder.
Model Building:

Split the dataset into training and testing sets.
Trained a 'DecisionTreeClassifier' on the training set.
Trained a 'RandomForestClassifier' on the training set.
Model Evaluation:

Predicted the test set results using both classifier.
Evaluated the classifiers using a confusion matrix, classification report, and accuracy score.
Performed cross-validation and plotted the cross-validation scores.
Key Insights
Target Variable Distribution: The dataset is imbalanced with more "no" responses than "yes".
Numerical Features: Distributions of age, duration, and campaign show significant variability.
Correlations: Some features like annual_income and monthly_inhand_salary show strong correlations.
Categorical Features: Distribution of occupations, payment behavior, and type of loans provide insights into the client demographics.
Conclusion
The decision tree and random forest classifiers provide baseline models for predicting credit scores. Further improvements can be made by exploring other machine learning algorithms, feature engineering, and hyperparameter tuning. The EDA has revealed important patterns and insights that could help in better understanding and managing customer credit scores.
