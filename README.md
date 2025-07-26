# 📊 RFM Analysis on E-commerce Customer Data

## 🧩 Problem Statement & Objective

**Problem Statement:**  
E-commerce companies accumulate massive customer transaction data but often fail to utilize it effectively for strategic decision-making. Segmenting customers based on their purchasing behavior can improve marketing ROI, customer retention, and lifetime value.

**Objectives:**
- Apply **RFM (Recency, Frequency, Monetary)** analysis to segment customers.
- Use **Pareto (80/20) Analysis** to identify top contributors to revenue.
- Build a **Power BI dashboard** for interactive visualization and reporting.
- Enable data-driven decision-making for targeted marketing strategies.

---

## 📁 Dataset Description

- **Source**: [Kaggle - E-Commerce Dataset]([https://www.kaggle.com/](https://www.kaggle.com/datasets/adilashrafi/online-retail-big-dataset))
- **File Name**: `ecomm_data.csv`
- **Fields**:
  - `InvoiceNo`, `StockCode`, `Description`, `Quantity`
  - `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`
- Contains transaction-level data from a UK-based online retailer over the course of a year.

---

## 🛠️ Tools & Technologies Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Power BI** – Dashboard development
- **Jupyter Notebook** – Analysis and documentation
- **Excel** – Data preparation (where applicable)

---

## 📌 Methodology

### 1. Data Cleaning & Preprocessing
- Removed rows with null `CustomerID` and negative `Quantity`.
- Converted `InvoiceDate` to datetime and set analysis snapshot date.

### 2. RFM Metric Calculation
- **Recency**: Days since the customer’s last purchase.
- **Frequency**: Number of purchases.
- **Monetary**: Total spend.

### 3. Scoring & Segmentation
- Created R, F, and M scores using quantiles (1–5 scale).
- Combined scores to form RFM segments (e.g., 555 = Champions).

### 4. Pareto Analysis
- Identified top 20% of customers contributing ~80% of revenue.
- Visualized revenue contribution by segment and top customers.

### 5. Power BI Dashboard
- Built a dynamic dashboard to explore:
  - Segment-wise revenue contributions
  - Customer distribution
  - Revenue by day of the week
  - RFM Heatmap
  - Top/Bottom customers
  - Time-series trend of active customers

---

## 📈 Key Insights

- **65%+ customers** are **dormant**, requiring reactivation campaigns.
- **Top 20% customers** contribute to nearly **80% of revenue** (Pareto Principle).
- **Thursdays** recorded the highest revenue generation.
- RFM Heatmap revealed strong clusters of high-spending frequent customers.

---

## 📊 Power BI Dashboard Preview

![Power BI Dashboard](./558354ac-af34-452a-8b98-851f1ff04138.png)
<img width="1317" height="732" alt="Screenshot 2025-07-26 164316" src="https://github.com/user-attachments/assets/6276589a-0ad1-421f-ade0-fb913faa7d50" />

---
