<img width="2400" height="1080" alt="Ekran görüntüsü 2025-11-14 003727" src="https://github.com/user-attachments/assets/e46517bc-2f21-4209-8ff8-a0d881ca69eb" />

# Retail Sales Insights | SQL (With RFM Analysis)
# Overview
This project demonstrates end-to-end SQL data analysis on a fictional retail store dataset.  
I have covered every stage of the data analytics lifecycle — from data validation and cleaning to exploratory analysis and advanced customer segmentation (RFM).

# Objective
The goal is to uncover actionable business insights to find the optimal marketing campaign launch conditions by asking :
- Who are the most valuable and frequent customers?  
- Which products and categories drive the most revenue?  
- When is the best time to launch marketing campaign?
- What is the best way to launch marketing campaign?  
- How can RFM segmentation help identify customer loyalty and retention opportunities?

# Data Set
The dataset was originally sourced from Kaggle; however, I modified it to better suit the specific needs of my project.
Please refer to repository for the altered data set.It contains;

* Transaction_ID:A unique identifier assigned to each transaction. 
* Customer_ID:A unique identifier for each customer
* Category:The general classification of the purchased item 
* Item_ID:A unique code assigned to each product or item. 
* Price_Per_Unit:The cost of one unit of the item purchased. 
* Quantity:The number of units purchased in the transaction.
* Total_Spent:The total monetary value of the transaction for that item.
* Payment_Method:The method used by the customer to complete the purchase 
* Location:The store, city, or region where the transaction took place. 
* Transaction_Date:The date when the transaction occurred.
* Discount_Applied:Indicates whether a discount was used in the transaction 

# Tools & Techniques
* MySQL 
* Window Functions (ROW_NUMBER, COUNT, SUM)**
* CTEs for segmentation**
* RFM Scoring System

# Project Overview

_At first glance, the data looked messy — inconsistent category names, missing values represented as \N, and even some potential duplicates. So before doing any complex analysis, I focused on one thing: getting the data right._

1. Data Validation:Ensured that all records have been implemented and data integrity is intact.
2. Data Staging:Created staging tables for safe data cleaning and transformation.
3. Data Cleaning & Missing Values:Handle missing values and standardize inconsistent entries.
4. Duplicate Handling:Removed that duplicate transactions while maintaining a clean dataset.
5. Final Data Standardization:Ensured that consistent and accurate categorical data.
6. Exploratory Data Analysis (EDA):Analysis to understand when,how,where,which product to launch to  marketing campaign on.
7. Advanced Analysis: RFM Segmentation
8. Summary of Insights will be shown below

# Results / Insights 

Let’s explore the types of insights we can present to our management team.

__Which Customers to Focus on;__

Based on the data (limited to the top 10 for clarity), we can see that the highest average order value belongs to the “Butchers” category, with Customer_5 leading in total spending. This customer also shows significant spending in the Beverages category. Similarly, Customer_13 demonstrates considerable spending in Electric Household Essentials and Food. Therefore, if the campaign were to target specific customers, focusing on these high-value individuals could maximize the overall return and campaign effectiveness.

<img width="673" height="209" alt="1" src="https://github.com/user-attachments/assets/c2867406-0533-4ee8-be27-6c48e06ebe59" />

__Which Products to Focus on;__
In this section, we examine which products are frequently purchased.
Butchers: Item_25_BUT and Item_22_BUT
Beverages: Item_25_EHE
These items are among the most frequently bought products. Therefore, our efforts should focus on these categories, as they represent high-demand goods.

<img width="400" height="200" alt="2" src="https://github.com/user-attachments/assets/27c196d9-1355-42e3-8b53-bc40fbf636a4" />

__When to Lauch the marketing campaign__

As could be expected, the end and the beginning of the year are the best periods due to higher sales volumes, which is typical in retail setting.

<img width="250" height="250" alt="3" src="https://github.com/user-attachments/assets/0a6de1fb-269a-4cee-84d0-25ed357a630f" />

__Which Location to Launch the Marketing Campaign__

There are only two business locations in the dataset, and the number of transactions is very similar for both. 
Based solely on these numbers, marketing efforts could be evenly split between the two locations.

<img width="250" height="250" alt="4" src="https://github.com/user-attachments/assets/5403399e-dab2-4dcb-905e-8140572f2ebb" />

__RFM Analysis__

RFM looks at below metrics;

* Recency:How recently a customer made a purchase or engaged with the business
* Frequency:How often a customer has made a purchase within a specific time period.
* Monetary Value:The total amount of money the customer has spent with the business over a specific period.

The RFM analysis places CUST_05 as the top-scoring customer, thanks to their strong Monetary and Frequency scores. CUST_01 follows closely in second place.
These customers demonstrate high engagement with the company and contribute significant revenue, making them our key accounts.
The other companies fall into a secondary tier, performing reasonably well but not at the level of CUST_05 and CUST_01.
While only the top 10 customers are displayed here, lower RFM scores in the overall dataset may indicate customers who are at risk of churn or potentially disengaging.

<img width="800" height="150" alt="Ekran görüntüsü 2026-05-04 233231" src="https://github.com/user-attachments/assets/4ece68da-2d8a-44f9-9265-bbfd16193206" />

# Links&References

Link for the SQL codes:
https://github.com/TheAnalystAlp/Retail-Sales-Insights-SQL-With-RFM-Analysis-/blob/main/Retail_Sales_Insights___SQL(With_RFM_Analysis).ipynb

Feel free to reach me at; Linkedin:www.linkedin.com/in/alp-tuna

My Website:https://alptheanalyst.wixsite.com/alptuna

My E-Mail:alptuna.professional@gmail.com

Link for the Colab file:[https://colab.research.google.com/drive/1oXrwRaj9hJYkiJVktSucdZ0gkGIsQ_VA ](https://colab.research.google.com/drive/1lP6t4pHuJGTe1LO0ynJ8ypPAcn7KwVjc?usp=sharing)

Link for the Data Set:https://github.com/TheAnalystAlp/Retail-Sales-Insights-SQL-With-RFM-Analysis-/blob/main/retail_store_sales.csv

