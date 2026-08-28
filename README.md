# Retail Sales — Exploratory Data Analysis

## 📊 Project Overview

This project performs an **Exploratory Data Analysis (EDA)** on a retail sales transaction dataset to identify sales trends, customer behavior patterns, and product/category performance.

The analysis uses **2,000 retail transactions from 2022–2023**, containing information about customers, demographics, product categories, quantities, pricing, cost of goods sold (COGS), and total sales value.

The goal is to transform raw transaction data into meaningful insights that can support **data-driven business decisions**.

---

## 🎯 Objectives

The analysis focuses on:

* Understanding the structure and quality of the dataset
* Identifying and handling missing values
* Calculating descriptive statistics
* Analyzing monthly and quarterly sales trends
* Understanding customer demographics and purchasing behavior
* Comparing product/category performance
* Examining relationships between numerical variables
* Identifying actionable business insights and recommendations

---

## 🗂️ Dataset

The dataset contains **2,000 individual sales transactions** across 2022 and 2023.

### Main Features

| Column            | Description                   |
| ----------------- | ----------------------------- |
| `transactions_id` | Unique transaction identifier |
| `sale_date`       | Date of the transaction       |
| `sale_time`       | Time of the transaction       |
| `customer_id`     | Customer identifier           |
| `gender`          | Customer gender               |
| `age`             | Customer age                  |
| `category`        | Product category              |
| `quantiy`         | Number of units purchased     |
| `price_per_unit`  | Price per unit                |
| `cogs`            | Cost of goods sold            |
| `total_sale`      | Total transaction value       |

> **Note:** The original dataset contains the column name `quantiy`. The spelling was retained to match the source data.

---

## 🛠️ Technologies & Libraries

* **Python**
* **Pandas** — Data manipulation and analysis
* **NumPy** — Numerical operations
* **Matplotlib** — Data visualization
* **Seaborn** — Statistical visualization
* **Jupyter Notebook** — Development environment

---

## 🔍 Analysis Workflow

### 1. Data Loading & Initial Inspection

The dataset is loaded using Pandas and initially inspected to understand:

* Dataset dimensions
* Column names
* Data types
* Missing values
* Sample records

The dataset contains **2,000 rows and 11 columns**.

---

### 2. Data Cleaning

Missing-value analysis identified missing values in:

* `age`
* `quantiy`
* `price_per_unit`
* `cogs`
* `total_sale`

The missing values represented a very small portion of the dataset. Rows with missing values in the key numerical fields used for calculations were removed.

After cleaning, **1,997 rows** remained.

Additional features were created for analysis:

* `month`
* `quarter`
* `hour`
* `profit`

Profit was calculated as:

```text
Profit = Total Sale − COGS
```

---

### 3. Descriptive Statistics

Statistical analysis was performed on:

* Customer age
* Quantity purchased
* Price per unit
* COGS
* Total sales

Some key observations include:

* Average customer age: **~41 years**
* Average quantity per transaction: **~2.5 units**
* Average transaction value: **~$457**
* Median transaction value: **$150**
* Maximum transaction value: **$2,000**

The significant difference between the mean and median transaction values indicates that a smaller number of high-value transactions substantially increase the average transaction value.

---

### 4. Time Series Analysis

Monthly and quarterly sales trends were analyzed to identify:

* Revenue fluctuations
* Seasonal patterns
* High-performing periods
* Low-performing periods
* Changes in sales activity over time

Visualizations were created to make these trends easier to interpret.

---

### 5. Customer Analysis

Customer demographics and purchasing behavior were explored using variables such as:

* Age
* Gender
* Customer ID
* Transaction value
* Purchase quantity

This helps identify characteristics of the customer base and understand how different customer groups contribute to sales.

---

### 6. Product & Category Analysis

Sales performance was analyzed across product categories to understand:

* Which categories generate the most revenue
* Category-level purchasing patterns
* Differences in transaction values
* Opportunities for improving product performance

---

### 7. Correlation Analysis

Relationships between numerical variables were examined using correlation analysis and visualization.

This helps understand relationships between variables such as:

* Quantity
* Price per unit
* COGS
* Total sales
* Profit

---

## 💡 Key Findings

The analysis revealed several useful patterns:

* The dataset contains a broad adult customer base, with ages ranging from **18 to 64**.
* The average customer age is approximately **41 years**.
* Customers purchase approximately **2.5 units per transaction on average**.
* The average transaction value is considerably higher than the median, indicating that high-value purchases have a strong effect on overall revenue statistics.
* Retail sales vary across different periods, making time-based analysis useful for identifying stronger and weaker sales periods.
* Product categories show differences in sales performance and customer purchasing behavior.

---

## 📈 Visualizations

The notebook uses multiple visualizations to communicate the analysis, including:

* Monthly sales revenue trends
* Quarterly sales analysis
* Customer demographic distributions
* Category-level sales comparisons
* Correlation heatmaps
* Other supporting statistical visualizations

These visualizations are used alongside written observations rather than being presented without interpretation.

---

## 📌 Business Recommendations

Based on the analysis, businesses can consider:

1. **Focus on high-performing product categories**
   Allocate inventory, marketing, and promotional resources toward categories that consistently generate strong sales.

2. **Use seasonal sales patterns for planning**
   Historical monthly and quarterly trends can help businesses improve inventory planning, staffing, and promotional campaigns during stronger and weaker periods.

3. **Develop customer-focused strategies**
   Customer demographic and purchasing patterns can be used to create more targeted promotions and improve customer engagement.

---

## 📁 Project Structure

```text
Retail-Sales-EDA/
│
├── DataAnalytics-L1-EDARetailSales.ipynb
├── Retail_Sales.csv
└── README.md
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <repository-url>
```

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Open the notebook

```bash
jupyter notebook DataAnalytics-L1-EDARetailSales.ipynb
```

Make sure `Retail_Sales.csv` is located in the appropriate directory so that the notebook can load the dataset.

---

## 📚 Skills Demonstrated

This project demonstrates practical skills in:

* Exploratory Data Analysis
* Data Cleaning
* Missing Value Analysis
* Descriptive Statistics
* Feature Engineering
* Time Series Analysis
* Customer Analysis
* Product/Category Analysis
* Correlation Analysis
* Data Visualization
* Business Insight Generation
* Data-driven Recommendations

---
