# E-Commerce Business Analysis

This was the third project I worked on in the **TripleTen Business Intelligence Analytics Program**. It was an independent project designed to showcase what I have learned in **Business Analytics**. The purpose was to analyze the company's raw transaction logs and turn the event logs into business metrics.

## Description

- 9-page spreadsheet
- Includes raw data , processed data, data analysis, and pivot tables.

## Process

1. **Exploration & Cleaning**: Explored, filtered, and cleaned the raw data to ensure data quality.
2. **Conversion Funnel**: Created and built a conversion funnel to understand user behavior.
3. **Cohort Analysis**: Prepared data for cohort analysis to calculate retention rates.
4. **Retention Analysis**: Analyzed retention rates for cohorts based on acquisition dates.
5. **Formatting & Documentation**: Finalized the formatting and documentation for client readability.

## Data

The data was one Google spreadsheet file provided by TripleTen. Raw data can be found [here](https://docs.google.com/spreadsheets/d/1kRss89jqYqRXL8d7n5U06Xsj3z6QUwYKrlWFm-f7vRM/edit?gid=0#gid=0).


- **Business Analyst Project.csv**: Raw transaction logs
- **raw_user_activity**: Each row represents an activity, or event, by a user on the company’s website
- **user_id**: Unique customer IDs
- **event_type**: The type of activity by the user
- **category_code**: Category of the product being viewed or purchased
- **brand**: The company that makes the product
- **price**: Price of the product, in USD
- **event_date**: Date of the user activity, in YYYY-MM-DD format
- **Table of Contents**: Preformatted yet empty table of contents sheet
- **Executive Summary**: Preformatted yet empty executive summary sheet

## Assumptions

- The **raw_user_activity** sheet accurately reflects all website activity for the relevant timeframe.
- Missing values or inconsistencies in the data are minimal and can be ignored.
- The provided data format (columns, data types) is correct and consistent.

## Executive Summary

This analysis focuses on understanding **user behavior** and **retention patterns** on an e-commerce website, with the goal of improving **customer engagement** and **conversion rates**.

## Results

### Conversion Funnel

- **Conversion rates at each stage**:
    - From product view to shopping cart: **29%**
    - From shopping cart to purchase: **36%**
    - Total conversion from viewing product to purchasing: **10%**
 
    - <img width="669" alt="E-commerce" src="https://github.com/user-attachments/assets/aa984744-4e7b-46b2-b3c5-54a5ccb6e0e4" />


### Retention Rates

- Cohorts were categorized by their **acquisition date** and a month-by-month retention analysis indicated a downward trend in each group. Additional exploration into factors such as **periodic trends** or **cyclical patterns** could help uncover the reasons behind this decline.

## Analysis

### Raw Data

The raw data consists of user activity logs that capture interactions such as product views, cart additions, and purchases, including relevant details like **user IDs**, **price**, **product categories**, and **event dates**. The data was provided by the e-commerce company.

### Conversion Funnel

The conversion funnel is built by counting unique users at each stage of interaction (**view → shopping_cart → purchase**) and calculating conversion rates to assess user flow and website effectiveness.

### Retention Rates

Retention rates are calculated by grouping users into **cohorts** based on their first purchase month and tracking their continued purchases across the first four months.


