# Aim of the Project

The aim of this project is to analyze supermarket sales data to uncover patterns in customer behavior, product performance, and sales trends. Through exploratory data analysis and visualizations, the project intends to identify key insights that can help improve business decisions related to marketing, inventory management, and customer satisfaction.
# Objectives of the Project
    •	To understand overall sales performance across branches and cities.
	•	To analyze customer behavior based on gender, customer type, and purchase patterns.
	•	To compare product line performance and identify high-selling categories.
	•	To examine factors affecting total sales such as quantity, unit price, and time.
	•	To explore monthly, daily, and hourly sales trends for better business planning.
	•	To generate actionable insights that help improve marketing strategies and customer satisfaction.
# About the Dataset

The dataset used in this project is a Supermarket Sales dataset, which contains detailed transaction-level information collected from three supermarket branches. It includes customer details, product information, pricing, and sales-related attributes.

This dataset is ideal for performing Exploratory Data Analysis (EDA) because it helps us understand sales trends, purchasing behavior, and product performance across different branches and customer groups.

  ## Key Features in the Dataset
	•	Invoice ID – Unique ID for each transaction
	•	Branch – Branch where the purchase was made
	•	City – City of the branch
	•	Customer Type – Member / Normal customers
	•	Gender – Male / Female
	•	Product Line – Category of the product purchased
	•	Unit Price – Price of one unit
	•	Quantity – Number of units purchased
	•	Tax 5% – Tax applied
	•	Total – Final amount including tax
	•	Date & Time – Transaction details
	•	Payment Method – Cash, E-wallet, or Card
  # ➤ Workflow of the Project
The project follows a structured end-to-end data analysis workflow.
The major steps included are:

  ## 1.	Data Loading & Initial Overview
	•	Importing necessary libraries
	•	Loading the dataset
	•	Viewing rows, columns, and structure
 ## 2.	Data Cleaning & Pre-Processing
	•	Handling missing values
	•	Removing duplicates
	•	Correcting data types
	•	Cleaning inconsistent entries
	•	Formatting date and time columns
 ## 3.	Feature Engineering
	•	Creating new columns such as Day, Month, and Hour
	•	Generating additional insights like transaction day, weekend/weekday
 ## 4.	Exploratory Data Analysis (EDA)
	•	Visualizing sales trends
	•	Branch-wise performance
	•	Gender and customer type analysis
	•	Product line comparisons
	•	Monthly, weekly, and hourly sales patterns
 ## 5.	Insight Generation
	•	Summarizing key findings from all visuals
	•	Identifying business opportunities and improvement areas
 ## 6.	Report Preparation
	•	Organizing results
	•	Writing documentation
	•	Preparing project summary and conclusion

# Import Required Libraries

In this project, we use several Python libraries that help us load, clean, analyze, and visualize the supermarket sales dataset.
Each library plays an important role in completing different steps of the analysis.


## 1. Pandas

- Definition: A powerful library use
for data manipulation and analysis.

- Usage: Loading the dataset, cleaning data, exploring rows & columns, and creating new features.

### Syntax:
import pandas as pd

## 2. NumPy

- Definition: A numerical computing library that supports mathematical operations.
- Usage: Calculations, numerical corrections, and supporting data transformations.
### Syntax:
import numpy as np

## 3. Matplotlib

- Definition: A basic visualization library for creating charts and graphs.
- Usage: Bar charts, line graphs, scatter plots, and other basic visualizations.
### Syntax:
import matplotlib.pyplot as plt

## 4. Seaborn

- Definition: A statistical visualization library built on top of Matplotlib.
- Usage: Heatmaps, boxplots, countplots, and advanced visualizations with clean styling.
### Syntax:
import seaborn as sns

# Read Data

- To begin working with the supermarket dataset, we load the CSV file using the pd.read_csv() function.
This reads the file and stores it in a DataFrame called df, which allows us to explore and analyze the dataset.

- After loading, we use df.head() to display the first few rows and confirm that the data has been imported correctly.

# Data Cleaning & Pre-processing

