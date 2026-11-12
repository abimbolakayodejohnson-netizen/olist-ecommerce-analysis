# Brazilian E-Commerce Exploratory Data Analysis

## Project Overview

This project explores the Brazilian E-Commerce Public Dataset by Olist to identify business insights relating to customer behaviour, sales trends, product performance, payment methods, delivery operations, seller performance, and customer satisfaction.

The analysis uses Python-based data analysis and statistical techniques to examine real-world e-commerce transactions and translate findings into practical business recommendations.

## Project Objectives

The objectives of this project are to:

- Examine order patterns and monthly sales trends.
- Analyse customer purchasing behaviour and repeat purchase rates.
- Investigate customer geographic distribution.
- Evaluate product and category performance.
- Examine the relationship between product characteristics and freight charges.
- Analyse payment methods and payment combinations.
- Evaluate seller performance.
- Investigate delivery performance and its relationship with customer reviews.

## Dataset

**Source:** Brazilian E-Commerce Public Dataset by Olist (Kaggle).

The dataset contains information about orders, customers, products, sellers, payments, reviews, and deliveries.

The raw dataset is not included in this repository. Download it from Kaggle and place the CSV files inside the `data/` directory before running the notebook.

**Dataset licence:** CC BY-NC-SA 4.0. Refer to the original dataset page for attribution and licence conditions.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- OpenPyXL
- Jupyter Notebook
- Git and GitHub

## Project Structure

```text
olist-ecommerce-analysis/
│
├── data/                  # Raw dataset files (not included)
│
├── notebooks/
│   └── olist_exploratory_data_analysis.ipynb
│
├── charts/                # Generated visualisations
│
├── outputs/
│   └── olist_ecommerce_business_report.xlsx
│
├── .gitignore
└── README.md
```

## Analysis Performed

### 1. Data Cleaning and Preparation
- Inspected dataset structures and data types.
- Examined missing values and duplicate records.
- Converted relevant timestamp columns to datetime.
- Prepared datasets for analysis and merging.

### 2. Order and Delivery Performance
- Examined order status distribution.
- Calculated delivery duration and delivery delays.
- Compared actual delivery dates with estimated dates.

### 3. Customer Satisfaction
- Examined review scores in relation to delivery performance.
- Used statistical testing to investigate the association between delivery performance and customer satisfaction.
- Identified differences in poor-review rates.

### 4. Payment Analysis
- Examined payment method distribution.
- Compared payment values across payment methods.
- Investigated multiple payment methods and payment combinations.

### 5. Customer Purchase Behaviour
- Analysed one-time and repeat customers.
- Calculated repeat purchase rate.
- Examined the interval between customers' first and last purchases.

### 6. Geographic Analysis
- Examined customer distribution across Brazilian states.
- Compared customer population with product-item value.
- Investigated geographic differences in average product-item value.

### 7. Product and Category Performance
- Evaluated product categories by product-item value and units sold.
- Examined average item prices and freight charges.
- Investigated relationships between product weight, dimensions, item prices, and freight values.

### 8. Sales Trends
- Examined monthly order patterns.
- Analysed monthly delivered product-item value.

### 9. Seller Performance
- Compared sellers using product-item value, item-record volume, and average item value.
- Examined the geographic distribution of high-performing sellers.

## Key Business Findings

- Repeat customers represented approximately **3.12%** of unique customers.
- Approximately **91.89%** of orders with known delivery performance arrived earlier than estimated.
- Late deliveries had an average review score of **2.27/5**, compared with **4.29/5** for early deliveries.
- Late deliveries had a poor-review rate approximately **6.66 times as high** as early deliveries.
- Credit cards accounted for approximately **73.92%** of payment records.
- Health and Beauty recorded the highest category product-item value at approximately **R$1.26 million**.
- Product weight had a strong positive correlation with average freight value (Pearson correlation: **0.923**).
- São Paulo, Rio de Janeiro, and Minas Gerais accounted for approximately **66.5%** of unique customers.
- November 2017 recorded the highest monthly order count, with **7,544 orders**.

## Business Recommendations

1. Improve delivery monitoring and investigate the causes of late deliveries.
2. Develop customer-retention strategies to encourage repeat purchases.
3. Use category performance to guide inventory and marketing decisions.
4. Consider product weight and dimensions when planning logistics and freight.
5. Maintain convenient and popular payment options.
6. Monitor seller performance using multiple operational metrics.
7. Strengthen operations in major customer markets while exploring growth opportunities elsewhere.
8. Use customer reviews to identify service and delivery problems.

## Important Analytical Considerations

- Product-item value refers to the sum of item prices and excludes freight charges.
- Some product-category and geographic analyses include all order statuses; these values should not automatically be interpreted as completed-sales revenue.
- Freight value represents the delivery charge recorded in the dataset, not necessarily the seller's actual shipping cost.
- The dataset contains incomplete periods at its beginning and end, which should be considered when interpreting monthly trends.
- Statistical correlations and associations do not establish causation.
- Purchase intervals are based on the difference between first and last purchases for repeat customers.

## Project Deliverables

- Jupyter Notebook containing the analysis.
- PNG charts illustrating key findings.
- Excel business report containing:
  - Executive Summary
  - Key Findings
  - Business Recommendations
  - Project Metrics

## Conclusion

This project demonstrates how Python-based exploratory data analysis can be used to investigate e-commerce operations, identify patterns in customer behaviour, evaluate delivery performance, and uncover opportunities for business improvement.

The findings highlight the importance of delivery reliability, customer retention, product management, and logistics planning in improving e-commerce performance.

