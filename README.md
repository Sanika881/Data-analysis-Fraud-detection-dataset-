<h2>Fraud Detection Using Data Analysis</h2>
Project Overview:
This project is all about spotting fraudulent transactions through data analysis techniques. I analysed the dataset filled with financial transactions, which includes user details, transaction amounts, and payment methods, to uncover patterns that might signal fraud. The aim is to preprocess the data, tackle any missing values, conduct exploratory data analysis (EDA), and extract insights that can aid in identifying fraudulent transactions.

<br>Dataset used:https://www.kaggle.com/datasets/ranjitmandal/fraud-detection-dataset-csv

<br>Dataset Description
The dataset features 51,000 transactions with 12 key attributes, including:

- Transaction_ID – A unique identifier for each transaction
- User_ID – A unique identifier for each user
- Transaction_Amount – The amount involved in the transaction
- Transaction_Type – The type of transaction (like ATM Withdrawal, POS Payment, Bill Payment, etc.)
- Time_of_Transaction – The exact time when the transaction took place
- Device_Used – The device used to make the transaction (Mobile, Desktop, Tablet)
- Location – The geographical location of the transaction
- Previous_Fraudulent_Transactions – The number of fraudulent transactions previously associated with the user
- Account_Age – How long the user’s account has been active
- Number_of_Transactions_Last_24H – The count of transactions made in the last 24 hours
- Payment_Method – The method used for the transaction (Debit Card, Credit Card, UPI, etc.)
- Fraudulent – A binary flag indicating whether the transaction is legitimate (0) or fraudulent (1)

<br>Handling Missing Values
We encountered several columns with missing values:
<br>For Transaction_Amount, we filled in the gaps by using the mean value of the column.

For Payment_Method, Location, Time_of_Transaction, and Device_Used, we opted to fill in the missing values with the most common entry, known as the mode.

To visualize the patterns in the missing data, we created a heatmap using Seaborn.

<br>Exploratory Data Analysis (EDA)
Descriptive Statistics
We generated a summary of the dataset with the .describe() function, which provided insights into:

The average and standard deviation of transaction amounts

The distribution of account ages and instances of fraudulent transactions

The fluctuations in transaction numbers over time

<br>Data Visualization
We created several plots to help us understand the data better:

A Heatmap of Missing Data – This illustrated the extent of the missing values.

Histograms & Boxplots – These showed how transaction amounts were distributed.

Scatter Plots & Violin Plots – These highlighted the relationship between different transaction types and fraudulent activities.

Bar Charts – These depicted the frequency of various payment methods.


<br>Conclusion
This project effectively delves into detecting fraudulent transactions through data analysis techniques. By addressing missing values and conducting exploratory data analysis, we identified key indicators of fraud, which can be instrumental in developing machine learning models for fraud detection.
