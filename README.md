# Credit-Default-Prediction

The dataset you will be using is default of credit card clients Data Set.
There are two data files: "CreditDefault_training.csv" and "CreditDefault_Xtest.csv"
Both files have the following fields, except the label ("default.payment.next.month") which is not available in "CreditDefault_Xtest.csv" 

**Features:**

1 - LIMIT_BAL:  Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit. <br>
2 - SEX: (1 = male; 2 = female) <br>
3- EDUCATION: (six levels: 1,2,3,4,5,6) <br>
4 - MARRIAGE: (1 = married; 2 = single; 3 = others) <br>
5 - AGE <br>

From "PAY_1" to "PAY_6": History of past payment (Repayment status: -2: Balance paid in full and no transactions this period; -1: Balance paid in full, but account has a positive balance at end of period due to recent transactions for which payment has not yet come due; 0: Customer paid the minimum due amount, but not the entire balance; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.)
From "BILL_AMT1" to "BILL_AMT6": Amount of bill statement (NT dollar).<br>
From "PAY_AMT1" to "PAY_AMT6": Amount of previous payment (NT dollar).<br>

**Target:**

default.payment.next.month: binary variable, whether default payment (Yes = 1, No = 0)

Prediction task is to determine whether there's credit default for a person.

**Data Processing and Feature Engineering:**

1. Standardization and One-Hot encoding
2. Hyperparameter Tuning

**Model:**

Logistic Regression

