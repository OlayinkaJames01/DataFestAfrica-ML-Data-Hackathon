# DataFestAfrica-ML-Data-Hackathon

## Problem Statement
Charles is a customer at the Borrowme FinTech lending Company and has been laying complaints on how his loan application process has overstayed for months. He is pleading with the company to fast-track the process so he can know his fate. 
It turns out that a long list of customers in the company are just like Charles and the CEO is concerned about this issue.

## Solution
The team at Borrowme has provided historical information containing the information of applicants and the status of their loan application process to us, the DataCatalysts team. We are expected to automate the process by building a machine learning model to predict if there was an outcome of being E-signed or not after the electronic credit facility process is completed.

## Solution Approach
To build a reliable model to solve this problem. The steps we followed are summarized below:
1. Business Understanding
2. Import Data
3. Exploratory Data Analysis
4. Feature Selection
5. Model Building
6. Model Evaluation

## Business Understanding

Overtime, traditional lending companies have been careful with granting loans to borrowers. Because they don't want to offer loans to unworthy people, they go through a time consuming process of evaluating the credit worthiness of would-be borrowers before approving or rejecting their loan application. 

This delay has several negative effects on the borrowers especially when the need for the money is urgent. Imagine if the life of a loved one is at stake or maybe a business contract is at the verge of getting terminated because of lack of funding or this borrower is in a debt that is depressing enough to make him take his life. 

Innovators have looked at this problem and birthed FinTech solutions to solve this. Companies can still carefully pick credit worthy individuals but this time, they will use technologies like Artificial Intelligence to gather the required data for evaluation. But then, even though it seems like it's a bit easier to gather data, this delay problem hasn't been entirely solved. Someone still needs to approve or reject this application as quickly as possible. This can only be done after this *someone* has studied this gathered data and confirmed if this borrower is credit worthy or not. 

The question is, should this still be done by humans when we already have technology? Why can't we just use technology to look through all these applications and immediately confirm if a borrower is credit worthy or not. This is why we, the DataCatalysts team have built a model to predict if an individual is credit worthy or not. 

Our model is predicting credit worthy individuals to get their online applications E-signed while the non-worthy individuals won't have their applications E-signed. 

## Data
Two datasets were given: The train and test datasets.

The train dataset has 12516 rows and 20 columns in the dataset.
The column names include:
Entry_id : User Identifier - client
age: Age of user
pay_schedule: How often applicants get paid
home_owner: 0:- Rented home 1:- Owner
income: Applicant income
months_employed: How many months has he been doing the job
years_employed: How many years he been doing job
current_address_year: How many years a person stayed at the current address
personal_account_m: How many months that person had a personal account
personal_account_y: How many years has that person had a personal account
has_debt: If the individual has debt
amount_requested: Loan amount requested
risk_score_n (1,2,3,4,5):- Various scores are defined by regulations and internal processes to classify individual risks
ext_quality_score_n (1 & 2): External quality scores defined for each individual
inquiries_last_month: Number of times an individual made inquiries in the previous month.

Target column in the test dataset:
e_signed: If the application was completed as an e-signing process or not 

### Exploratory Data analysis
Checking out how each column affects the target column (e_signed). 

### Model Building
Used various classification models like Logistic Regression, CatBoost, Xgboost, Random Forest and LightGB models to get the best prediction possible. A lot of hyperparameter tunnings were done in a bid to get the optimized parameter for the best performing models.
