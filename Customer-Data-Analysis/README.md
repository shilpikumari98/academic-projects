
# Customer Data Analysis

## Overview
This project aims to analyze customer data, focusing on key insights such as distribution by country, subscription trends, and customer segmentation by various attributes such as company, email domain, and city. The data is visualized using various plotting techniques including bar plots and pie charts.

## Project Description
The dataset contains customer details including `Customer Id`, `First Name`, `Last Name`, `Company`, `City`, `Country`, `Phone 1`, `Phone 2`, `Email`, `Subscription Date`, and `Website`. Through this project, various analyses are performed, including:

- **Data Cleaning**: Handling missing or invalid data, normalizing phone numbers, and validating email formats.
- **Customer Distribution**: Visualization of customer distribution by country and city.
- **Customer Segmentation**: Analyzing and visualizing the distribution of customers by company and email domain.
- **Data Validation**: Ensuring that data such as phone numbers and emails are valid and properly formatted.

## Technologies Used
- **Python**
  - Pandas: Data manipulation and cleaning
  - Matplotlib: Data visualization (Bar plots, Pie charts)
- **Jupyter Notebooks** (for easy data exploration and visualization)

## Data Cleaning Steps
- **Phone Numbers**:
  - Removed non-numeric characters from phone numbers.
  - Validated phone numbers for correct length (10 digits).
- **Email**:
  - Validated email formats using regular expressions.
  - Extracted and visualized the most common email domains.
- **Date**:
  - Converted subscription date to datetime format for analysis.

## Visualizations Created
1. **Top 5 Countries with Highest Number of Customers**: A **bar plot** showing the top 5 countries with the highest number of customers.
2. **Top 5 Companies with Highest Customers**: A **bar plot** showing the top 5 companies with the most customers.
3. **Top 5 Cities with Highest Customers**: A **bar plot** showing the top 5 cities with the most customers.
4. **Top 5 Email Domains**: A **pie chart** displaying the most common email domains among customers.

## Steps Involved
1. **Data Loading**: Load the customer data into a DataFrame.
2. **Data Cleaning**: Handle missing values, validate and clean phone numbers and emails.
3. **Feature Engineering**: Extract additional features like email domain 
4. **Visualization**: Generate various plots to visualize the data and trends.