Data cleaning and preprocessing are essential steps to improve the quality, accuracy, and reliability of a dataset before performing Exploratory Data Analysis (EDA).

## Real-world datasets often contain issues such as:
	•	Missing or incomplete values
	•	Duplicate rows
	•	Incorrect or inconsistent data types
	•	Extra spaces, special characters, or formatting errors
	•	Outliers or unexpected values
	•	Unnecessary or irrelevant columns

## Cleaning the data ensures:
	•	✔ The dataset is consistent and structured
	•	✔ Analysis and visualizations become accurate
	•	✔ Models and insights are reliable
	•	✔ Easy interpretation during EDA

### Steps included in this project’s cleaning process:
	1.	Checking dataset structure (shape, info, describe)
	2.	Handling missing values
	3.	Removing duplicate rows
	4.	Correcting data types (numeric → float/int, categorical → category)
	5.	Cleaning column values (removing spaces, symbols, formatting fixes)
	6.	Creating derived/engineered columns (like Total, Gross Income, etc.)
	7.	Saving the cleaned dataset for further analysis

This preprocessing step ensures the dataset is ready for efficient and meaningful Exploratory Data Analysis.

# 📊 Dataset Structure & Initial Understanding

## Before performing any cleaning or analysis, it is important to understand the overall structure of the dataset. This helps us verify that the data has loaded correctly and gives insights into:
	•	Number of rows and columns
	•	Column names and their data types
	•	Presence of missing values
	•	Basic statistical summary of numerical fields

These checks help us plan what cleaning steps are needed.
###  1. Checking the Dimensions of the Dataset

df.shape displays the number of rows and columns.
This help us understand how large the dataset is.

### Column Types and Dataset Structure
 In this step, we examine the structure of the dataset to understand:
- The total number of columns
- The data type of eachIn column
- Whether there are any missing values

This helps ensure that all columns are correctly formatted before further analysis.
### Missing Value Analysis

In this step, we check whether the dataset contains any missing or null values.
Identifying missing values is important to ensure data quality and to decide
whether cleaning or imputation is required before analysis.

### Duplicate Value Analysis

In this step, we check whether the dataset contains any duplicate records.
Duplicate data can affect analysis accuracy, so identifying and handling
duplicates is an important part of data preprocessing.

### Converting Selected Columns to Categorical Data Type

In this step, selected columns are converted to categorical data types.
Categorical conversion helps improve memory efficiency and ensures that
non-numeric variables are treated correctly during analysis and visualization.

### Date & Time Standardization

In this step, we standardize the Date and Time columns to ensure consistency and accuracy for time-based analysis.

# What we do in this step:
	•	Convert the Date column into a proper datetime format.
	•	Standardize the Time column to handle mixed time formats.
	•	Combine Date and Time into a single DateTime column.

# Why this is needed:
	•	Enables accurate time-based analysis (hourly, daily, monthly trends).
	•	Ensures consistency across all timestamp values.
	•	Prepares the dataset for advanced analysis and visualization.

  # Date & Time Standardization
	•	Converted the Date column to a proper datetime format.
	•	Standardized the Time column to handle mixed time formats.
	•	Combined Date and Time into a single DateTime column.
	•	Ensured all timestamp values are consistent and ready for time-based analysis.

  # Dataset Summary

After completing data loading and preprocessing, we summarize the dataset to understand its overall structure and contents.

# Summary includes:
	•	Total number of rows and columns in the dataset.
	•	Data types of each column.
	•	Presence of missing values (if any).
	•	Overall readiness of the dataset for exploratory data analysis.

This summary helps verify that the dataset is clean, well-structured, and suitable for further analysis.

# Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) is the process of exploring and understanding the dataset using summary statistics and visualizations.
It helps identify patterns, trends, distributions, and potential anomalies in the data before performing deeper analysis or modeling.

⸻

## Usage of EDA in This Project
	•	To understand the distribution of categorical and numerical variables
	•	To identify patterns, trends, and dominant categories
	•	To detect any imbalance or irregularities in the dataset
	•	To generate insights that support further analysis and reporting

⸻

