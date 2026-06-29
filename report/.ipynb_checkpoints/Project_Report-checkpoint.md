# Integrated Data Analysis and Visualization Project Report

# Walmart Customer Purchases Dataset

# Submitted By
Name: Arshad

Course: B.Tech – Artificial Intelligence & Data Science

---

# Table of Contents

1. Introduction
2. Problem Statement
3. Objectives
4. Dataset Description
5. Tools and Technologies Used
6. Data Loading
7. Data Cleaning and Preprocessing
8. Exploratory Data Analysis (EDA)
9. Time-Series Analysis
10. Categorical Analysis
11. Relationship Analysis
12. Distribution Analysis
13. Correlation Analysis
14. Key Insights
15. Conclusion
16. Future Scope

---

# 1. Introduction

Data analysis plays a vital role in understanding customer behavior and business performance. Retail organizations generate enormous amounts of transactional data every day. Proper analysis of this data helps businesses identify purchasing trends, improve customer experience, optimize inventory, and increase revenue.

This project performs a complete Exploratory Data Analysis (EDA) on the Walmart Customer Purchases dataset. Using Python and popular data science libraries such as Pandas, NumPy, Matplotlib, and Seaborn, the dataset is cleaned, explored, visualized, and analyzed to discover meaningful business insights.

The project demonstrates the complete workflow of a real-world data analysis project, beginning with data loading and ending with interpretation of the results.

---

# 2. Problem Statement

The objective of this project is to analyze customer purchasing behavior using the Walmart Customer Purchases dataset.

The project aims to answer questions such as:

* Which product categories generate the highest sales?
* Which cities contribute the most revenue?
* How do sales change over time?
* Which payment methods are most commonly used?
* Is there any relationship between customer age and purchase amount?
* Are there unusual purchasing patterns or outliers?
* What business insights can be obtained from the available data?

---

# 3. Objectives

The major objectives of this project are:

* Load the dataset using Pandas.
* Perform data cleaning and preprocessing.
* Identify missing values and duplicate records.
* Generate descriptive statistics.
* Analyze sales trends over time.
* Compare sales across different product categories.
* Analyze customer purchases across cities.
* Study payment method preferences.
* Explore relationships between numerical variables.
* Visualize data using professional graphs.
* Summarize important findings.

---

# 4. Dataset Description

The dataset contains customer purchase records collected from Walmart transactions.

The important attributes include:

| Column           | Description                            |
| ---------------- | -------------------------------------- |
| Customer_ID      | Unique customer identifier             |
| Age              | Customer age                           |
| Gender           | Customer gender                        |
| City             | Customer city                          |
| Category         | Product category                       |
| Product_Name     | Purchased product                      |
| Purchase_Date    | Date of purchase                       |
| Purchase_Amount  | Amount spent                           |
| Payment_Method   | Mode of payment                        |
| Discount_Applied | Indicates whether discount was applied |
| Rating           | Customer rating                        |
| Repeat_Customer  | Indicates repeat customer status       |

The dataset consists of customer demographics together with transaction information, making it suitable for sales and customer behavior analysis.

---

# 5. Tools and Technologies Used

Programming Language

* Python

Development Environment

* Jupyter Notebook

Libraries Used

* Pandas
* NumPy
* Matplotlib
* Seaborn

Version Control

* Git
* GitHub

---

# 6. Data Loading

The dataset was loaded into Python using the Pandas library.

The dataset was imported from a CSV file into a DataFrame.

After loading, the following preliminary checks were performed:

* Displaying first few rows
* Displaying last few rows
* Dataset dimensions
* Column names

These checks ensured that the dataset had been imported successfully.

---

# 7. Data Cleaning and Preprocessing

Before analysis, the dataset was cleaned to improve data quality.

The following preprocessing steps were performed:

### Data Type Verification

The data types of every column were examined using:

* df.info()
* df.dtypes

---

### Date Conversion

The Purchase_Date column was converted into DateTime format to enable time-series analysis.

---

### Missing Value Detection

Missing values were checked using:

* df.isnull().sum()

The dataset contained minimal or no missing values. Any missing values identified were handled appropriately before further analysis.

---

### Duplicate Detection

Duplicate records were identified using:

* df.duplicated().sum()

Duplicate rows, if any, were removed to ensure data integrity.

---

### Statistical Summary

Descriptive statistics including:

* Mean
* Median
* Minimum
* Maximum
* Standard Deviation

were generated using:

* df.describe()

This provided a quick overview of the numerical variables.

