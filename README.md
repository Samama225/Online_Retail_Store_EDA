# Online Retail Store EDA with Python

## 📌 Project Overview

This project is part of Coursera's hands-on guided projects. It involves performing **Exploratory Data Analysis (EDA)** on an online retail dataset to uncover insights about sales trends, customer behavior, and popular products. The dataset contains transactional data from a UK-based online retailer between **2010 and 2011**.

By cleaning, analyzing, and visualizing the data, we aim to provide actionable insights that can help optimize the store's operations, improve customer satisfaction, and guide business decisions.

---

## 📂 Dataset

* **File:** `Online Retail.xlsx`
* **Columns:**

  * `InvoiceNo` – Invoice number of the transaction
  * `StockCode` – Unique product code
  * `Description` – Product description
  * `Quantity` – Number of units purchased
  * `InvoiceDate` – Date and time of transaction
  * `UnitPrice` – Price per unit of product
  * `CustomerID` – Unique customer identifier
  * `Country` – Country where transaction occurred

---

## ⚙️ Technologies Used

* **Python 3**
* **Pandas** – Data cleaning & manipulation
* **NumPy** – Numerical operations
* **Matplotlib & Seaborn** – Data visualization

---

## 📝 Project Workflow

### 1. Data Loading

* Loaded dataset from `Online Retail.xlsx` using Pandas.

### 2. Data Cleaning

* Removed missing `CustomerID` values.
* Removed transactions with negative/zero `Quantity` and `UnitPrice`.
* Created a new column `TotalSales = Quantity * UnitPrice`.
* Converted `InvoiceDate` to datetime format.

### 3. Exploratory Data Analysis

* Descriptive statistics and summary.
* Sales trends analysis (monthly & weekday sales).
* Best-selling products.
* Top contributing countries (excluding UK).
* Most valuable customers.
* Outlier detection in `Quantity` and `UnitPrice`.

### 4. Visualization

* Line plot of **monthly sales**.
* Bar plots for **weekday sales, top products, countries, and customers**.
* Boxplots for **outlier detection**.

### 5. Key Insights

* Sales peak during **holiday months (Nov–Dec)**.
* Higher sales activity occurs on **Thursdays & Fridays**.
* A few products dominate sales volume (bulk decorative/utility items).
* **UK** is the largest market, but other countries also generate significant revenue.
* A small number of **VIP customers** contribute heavily to total sales.
* Outliers exist, possibly due to bulk corporate orders or data entry errors.

---

## 📊 Example Visuals

* Total Sales by Month
* Total Sales by Day of Week
* Top 10 Products Sold
* Top 10 Countries by Sales
* Customer Contribution

---

## 🚀 How to Run

1. Clone or download the project.
2. Place the dataset `Online Retail.xlsx` in your project folder.
3. Run the Jupyter Notebook or Python script.

```bash
pip install pandas numpy matplotlib seaborn openpyxl
python online_retail_eda.py
```

4. (Optional) Save the cleaned dataset:

```python
df.to_csv("online_retail.csv", index=False)
```

---

## ✅ Deliverables

* Cleaned dataset (`online_retail.csv`)
* EDA notebook/script with visualizations
* Final insights & business recommendations

---

## 📌 Author

**Samama Shabbir**
Data Science Enthusiast | IBM Data Science Certified | Machine Learning Learner