## What Is Done Here
	•	Performed univariate analysis on categorical columns
	•	Visualized the frequency of each category using count plots
	•	Identified the most common categories across different features

⸻

# Univariate Analysis – Categorical Columns

Univariate analysis focuses on analyzing one variable at a time.
In this section, categorical variables are analyzed individually to understand their frequency distribution and identify the most common categories.

⸻

## Techniques Used
	•	Count plots are used to show the frequency of each category
	•	Helps compare category distributions across different features
  # City Distribution:
    Displays the number of transactions recorded in each city.

  # Branch Distribution:
    Shows the count of transactions across different supermarket branches.

# Customer Type Distribution
    Displays the frequency of Member and Normal customers.

# Gender Distribution
    Shows how transactions are distributed between male and female customers.

# Product Line Distribution
    Shows the frequency of sales across different product categories.

# Payment Method Distribution
    Displays the usage of different payment methods used by customers.

    # Univariate Analysis – Numerical Columns

# Usage:
	•	To understand how each numerical variable is distributed individually.
	•	To identify the spread, skewness, and common value ranges of numeric data.
	•	To detect outliers or unusual patterns in numerical features.

# What is done here:
	•	Performed univariate analysis on numerical columns.
	•	Used histograms to visualize the frequency distribution of values.
	•	Applied KDE (Kernel Density Estimation) curves to understand the smooth distribution pattern.
	•	Analyzed variables such as unit price, quantity, sales, tax, gross income, and rating separately.
## Bivariate Analysis – Relationship Between Variables

Bivariate analysis is used to study the relationship between two variables at a time.  
It helps in comparing how one variable changes with respect to another.

### What is done here
- Product Line vs Sales:  Identifies which product line generates the highest total sales.
- Branch vs Gross Income:  Compares income earned by different supermarket branches.
- Gender vs Rating:  Analyzes whether customer ratings differ based on gender.

### Purpose
- To understand relationships between categorical and numerical variables  
- To compare performance across different categories  
- To identify meaningful patterns that support business insights
  ## Create DateTime and Time-based Features

This step combines the Date and Time columns into a single DateTime feature and extracts useful time-based components.

### What is done
- Combined `Date` and `Time` into a single `DateTime` column
- Extracted Hour, Day, and Month from the DateTime column

### Purpose
- To enable time-based analysis such as hourly, daily, and monthly trends
- To support further analysis like peak hours, busy days, and seasonal patterns
  # SALES BY HOUR OF THE DAY
      Shows how sales vary across different hours.
      Helps identify peak business hours.
  # DAILY SALES TREND
      Displays total sales across different dates.
      Helps observe overall sales patterns and fluctuations over time.
  
  # SALES BY DAY OF WEEK
      Compares total sales across days of the week.
      Helps identify high-performing and low-performing days.
# Correlation Analysis
- Shows how strongly numerical variables are related to each other
- Correlation values range from -1 to +1

# Usage
-   Helps understand relationships between numerical features
-   Identifies variables that increase or decrease together
-  Useful for feature selection and business insights

# What is done here
- Selected only numerical columns from the dataset
- Calculated correlation values between features
- Visualized the correlations using a heatmap

#FEATURE ENGINEERING
- Feature engineering is the process of creating new meaningful features from existing data

Usage
- Helps improve data understanding
- Makes patterns easier to analyze
- Supports better insights and analysis

What is done here
- Combined Date and Time columns to create a single DateTime feature
- Extracted Hour, Day, Month, and Weekday from the DateTime column
- Created time-based features to analyze sales trends
  
## Key Insights From EDA
- Fashion Accessories and Food & Beverages show the highest total sales.
- Most customers belong to the **Member** category.
- Female customers slightly outnumber male customers.
- E-Wallet and Cash are the most preferred payment methods.
- The busiest sales hours fall between **1 PM to 8 PM**.
- Tuesday and Saturday record the highest sales among all weekdays.
- Gross income is strongly correlated with **Sales**, **COGS**, and **Quantity**.
- Branch A and Branch C generate more sales than Branch B.
- Product lines like Fashion Accessories have higher customer ratings.
# FEATURE ENGINEERING
Feature engineering is the process of creating new meaningful features from existing data to improve analysis and gain better insights.

