# Exploratory Data Analysis (EDA)

## Project

E-Commerce Order Analytics

## Objective

The objective of this phase is to analyze the cleaned e-commerce dataset
and identify meaningful business patterns, trends, customer behaviour,
and anomalies.

EDA helps transform raw data into business insights before further
analysis using SQL and visualization tools.

---

# Dataset Overview

The analysis is performed on the cleaned dataset created during Week 1.

Dataset Size:

- Rows: 1200
- Columns: 17

Dataset Grain:

Each row represents a single customer order transaction.

Primary Key:

OrderID

---

# Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# Analysis Performed

## 1. Dataset Exploration

Performed initial inspection:

- Checked dataset dimensions
- Reviewed column information
- Verified data types
- Examined sample records


## 2. Descriptive Statistics

Calculated:

- Mean
- Median
- Minimum
- Maximum
- Standard deviation


For numerical columns:

- Quantity
- UnitPrice
- ItemsInCart
- TotalPrice


## 3. Data Quality Checks

Verified:

- Missing values
- Duplicate records
- Unique values
- Category distributions


## 4. Product Analysis

Analyzed:

- Product-wise quantity sold
- Product revenue contribution


Business Question:

Which products drive sales and revenue?


## 5. Category Analysis

Compared:

- Electronics
- Furniture


Business Question:

Which category contributes more revenue?


## 6. Sales Trend Analysis

Created time-based analysis using:

- Order Year
- Order Month


Business Question:

How does revenue change over time?


## 7. Customer Behaviour Analysis

Analyzed:

- Payment method preference
- Discount usage
- Order value segments


Business Question:

How do customers purchase?


## 8. Outlier Detection

Used IQR method to identify unusual values.

Checked:

- TotalPrice
- Quantity
- UnitPrice


Purpose:

Detect abnormal transactions or high-value customers.

---

# Key Business Questions Answered

- Which products generate maximum revenue?
- Which category performs better?
- Are discounts influencing sales?
- What are the monthly/yearly sales trends?
- Are there unusual order values?

---

# Output

The EDA notebook contains:

✓ Statistical analysis  
✓ Business-focused visualizations  
✓ Trend analysis  
✓ Outlier detection  
✓ Initial insights  


---

# Next Steps

Future analysis:

- SQL-based business queries
- Power BI dashboard development
- Advanced business reporting