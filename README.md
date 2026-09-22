# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior to identify purchasing patterns, customer segments, product preferences, subscription behavior, and revenue trends.

The project follows an end-to-end **data analytics workflow**, starting with data loading and exploratory analysis in Python, followed by data cleaning and SQL-based business analysis. The findings are then presented through an interactive **Power BI dashboard** and summarized into actionable business insights.

### Key Objectives

* Understand customer purchasing patterns
* Identify high-performing products and categories
* Analyze customer spending and revenue contribution
* Compare subscribed and non-subscribed customers
* Analyze the impact of discounts and shipping methods
* Segment customers based on previous purchasing behavior
* Present key findings through an interactive dashboard

---

## Dataset

The project uses a customer shopping behavior dataset containing information related to:

* Customer demographics
* Products purchased
* Product categories
* Purchase amounts
* Review ratings
* Discounts
* Shipping methods
* Subscription status
* Previous purchases
* Customer segments

The dataset is provided in:

`customer_shopping_behavior.csv`

---

## Tools & Technologies

| Tool                                | Purpose                                   |
| ----------------------------------- | ----------------------------------------- |
| **Python**                          | Data loading, exploration and analysis    |
| **Pandas**                          | Data manipulation and cleaning            |
| **Matplotlib / Seaborn**            | Exploratory data visualization            |
| **SQL**                             | Business-oriented data analysis           |
| **PostgreSQL / MySQL / SQL Server** | Database querying                         |
| **Power BI**                        | Interactive dashboard and visualization   |
| **Jupyter Notebook**                | Python-based analysis                     |
| **GitHub**                          | Project documentation and version control |

---

## Project Workflow

### 1. Data Loading

The dataset was imported into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")
```

The initial dataset was examined to understand:

* Number of records and columns
* Data types
* Missing values
* Duplicate records
* Basic statistical characteristics

---

### 2. Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to identify patterns and relationships within the dataset.

The analysis included:

* Distribution of customer demographics
* Purchase amount analysis
* Product and category performance
* Customer subscription behavior
* Review rating analysis
* Discount usage
* Shipping preferences
* Previous purchase behavior

Visualizations were used to better understand important trends and relationships.

---

### 3. Data Cleaning & Preparation

The dataset was cleaned and prepared for further analysis.

Key activities included:

* Handling missing values
* Checking for duplicate records
* Correcting data types
* Standardizing categorical values
* Creating useful derived columns
* Preparing the dataset for SQL analysis and visualization

The cleaned data was then used for downstream analysis.

---

### 4. SQL Analysis

The cleaned dataset was loaded into a relational database and analyzed using SQL.

The project includes business-oriented SQL queries covering areas such as:

* Revenue by gender
* Customers spending above average
* Highest-rated products
* Standard vs. Express shipping spending
* Subscriber vs. non-subscriber spending
* Products with the highest discount usage
* Customer segmentation
* Top products within each category
* Repeat buyers and subscription behavior
* Revenue contribution by age group

The SQL analysis uses concepts including:

* `GROUP BY`
* Aggregate functions
* `CASE`
* Subqueries
* CTEs
* Window functions
* `ORDER BY`
* Filtering and conditional logic

SQL queries are available in:

`customer_behavior_sql_queries.sql`

---

## Dashboard

An interactive Power BI dashboard was created to present the key findings from the analysis.

The dashboard focuses on:

* Customer demographics
* Revenue and purchase behavior
* Product performance
* Customer segmentation
* Subscription analysis
* Discount and shipping patterns
* Category-level insights

Power BI dashboard file:

`customer_behavior_dashboard.pbix`

The dashboard is designed to allow users to interactively explore customer behavior and identify important business trends.

---

## Key Results & Insights

The analysis provides insights into:

* Customer purchasing and spending patterns
* Revenue contribution across different customer groups
* Product and category performance
* Differences between subscribed and non-subscribed customers
* The relationship between repeat purchasing and subscription behavior
* Discount usage across products
* Customer segmentation based on previous purchases
* Differences in spending across shipping methods and demographic groups

These findings can help businesses better understand their customers and support decisions related to **customer retention, product strategy, promotions, and revenue growth**.

---

## Project Structure

```text
Customer-shopping-behavior-analysis/
│
├── Customer_Shopping_Behavior_Analysis.ipynb
├── customer_behavior_sql_queries.sql
├── customer_shopping_behavior.csv
├── customer_behavior_dashboard.pbix
├── Business Problem Document.pdf
└── README.md
```

---

## How to Run

### Python Analysis

1. Clone the repository:

```bash
git clone https://github.com/divyansh282/Customer-shopping-behavior-analysis.git
```

2. Navigate to the project folder:

```bash
cd Customer-shopping-behavior-analysis
```

3. Install the required Python libraries:

```bash
pip install pandas matplotlib seaborn jupyter
```

4. Open the Jupyter Notebook:

```bash
jupyter notebook Customer_Shopping_Behavior_Analysis.ipynb
```

5. Run the notebook cells sequentially to reproduce the data analysis and visualizations.

---

### SQL Analysis

1. Create a database using **PostgreSQL, MySQL, or SQL Server**.
2. Import `customer_shopping_behavior.csv` into a table named `customer`.
3. Open:

```text
customer_behavior_sql_queries.sql
```

4. Execute the queries in your database environment.

> **Note:** Some SQL syntax may need minor adjustments depending on the database system being used. For example, PostgreSQL-specific syntax such as `::numeric` may need to be modified for MySQL or SQL Server.

---

### Power BI Dashboard

1. Install Microsoft Power BI Desktop.
2. Open:

```text
customer_behavior_dashboard.pbix
```

3. If required, update the data source path to the location of the dataset.
4. Refresh the data and explore the dashboard.

---

## Files Included

| File                                        | Description                           |
| ------------------------------------------- | ------------------------------------- |
| `Customer_Shopping_Behavior_Analysis.ipynb` | Python-based data analysis and EDA    |
| `customer_shopping_behavior.csv`            | Customer shopping behavior dataset    |
| `customer_behavior_sql_queries.sql`         | SQL business analysis queries         |
| `customer_behavior_dashboard.pbix`          | Interactive Power BI dashboard        |
| `Business Problem Document.pdf`             | Business problem and analysis context |

---

## Skills Demonstrated

**Data Analytics:**
Exploratory Data Analysis, Data Cleaning, Data Preparation, Business Analysis

**Python:**
Pandas, Data Analysis, Data Visualization

**SQL:**
Joins, Aggregations, Subqueries, CTEs, CASE Statements, Window Functions

**Power BI:**
Dashboard Development, Data Visualization, Interactive Reporting

**Business Skills:**
Customer Segmentation, Revenue Analysis, Product Analysis, Insight Generation

---

## Conclusion

This project demonstrates an end-to-end approach to solving a business analytics problem — from **raw data preparation and exploratory analysis to SQL-based business analysis and interactive Power BI reporting**.

The project focuses on converting customer transaction data into meaningful insights that can support data-driven business decisions.
