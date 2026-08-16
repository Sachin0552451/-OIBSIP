# Superstore Sales Data Analysis

## About the Project

This project is an exploratory data analysis of the **Superstore sales dataset**. The main goal was to understand how the business is performing by looking at sales, profit, customers, products, categories, regions, discounts, and shipping.

I worked through the dataset step by step — starting with data inspection and cleaning, then moving into exploratory analysis and visualization, and finally converting the findings into business insights and recommendations.

The analysis was performed using **Python in Google Colab**.

## Dataset

The dataset contains **9,994 records and 21 original columns** covering information such as:

* Order and shipping details
* Customer information
* Customer segments
* Product categories and sub-categories
* Regions and locations
* Sales
* Quantity
* Discount
* Profit

The dataset contains **no missing values and no completely duplicated records**.

## What I Analyzed

### 1. Data Cleaning & Preparation

Before starting the analysis, I checked the quality of the data and prepared it for further analysis.

Some of the main steps included:

* Checking dataset shape and columns
* Checking data types
* Checking missing values
* Checking duplicate records
* Converting `Order Date` and `Ship Date` into datetime format
* Checking invalid shipping dates
* Creating `Shipping Days`
* Creating Year, Month, Month Name, Quarter, and Year-Month columns
* Checking invalid sales, quantity, discount, and profit values

After preparation, the dataset contained **9,994 rows and 27 columns**, including the newly created analysis columns. The final data-quality checks showed zero missing values, zero duplicate rows, no invalid quantities, no invalid discounts, and no invalid shipping dates.

### 2. Descriptive Statistics

I used descriptive statistics to understand the basic behavior of the numerical variables.

Some important values from the analysis:

| Metric        |   Mean | Median |   Minimum |   Maximum |
| ------------- | -----: | -----: | --------: | --------: |
| Sales         | 229.86 |  54.49 |      0.44 | 22,638.48 |
| Quantity      |   3.79 |   3.00 |         1 |        14 |
| Discount      |   0.16 |   0.20 |         0 |      0.80 |
| Profit        |  28.66 |   8.67 | -6,599.98 |  8,399.98 |
| Shipping Days |   3.96 |   4.00 |         0 |         7 |

The large difference between the mean and median for Sales shows that the sales values are influenced by some high-value transactions. Profit also has a wide range, including both significant losses and high-profit transactions.

### 3. Sales Trend Analysis

I analyzed sales across different time periods to understand how the business performed from **2014 to 2017**.

The analysis includes:

* Yearly sales
* Monthly sales
* Quarterly analysis
* Year-Month trends

The analysis identified **2017 as the strongest sales year**, with sales of approximately **733,215** according to the notebook's business insights.

### 4. Customer Analysis

The dataset contains three customer segments:

* Consumer
* Corporate
* Home Office

The Consumer segment has the largest number of records, followed by Corporate and Home Office.

I also compared customer segments across regions to understand differences in sales and profitability and to identify opportunities for more targeted regional strategies.

### 5. Product Analysis

Product-level analysis was used to understand which products have the highest demand.

The project identifies the **top 10 products based on total quantity sold**. These products are important from an inventory-planning perspective because they represent strong customer demand.

One important point from the analysis is that a product selling in high quantities does not automatically mean that it is highly profitable. Sales volume, pricing, discounts, and profit should be considered separately.

### 6. Revenue by Category

The analysis compares the major product categories:

* Furniture
* Office Supplies
* Technology

This helps understand which categories contribute most to the business's overall revenue and how their performance differs.

### 7. Regional Analysis

The dataset contains four regions:

* West
* East
* Central
* South

The analysis found that the **West region was the strongest region in terms of sales and total profit**, making it an important region for understanding what is working well in the business.

### 8. Correlation Analysis

I also used correlation analysis and a heatmap to understand relationships between numerical variables.

One of the important observations was the relationship between **Discount and Profit**. The analysis showed a negative correlation, suggesting that higher discount levels are generally associated with lower profitability.

This is an important business point because increasing sales through heavy discounting does not necessarily mean the business is becoming more profitable.

## Key Business Insights

Some of the major insights from the project are:

1. Sales performance changes significantly across different years and months.
2. 2017 was the strongest sales year in the analyzed dataset.
3. Customer segments contribute differently to sales and profitability.
4. A relatively small group of products contributes strongly to unit sales.
5. The West region performed strongly in both sales and profit.
6. Discounts have an important relationship with profitability.
7. High sales do not always mean high profit.
8. Profitability should be analyzed along with revenue, product demand, customer segment, and region.

## Business Recommendations

Based on the analysis, I would recommend:

* Focus inventory and marketing efforts on high-performing categories and products.
* Keep sufficient stock of products with consistently high demand.
* Review discounting strategies instead of relying heavily on large discounts.
* Develop region-specific sales and marketing strategies.
* Track profit and profit margin along with revenue.
* Use customer segmentation to create more targeted marketing campaigns.
* Investigate products and transactions that generate high sales but low or negative profit.

## Tools & Technologies

The project was built using:

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Google Colab** – Development environment

## Project Workflow

```text
Raw Dataset
     ↓
Data Inspection
     ↓
Data Cleaning
     ↓
Data Quality Checks
     ↓
Feature Creation
     ↓
Descriptive Statistics
     ↓
Exploratory Data Analysis
     ↓
Visualization
     ↓
Business Insights
     ↓
Recommendations
     ↓
Conclusion
```

## Project Structure

```text
Superstore-Sales-Analysis/
│
├── SuperStore.ipynb
├── Superstore dataset.csv
└── README.md
```

## Conclusion

This project helped me understand how raw business data can be transformed into useful information for decision-making.

Instead of looking only at total sales, I analyzed the data from multiple perspectives — **profitability, customers, products, categories, regions, discounts, and time trends**.

The project also gave me practical experience with an end-to-end data analytics workflow, from cleaning and exploring a dataset to finding patterns and turning those patterns into business recommendations.

## Author

**Sachin Pandey**
Interested in Data Analytics, Python, and building practical technology projects.

---

If you found this project useful or have suggestions for improving the analysis, feel free to explore the repository and share your feedback.
