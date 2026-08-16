# Festival Sales Data Analysis 📊

## 📌 Project Overview

This project performs an **Exploratory Data Analysis (EDA)** on a festival sales dataset to understand customer purchasing behavior, sales trends, and the product categories contributing to overall sales.

The analysis uses **Python, Pandas, NumPy, Matplotlib, and Seaborn** to clean the dataset, analyze customer demographics, identify high-performing states and occupations, and find the most popular product categories and products.

---

## 🎯 Objectives

The main objectives of this project are:

- Understand the structure and quality of the sales dataset.
- Clean missing, blank, and irrelevant data.
- Analyze customer demographics such as gender and age group.
- Identify states generating the highest number of orders and sales.
- Analyze purchasing behavior based on marital status.
- Understand sales contribution by occupation.
- Identify the most popular product categories.
- Find the top-selling products based on order volume.
- Generate business insights from the analysis.

---

## 📂 Dataset

**Dataset:** `Festival Sales Data.csv`

The dataset contains **11,251 records and 15 columns** before data cleaning.

### Important Columns

| Column | Description |
|---|---|
| `User_ID` | Unique customer identifier |
| `Cust_name` | Customer name |
| `Product_ID` | Product identifier |
| `Gender` | Customer gender |
| `Age Group` | Customer age group |
| `Age` | Customer age |
| `Marital_Status` | Customer marital status |
| `State` | Customer's state |
| `Zone` | Geographical zone |
| `Occupation` | Customer occupation/industry |
| `Product_Category` | Product category |
| `Orders` | Number of orders |
| `Amount` | Purchase amount |
| `Status` | Blank/irrelevant column removed during cleaning |
| `unnamed1` | Blank/irrelevant column removed during cleaning |

---

## 🛠️ Technologies & Libraries

- **Python**
- **Jupyter Notebook**
- **Pandas** – data manipulation and analysis
- **NumPy** – numerical operations
- **Matplotlib** – data visualization
- **Seaborn** – statistical visualization

---

## 🔄 Project Workflow

### 1. Import Libraries

The project starts by importing the required Python libraries:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

### 2. Load the Dataset

The CSV file is loaded into a Pandas DataFrame.

```python
df = pd.read_csv('Festival Sales Data.csv', encoding='unicode_escape')
```

### 3. Data Cleaning

The following cleaning operations are performed:

- Removed unrelated/blank columns:
  - `Status`
  - `unnamed1`
- Checked for missing values.
- Removed rows containing null values.
- Converted the `Amount` column from float to integer.

```python
df.drop(['Status', 'unnamed1'], axis=1, inplace=True)
df.dropna(inplace=True)
df['Amount'] = df['Amount'].astype('int')
```

### 4. Exploratory Data Analysis

The dataset is analyzed across several dimensions:

- Gender
- Age Group
- State
- Marital Status
- Occupation
- Product Category
- Product ID

Bar charts and count plots are used to identify patterns and trends.

---

## 📊 Key Analysis & Insights

### 👩 Gender Analysis

The analysis shows that:

- **Female customers form the majority of buyers.**
- Female customers also have higher overall purchasing power than male customers based on total purchase amount.

---

### 👥 Age Group Analysis

The analysis indicates that:

- Customers in the **26–35 years** age group are the major buyers.
- Female customers within this age group represent a particularly strong customer segment.

---

### 📍 State Analysis

The state-level analysis examines both:

- Total number of orders
- Total sales amount

The project identifies **Uttar Pradesh, Maharashtra, and Karnataka** among the leading states in terms of orders and/or total sales.

---

### 💍 Marital Status Analysis

The analysis shows that:

- Married customers represent a significant buyer segment.
- Married women show particularly high purchasing power in the analyzed dataset.

---

### 💼 Occupation Analysis

The occupation analysis highlights strong customer participation and sales contribution from sectors including:

- IT Sector
- Healthcare
- Aviation

These occupations represent important customer segments for the business.

---

### 🛍️ Product Category Analysis

The analysis identifies **Food, Clothing, and Electronics** among the major product categories based on sales/order activity.

These categories can be considered important areas for festival sales planning.

---

### 🏆 Top-Selling Products

The project also groups the data by `Product_ID` and identifies the **top 10 products by total orders**.

This helps identify products with high demand during the festival sales period.

---

## 📈 Visualizations

The notebook contains visualizations for:

- Gender-wise customer count
- Gender-wise total sales
- Age group vs gender
- Age group vs total sales
- Top 10 states by orders
- Top 10 states by sales
- Marital status distribution
- Marital status vs gender sales
- Occupation distribution
- Occupation-wise sales
- Product category distribution
- Product category-wise sales
- Top 10 products by orders

---

## 📁 Project Structure

```text
Festival-Sales-Analysis/
│
├── Festival Sales Data.csv
├── Festival_Sales_Analysis.ipynb
└── README.md
```

---

## ▶️ How to Run the Project

### Step 1: Clone the repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Open the project folder

```bash
cd Festival-Sales-Analysis
```

### Step 3: Install required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Open the notebook

Open:

```text
Festival_Sales_Analysis.ipynb
```

Run the cells sequentially to reproduce the analysis.

---

## 💡 Business Recommendations

Based on the analysis performed in this project, businesses can consider:

1. **Targeting the 26–35 age group** with festival-focused campaigns.
2. Creating marketing campaigns specifically aimed at **female customers**, who show strong purchasing activity in the dataset.
3. Focusing regional campaigns on high-performing states such as **Uttar Pradesh, Maharashtra, and Karnataka**.
4. Developing targeted offers for customers working in **IT, Healthcare, and Aviation**.
5. Promoting high-performing categories such as **Food, Clothing, and Electronics**.
6. Maintaining sufficient inventory for the most frequently ordered products during festival periods.

---

## 🚀 Skills Demonstrated

This project demonstrates practical skills in:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Aggregation
- GroupBy Operations
- Handling Missing Values
- Data Type Conversion
- Data Visualization
- Business Insight Generation
- Python for Data Analysis
- Pandas & NumPy
- Matplotlib & Seaborn

---

## 👨‍💻 Author

**Yash Baghel**

B.Tech – Electronics & Communication Engineering

### 📌 Project Type

**Data Analytics / Exploratory Data Analysis Project**

---

## ⭐ If you find this project useful

Feel free to star the repository and use the project as a reference for learning Python-based data analysis.
