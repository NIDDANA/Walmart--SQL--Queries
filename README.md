# Walmart Sales Data Analysis - SQL Project

## Overview
This project focuses on analyzing Walmart's sales data to uncover insights into product performance, sales trends, customer behavior, and branch performance. By analyzing the data, we aim to improve sales strategies and enhance decision-making processes. The dataset used in this project is from the **Kaggle Walmart Sales Forecasting Competition**.

## Project Goals
The main goal of this project is to understand the factors influencing Walmart's sales across different branches. We will explore various aspects of the data, including product performance, customer purchasing trends, and sales strategies, to help optimize sales processes.

## Dataset Description
The data used in this project comes from three Walmart branches located in Mandalay, Yangon, and Naypyitaw. It contains 17 columns and 1000 rows of sales transactions. Here's a breakdown of the columns:

| **Column**            | **Description**                                      | **Data Type**        |
|-----------------------|------------------------------------------------------|----------------------|
| **invoice_id**         | Unique identifier for each sale                      | VARCHAR(30)          |
| **branch**             | The branch where the sale took place                 | VARCHAR(5)           |
| **city**               | The location of the branch                           | VARCHAR(30)          |
| **customer_type**      | Type of customer (e.g., Regular, New)                | VARCHAR(30)          |
| **gender**             | Gender of the customer                               | VARCHAR(10)          |
| **product_line**       | Product category sold                                | VARCHAR(100)         |
| **unit_price**         | Price per unit of product sold                       | DECIMAL(10, 2)       |
| **quantity**           | Quantity of products sold                            | INT                  |
| **VAT**                | Tax amount on the purchase                           | FLOAT(6, 4)          |
| **total**              | Total cost of the purchase                           | DECIMAL(12, 4)       |
| **date**               | Date when the purchase occurred                      | DATETIME             |
| **time**               | Time of the purchase                                 | TIME                 |
| **payment**            | Total amount paid for the purchase                   | DECIMAL(10, 2)       |
| **cogs**               | Cost of Goods Sold (COGS)                            | DECIMAL(10, 2)       |
| **gross_margin_pct**   | Gross margin percentage                              | FLOAT(11, 9)         |
| **gross_income**       | Gross income from the sale                           | DECIMAL(12, 4)       |
| **rating**             | Customer rating for the product                      | FLOAT(2, 1)          |

## Analysis Focus Areas
This project focuses on three main areas of analysis:

1. **Product Analysis**
   - Identify top-performing product lines.
   - Analyze sales trends and patterns.
   - Determine product lines that need improvement.

2. **Sales Analysis**
   - Evaluate sales performance over time.
   - Identify patterns in the data, such as best-selling products and months with the highest sales.

3. **Customer Analysis**
   - Explore customer segments.
   - Understand purchasing behavior and profitability for each segment.

## Approach

### 1. Data Wrangling
We begin by cleaning the data, ensuring no NULL or missing values. This includes:
   - Creating a database and inserting data into a table.
   - Ensuring all columns are properly populated, with no NULL values.

### 2. Feature Engineering
We generate new columns to provide more insights, such as:
   - **Time of Day**: Classify sales into Morning, Afternoon, and Evening.
   - **Day of the Week**: Extract the day of the week from the transaction date.
   - **Month of the Year**: Extract the month of the transaction.

### 3. Exploratory Data Analysis (EDA)
We explore the data to answer key business questions, such as:
   - How many distinct cities are in the dataset?
   - What is the most common payment method?
   - Which product line has the highest revenue?

## Key Business Questions

### Generic Questions
- How many distinct cities are there in the dataset?
- In which city is each branch located?

### Product Analysis
- How many distinct product lines are there?
- What is the most common payment method?
- What is the best-selling product line?
- What is the total revenue by month?
- Which month recorded the highest Cost of Goods Sold (COGS)?
- Which product line generated the most revenue?
- Which city has the highest revenue?
- Which product line had the highest VAT?
- Which product lines are performing "Good" or "Bad" based on sales?

### Sales Analysis
- How many sales were made at different times of the day (morning, afternoon, evening)?
- Which customer type generates the highest revenue?
- Which city has the largest VAT tax percentage?
- Which customer type pays the most VAT?

### Customer Analysis
- How many unique customer types exist in the data?
- How many unique payment methods are there?
- Which customer type is the most common?
- What is the gender distribution per branch?
- Which time of day do customers give the most ratings?
- Which day of the week has the best average ratings?

## Conclusion
This analysis will provide insights into Walmart's sales performance and help optimize sales strategies across different branches. By understanding customer behavior, sales trends, and product performance, Walmart can better align its business strategies and improve profitability.

## Tools & Technologies Used
- **SQL** for data management and querying
- **Python** for data wrangling and analysis (if applicable)
- **Jupyter Notebook** for analysis and visualization

This project helps uncover valuable insights from Walmart's sales data, providing a better understanding of product and customer performance, which can guide future business strategies.