### Creating New Features
- New profit-based features were created to better understand the financial performance of each transaction.
- Gross profit was calculated by subtracting cost of goods sold (COGS) from gross income.
- Profit margin was calculated to measure profitability as a percentage relative to cost.
- These features help compare profitability across different products, branches, and time

# Feature Engineering – Date and Time

Date and time feature engineering converts raw date and time values into structured formats that enable time-based analysis. This helps identify trends, patterns, and peak periods in sales data.
###  Date Conversion
The Date column is converted into datetime format to ensure consistency and allow accurate extraction of date-related features.
### Extracting Date Features -
 Day, month, and weekday are extracted from the Date column to analyze sales behavior across different days, months, and weekdays.

# Time Feature Engineering

The Time column is converted into datetime format and the hour is extracted to study sales distribution across different hours of the day.


## Importance of Date and Time Features

These features help uncover temporal patterns such as peak sales hours, high-performing days, and seasonal trends, supporting better business and operational decisions.
  

### Insights From Engineered Features

- Profit margin stays constant at 5% across all transactions.
- Gross profit increases as gross income increases.
- Sales happen mostly during afternoon and evening hours.
- Sunday and Friday appear to be busy days based on transaction dates.
- Monthly patterns show activity during the first quarter of the year.

  # Visualizations for engineered features
- Visualizations are used to analyze the newly created features such as profit, profit margin, hour, weekday, and month.
- They help understand how engineered features behave across time, branches, and product categories.
- Bar plots are used to compare sales and profit across hours, weekdays, and branches.
- Line plots are used to observe trends in sales and profit over time.
- These visualizations help identify peak hours, high-profit periods, and better-performing days.
- Overall, they validate the usefulness of engineered features and convert them into actionable insights.

   # Final Conclusion

The analysis of the supermarket dataset provides meaningful insights into customer behavior, sales trends, and product performance. Using Exploratory Data Analysis (EDA), feature engineering, and visualizations, several important patterns were identified that reflect the overall business performance.


   ### Key Takeaways

    • Fashion Accessories and Food & Beverages consistently generate the highest sales across all branches.
    • A majority of customers belong to the Member category, indicating strong customer loyalty.
    • Female customers slightly outnumber male customers in total purchases.
    • E-Wallet and Cash are the most commonly used payment methods.
    • Sales peak during the afternoon and evening hours, especially between 1 PM and 8 PM.
    • Tuesday and Saturday record the highest sales among all weekdays.
    • Gross income shows a strong positive relationship with sales value and quantity sold.
    • Branch A and Branch C outperform Branch B in terms of total sales.
    • Product lines such as Fashion Accessories receive higher customer ratings.
    • Profit margin remains almost constant at 5% across all transactions, indicating a fixed pricing strategy.

# Overall Conclusion

The supermarket performs best during weekends and in specific high-demand product categories. Members form the core customer base, and digital payment methods are widely adopted. The consistent profit margin suggests a stable pricing policy across products and branches. These insights can support better inventory management, targeted promotions, and improved branch-level business decisions.
# Future Scope

### This project can be further enhanced and expanded in the following ways:
	•	Predictive Modeling: Machine learning models can be applied to forecast future sales, demand, and customer purchase behavior.
	•	Customer Segmentation: Clustering techniques can be used to group customers based on spending patterns, frequency, and preferences for targeted marketing.
	•	Advanced Time-Series Analysis: Seasonal and trend analysis can be performed to better understand long-term sales patterns.
	•	Profit Optimization: Dynamic pricing strategies can be explored instead of a fixed profit margin to improve profitability.
	•	Real-Time Dashboard: Interactive dashboards using tools like Power BI or Tableau can be created for real-time business monitoring.
	•	External Data Integration: Incorporating external factors such as holidays, promotions, or weather can improve analysis accuracy.
	•	Recommendation Systems: Product recommendation systems can be developed to enhance customer experience and increase sales.








  




  
