# 🛒 E-Commerce Sales Analytics Dashboard

![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

An end-to-end data analytics project on a real-world **UK-based e-commerce transactional dataset**. The project covers the complete pipeline — data cleaning in Python, EDA with visualizations, customer segmentation using K-Means, and an interactive Power BI dashboard for business stakeholders.

---

## 🗂️ Project Structure

```
ecommerce-sales-dashboard/
│
├── data/
│   ├── online_retail.csv             # Raw dataset
│   └── cleaned_data.csv              # Cleaned & exported from Python
│
├── notebook/
│   └── Ecommerce_Project.ipynb       # Full Python notebook (Colab)
│
├── dashboard/
│   └── screenshots/
│       └── dashboard_preview.png     # Power BI dashboard screenshot
│
└── README.md
```

---

## 📦 Dataset

| Field | Detail |
|-------|--------|
| Source | [UCI Online Retail Dataset]() |
| Records | ~541,000 transactions |
| Region | UK-based online retailer |
| Columns | InvoiceNo, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country |

---

## 🔧 Workflow

### 1️⃣ Data Cleaning — Python
- Removed rows with missing `Description`, `UnitPrice`, and `CustomerID`
- Dropped duplicates and cancelled orders (`Quantity ≤ 0`, `UnitPrice ≤ 0`)
- Converted `InvoiceDate` to datetime format
- Engineered new columns: `TotalPrice`, `Month`, `Year`
- Exported cleaned data as `cleaned_data.csv`

### 2️⃣ Exploratory Data Analysis — Python
- Monthly Sales Trend (line chart)
- Top 10 Products by Quantity Sold (bar chart)
- Top Countries by Revenue (bar chart)
- Customer Spending Distribution (histogram)

### 3️⃣ Customer Segmentation — K-Means Clustering
Customers grouped into 3 segments using `TotalSpending`, `Frequency`, and `Quantity`:

| Cluster | Profile | Business Strategy |
|---------|---------|-------------------|
| 0 | Low spenders, infrequent buyers | Re-engagement campaigns |
| 1 | Mid spenders, regular buyers | Loyalty rewards |
| 2 | High spenders, frequent buyers | VIP / premium offers |

### 4️⃣ Power BI Dashboard
Interactive dashboard built using `cleaned_data.csv`:

| KPI | Value |
|-----|-------|
| Total Revenue | 570K |
| Total Orders | 1K |
| Total Customers | 885 |
| Avg Revenue | 22.22 |

**Visuals:** Top 10 Products · Monthly Revenue Trend · Revenue vs Quantity Scatter · Customer Table · Year Slicer

### Dashboard Preview

![E-Commerce Sales Dashboard](https://github.com/santhi1701/E-Commerce-Sales-Analytics-Dashboard/blob/main/Screenshot.png)

---

## 💡 Key Insights

- 🏆 **Regency Cakestand 3 Tier** was the top revenue-generating product
- 📅 Revenue peaked in **November–December** — holiday season effect
- 🌍 **United Kingdom** accounts for over 80% of total revenue
- 👥 Most customers are low-frequency buyers — retention is a key opportunity
- 🔵 A small group of high-value customers (Cluster 2) drives disproportionate revenue

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10 | Data cleaning & EDA |
| Pandas | DataFrame operations |
| Matplotlib | Visualizations |
| Scikit-Learn | K-Means customer segmentation |
| Google Colab | Notebook environment |
| Power BI Desktop | Interactive dashboard |

---

## 🚀 How to Run

**Python Notebook**
1. Open [Google Colab](https://colab.research.google.com/) and upload `notebook/Ecommerce_Project.ipynb`
2. Upload `cleaned_data.xlsx` to the session
3. Run all cells — `cleaned_data.csv` exports automatically

**Power BI Dashboard**
1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Get Data → Text/CSV → select `data/cleaned_data.csv`
3. Build visuals or refer to the screenshot in `screenshot.png`

---

## 🙋 Author

**Santhi Kumari Muchu**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/santhi-kumari-muchu-b09762376/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github&logoColor=white)](https://github.com/santhi1701)

---

⭐ If you found this helpful, give it a star!
