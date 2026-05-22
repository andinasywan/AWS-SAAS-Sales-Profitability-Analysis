# SaaS Sales Profitability Analysis

## Project Overview

This project analyzes SaaS sales transaction data to evaluate company performance, profitability, discount impact, and loss-making areas. The analysis focuses on identifying which regions, segments, industries, and products contribute the most to sales and profit, as well as understanding how discount levels relate to profit margin and transaction losses.

The main business problem addressed in this project is that high sales do not always lead to high profit. Therefore, this analysis aims to help the company shift from sales-focused growth to profit-focused growth.

## Business Questions

1. Which regions, segments, industries, and products generate the highest sales and profit?
2. Does high sales always translate into high profit and healthy profit margin?
3. How does discount relate to profit and profit margin?
4. Which business areas should be prioritized, evaluated, or improved to increase profitability?

## Dataset

The dataset used in this project is **SaaS Sales**, containing B2B SaaS sales transaction records.

Key fields used in the analysis include:

- Order ID
- Order Date
- Customer ID
- Region
- Segment
- Industry
- Product
- Sales
- Quantity
- Discount
- Profit

Additional columns were created during analysis:

- Profit Margin
- Profit Margin Pct
- Discount Pct
- Profit Status
- Discount Category
- Loss Transaction
- Loss Amount

## Tools Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Looker Studio
- Canva

## Analysis Process

### 1. Data Understanding
The dataset was explored to understand the structure, columns, data types, and key numerical and categorical variables.

### 2. Data Cleaning
The cleaning process included:

- Checking missing values
- Checking duplicate data
- Standardizing categorical columns
- Converting date columns
- Creating new features for profitability and discount analysis
- Checking outliers in sales, profit, discount, and profit margin

### 3. Exploratory Data Analysis
EDA was conducted to analyze:

- Yearly sales and profit trend
- Monthly highest and lowest sales/profit
- Performance by region
- Performance by segment
- Performance by industry
- Performance by product
- Discount and profitability relationship
- Loss transactions by product and segment

### 4. Statistical Analysis
Statistical analysis was conducted to support the findings:

- Correlation analysis
- Shapiro-Wilk normality test
- Mann-Whitney U Test

The Mann-Whitney U Test was used because the profit data was not normally distributed.

## Key Findings

- Sales increased from **484K in 2020** to **734K in 2023**.
- Profit increased from **50K in 2020** to **94K in 2023**.
- Profit margin peaked in **2022 at 13.43%**, then slightly declined to **12.74% in 2023**.
- **EMEA** generated the highest total sales and profit.
- **AMER** had the highest profit margin.
- **APJ** had the lowest profit margin.
- **SMB** contributed the highest sales and profit, but also recorded the highest total loss.
- **Finance**, **Energy**, and **Manufacturing** were the most profitable industries.
- **Alchemy** generated the highest profit, while **ContactMatcher** generated the highest sales.
- **Marketing Suite** recorded negative profit.
- Medium to very high discount categories generated negative profit.
- Discount had a strong negative correlation with profit margin, with correlation value of **-0.86**.
- Mann-Whitney U Test showed **p-value < 0.001**, indicating a significant profit difference between Low/No Discount and High Discount transactions.

## Business Recommendations

1. **Control high discount usage**  
   Limit medium-to-very-high discount usage and monitor its impact on profit margin.

2. **Evaluate loss-making areas**  
   Review SMB and ContactMatcher transactions to identify pricing, discount, and customer patterns causing loss.

3. **Prioritize profitable markets**  
   Focus on EMEA for total profit contribution and maintain AMER because it has the strongest profit margin.

4. **Push high-profit products**  
   Prioritize products such as Alchemy, Site Analytics, and Data Smasher.

5. **Use profit margin as a key performance indicator**  
   Sales should not be the only performance metric. Profit margin should be used to evaluate business health.

6. **Build profitability monitoring dashboard**  
   Monitor sales, profit, profit margin, discount category, and loss transactions through an interactive dashboard.

## Dashboard

The dashboard was created using **Looker Studio** and consists of three main pages:

1. **Executive Overview**  
   Shows overall sales, profit, profit margin, discount, and regional performance.

2. **Market & Product Performance**  
   Shows segment, industry, and product performance.

3. **Discount & Loss Analysis**  
   Shows discount impact, total loss, loss by product, and loss by segment.

Dashboard link:  
https://datastudio.google.com/reporting/5ae502a1-0e42-47d0-a49f-e7bb9b0af4a1

## Presentation

Presentation slides summarize the business problem, key insights, statistical validation, and recommendations.

Slide link:  
https://canva.link/mx0u2h7671k665y


