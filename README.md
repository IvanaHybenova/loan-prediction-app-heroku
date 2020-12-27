# loan-prediction-app-heroku
An API for a classification model to predict loan status deployed on Heroku. 
https://loan-prediction-app-heroku.herokuapp.com/

## Content
A loan application is used by borrowers to apply for a loan. 
Through the loan application, borrowers reveal key details about their finances to the lender. 
The loan application is crucial to determining whether the lender will grant the request for funds or credit.

## Problem Statement
The director of SZE bank identified that going through the loan applications to filter the people who can be granted loans   
or need to be rejected is a tedious and time-consuming process. He wants to automate it and increase his bank’s efficiency. 

## Objective  
The idea behind this ML project is to build an ML model and web application that the bank can use to classify if a user can be granted a loan or not.

## Data
The dataset contains information about Loan Applicants. There are 12 independent columns and 1 dependent column. 
This dataset includes attributes like Loan ID, gender, if the loan applicant is married or not, the level of education, applicant’s income etc. 

Data Description  
Loan_ID: A unique ID assigned to every loan applicant 
Gender: Gender of the applicant (Male, Female)  
Married: The marital status of the applicant (Yes, No)  
Dependents: No. of people dependent on the applicant (0,1,2,3+)  
Education: Education level of the applicant (Graduated, Not Graduated)  
Self_Employed: If the applicant is self-employed or not (Yes, No)  
ApplicantIncome: The amount of income the applicant earns  
CoapplicantIncome: The amount of income the co-applicant earns  
LoanAmount: The amount of loan the applicant has requested for  
Loan_Amount_Term: The  no. of days over which the loan will be paid  
Credit_History: A record of a borrower's responsible repayment of debts (1- has all debts paid, 0- not paid)  
Property_Area : The type of location where the applicant’s property lies (Rural, Semiurban, Urban)  
Loan_Status: Loan granted or not (Y, N)  

## Built Model

Random Forest classifier with parameters:
max_depth=3, 
max_features=9,  
min_samples_leaf=5,  
n_estimators=80,  
random_state=0

Is deployed as flask API on Heroku, accesible on this [link](https://loan-prediction-app-heroku.herokuapp.com/).
