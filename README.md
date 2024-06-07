# Super-Store-Sales-Performance-Dashboard

## Tbale Of Content

- [Project Overview](#Project-Overview)
- [Data Source](#Data-Source)
- [Tools](#Tools)
- [Data Cleaning / Data Preparation](#Data-cleaning--Data-preparation)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
  
### Project Overview

The Sales Analysis Dashboard aims to provide comprehensive insights into various aspects of sales performance,
including trends over time, product distribution, regional sales, order processing times, and customer segment analysis.
This dashboard utilizes Pivot Tables and various chart types to visualize and analyze sales data effectively.

### Data Source

Superstore Sales Dataset: The primary dataset used for this analysis is 'Superstore Sales Dashboard.xlsx' file, Containing details about the customers' purchases.

### Tools

- Excel (Data Cleaning, Data Analysis, Data Visualization)
  - [Dowload_here](https://microsoft.com/)

# Data cleaning / Data preparation

In the initial data preparation, these are the performed tasks:
1. Data loading and inspecting.
2. Data cleaning and formatting.
3. Adding helping columns for deeper analysis.

### Exploratory Data Analysis

EDA involved exploring the sales data to uncover patterns and metrics, such as:
 
- Sales Trends Over Time  
- Sales by Region
- Customer Segment Analysis

### Results & Findings

**Key Insights from Sales Analysis Dashboard**

1. Dominance of Standard Class in Shipping:
The Standard Class emerges as the most utilized shipping mode, surpassing all other classes in popularity and usage.

2. Regional Sales Leaders - East and West:
The Eastern and Western regions stand out as the top performers in sales generation, significantly leading over other regions.

3. Surge in Sales in the Second Half of the Year:
There is a notable increase in sales during the second half of the year, with a significant boost starting from the beginning of August, highlighting a strong upward trend.

### Recommandations

Based on the analysis, we recommand the following actions:
- Invest in marketing advertising during peak sales season to maximize revenue.
- Focusing on expanding and promoting products in the least performing sub-categories.
- Implementing a customer segmentation strategy to effectively target high lifetime value (LTV) customers.
  
### Limitations 

One limitation of the dataset was the need to add a helper column for categorizing shipping time speeds.
This was necessary to make the data more interpretable, as the original column consisted solely of raw numerical values Without this additional categorization,
it would have been challenging to analyze and visualize shipping speeds effectively.
I've written this formula to perform this:
``` Exdel Formula
=IFS([@[Delivery Speed]]<=2,"Express Delivery",[@[Delivery Speed]]<=5,"Standard Delivery",[@[Delivery Speed]]<=7,"Delayed Delivery", TRUE,"Overdue Delivery")
```







