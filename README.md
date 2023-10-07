![banner](Assets/Banner.jpg)

# Coffee-Bean-Sales-Data-Analysis-On-Excel
_**Unlocking Coffee's Hidden Potential - A Journey Through Data**_
- The Coffee Bean Sales Dataset offers a multifaceted exploration of the thriving coffee industry, providing a comprehensive view of sales, customer profiles, and coffee product details. This rich dataset is a gateway to understanding consumer behavior, optimizing product offerings, and improving business strategies in the world of coffee.

## Author
- [@saadharoon27](https://github.com/saadharoon27)

## Table of Contents
- [Business Problem](#business-problem)
- [Data Source](#data-source)
- [Business Problem](#business-problem)
- [Objective, Solution, and Outcome](#objective-solution-and-outcome)
- [Method](#method)
- [Quick Glance At The Dashboard](#quick-glance-at-the-dashboard)
- [Data Overview](#data-overview)
- [Step By Step Procedure](#step-by-step-procedure)
- 
- [Business Insights](#business-insights)
- [Business Suggestion](#business-suggestion)

## Business Problem
**Business Problem Statement:** <br>
The primary objectives include identifying top customers, tracking coffee-type sales trends, and analyzing sales by country. The dashboard should enable customer engagement and loyalty strategies, optimize product offerings, and support geographical expansion efforts.

## Objective, Solution, and Outcome
**Overall Objectives:** <br>
- Identify **top 5** customers
- Track coffee-type sales trends for better inventory management.
- Analyze sales by country to aid expansion.

**Solution Requirements:** <br>
- User-friendly and visually appealing dashboard.
- Interactive visualizations for trend identification.

**Expected Outcomes:** <br>
The Coffee Sales Dashboard will give actionable insights to boost sales, improve customer satisfaction, and drive strategic expansion efforts.

## Data Source
- [Coffee Beans Sales Dataset](https://www.kaggle.com/datasets/saadharoon27/coffee-bean-sales-raw-dataset)

## Method
- Exploratory data analysis _(EDA)_

## Quick Glance At The Dashboard
![dashboard](Assets/Glance.png)

## Data Overview
Data on coffee bean sales are divided into 3 separate sheets:
| Sheet Name     	            | Column Names    	|
|-------------------	        |------------------	|
| Orders     	                | Order ID (Primary Key), 
Order Date, Customer ID, Product ID, Quantity Ordered                                              |
| Customers    	              | Customer ID (Primary Key), Customer Name, Email, Phone Number, Address Line 1, City, Country, Postcode, Loyalty Card|
| Products               	    | Product ID (Primary Key), Coffee Type, Roast Type, Size, Unit Price, Price Per 100g, Profit 	                             |

## Steps By Step Procedure

- **Data Cleaning**
  - **Gender column:** Replaced the categorical value _‘M’_ and _‘W’_ values to _‘Men’_ and _‘Women’_.
  - **Quantity column:** Replaced the values _‘One’_ and _‘Two’_ to _‘1’_ and _‘2’_ respectively.

- **Data Processing**
  - **Age Group:** To address the *question vi* Of business question, a new column has to be created named **‘Age Group’** to extract the relationship between _‘Age’_, _‘Gender’_, and the _number of orders_ they made. 
  - **Categories:** >=50, Senior; >=30 and <50, Adult; <30, Young
  - **Month Column:** To address *question ii*, a **‘Month’** column has been created.

- **Analysis & Dashboarding**
  - **Step 1:**
    - To address _questions i_ and _ii_, created a new pivot table in sheet **‘Q1 - Order vs Sales Chart’** comparing total monthly sales value and the number of orders.
  - **Step 2:**
    - Created a new sheet, **‘Q3 – Most Purchases’** to analyse which gender purchased the most, addressing _question iii_.
  - **Step 3:**
    - Created a new sheet, **‘Q4 – Order Status’** to address _question iv_, which checks the status of the order compared to the total orders.
  - **Step 4:**
    - To address _question v_, a new pivot table has been made in the sheet named: **‘Q5 – Top 5 States’**.
  - **Step 5:**
    - To understand the relationship between _age, gender,_ and _number of orders,_ and to address _question vi_ a new sheet has been created named: **‘Q6 – Age, Gender, Orders’**.
  - **Step 6:**
    - Addressing _question vii_: To check which channel has the highest contribution a pivot chart has been created in sheet: **‘Q7 – Channels’**.

- **Filters**
  - To create an interactive visual dashboard, **3 slicers** were made on: *Month, Channel,* and *Category.*