---

# 8. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand the structure and characteristics of the dataset.

The following analyses were conducted:

* Dataset dimensions
* Data types
* Missing values
* Duplicate values
* Descriptive statistics
* Distribution of numerical variables
* Category-wise analysis
* City-wise analysis

EDA helped in understanding customer purchasing patterns before performing deeper analysis.

---

# 9. Time-Series Analysis

Purchase dates were converted into monthly and quarterly periods.

Monthly purchase totals were calculated by grouping the Purchase_Date column.

Line charts were created to visualize monthly sales trends.

Quarterly sales were also aggregated and displayed using bar charts.

These visualizations helped identify fluctuations in purchasing behavior over time and highlighted periods of higher or lower sales activity.

*(Insert Monthly Sales Trend graph here.)*

*(Insert Quarterly Sales graph here.)*

---

# 10. Categorical Analysis

Several categorical variables were analyzed.

### Sales by Product Category

A bar chart was created to compare total purchase amounts across product categories.

This visualization helped identify the highest-performing product categories.

*(Insert Sales by Category graph here.)*

---

### Sales by City

Total purchase amount was calculated for each city.

Cities were sorted according to total sales and displayed using a bar chart.

This analysis identified locations generating the highest revenue.

*(Insert Sales by City graph here.)*

---

### Payment Method Distribution

Customer payment methods were analyzed using a chart showing the frequency of each payment method.

This visualization illustrated customer payment preferences.

*(Insert Payment Method Distribution graph here.)*

---

# 11. Relationship Analysis

Relationships between numerical variables were examined using scatter plots.

### Age vs Purchase Amount

This visualization helped determine whether customer age influenced purchasing behavior.

### Rating vs Purchase Amount

This graph examined whether higher customer ratings were associated with larger purchase amounts.

The scatter plots suggested that while certain clusters exist, strong linear relationships may not always be present.

*(Insert Scatter Plot graphs here.)*

---

# 12. Distribution Analysis

Distribution analysis was performed using histograms and box plots.

### Purchase Amount Distribution

A histogram illustrated how purchase amounts are distributed across customers.

This helped identify whether the data followed a normal distribution or was skewed.

---

### Purchase Amount Box Plot

The box plot highlighted:

* Median purchase amount
* Interquartile range
* Potential outliers

Outliers indicate unusually high or low purchases.

*(Insert Histogram and Box Plot here.)*

---

# 13. Correlation Analysis

A correlation heatmap was generated using numerical columns.

The heatmap illustrated relationships between variables such as:

* Age
* Purchase Amount
* Rating

Positive correlations indicate variables increasing together, while negative correlations indicate inverse relationships.

This analysis helps identify variables that may be useful for future machine learning models.

*(Insert Correlation Heatmap here.)*

---

# 14. Key Insights

The following observations were obtained from the analysis:

* Product categories contribute differently to total sales, with some categories generating significantly higher revenue.
* Customer purchases vary across different cities, indicating regional differences in purchasing behavior.
* Monthly sales fluctuate over time, suggesting seasonal or promotional influences.
* Payment method analysis reveals customer preferences for specific modes of payment.
* Purchase amounts exhibit variability, with a small number of high-value transactions identified as outliers.
* Scatter plots indicate limited visible relationships between age and purchase amount, although customer demographics remain useful for segmentation.
* Correlation analysis shows the strength of relationships among numerical variables and highlights potential features for future predictive modeling.

---

# 15. Conclusion

This project successfully demonstrated an end-to-end data analysis workflow using Python.

Beginning with data loading and preprocessing, the project progressed through exploratory data analysis, statistical summaries, visualization, and interpretation of results.

The generated visualizations provided valuable insights into customer purchasing behavior, product category performance, city-wise sales distribution, payment preferences, and purchase trends over time.

The project highlights how data analysis can transform raw transactional data into meaningful business information that supports better decision-making.

---

# 16. Future Scope

The project can be extended in several ways:

* Build predictive machine learning models for sales forecasting.
* Perform customer segmentation using clustering algorithms.
* Predict repeat customers.
* Develop an interactive dashboard using Power BI or Tableau.
* Deploy the analysis as a web application using Streamlit.
* Integrate real-time sales data for continuous monitoring.

---

# References

* Pandas Documentation
* NumPy Documentation
* Matplotlib Documentation
* Seaborn Documentation
* Walmart Customer Purchases Dataset
* Python Official Documentation

---

<--------------------End of Report-------------------->
