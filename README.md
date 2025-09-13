# 🛒 Customer Purchase Behavior Analysis & Segmentation

### 📌 Overview
This project performs an **end-to-end analysis of retail customer purchase data** using **SQL, Python, and Power BI**.  
It focuses on customer segmentation, purchasing trends, and actionable insights to support sales & marketing strategies.

---

### 🎯 Objectives
- Identify **top-performing customer segments**
- Analyze **monthly revenue trends & customer activity**
- Perform **Pareto analysis (80/20 rule)**
- Provide **business recommendations** through interactive dashboards

---

### 📂 Project Structure
customer-purchase-behavior-analysis/

│── README.md <- Project documentation

│── scripts/

│ └── customer_segmentation.ipynb <- Google Colab (ETL, SQL queries, segmentation, exports)

│── data/

│ ├── Customer_Segmentation.csv <- Customer-level revenue & frequency with segment

│ ├── Monthly_Trends.csv <- Monthly revenue & customer activity

│ ├── Segment_Summary.csv <- Segment counts, revenue, revenue share

│ ├── Pareto_Summary.csv <- Top 10% customers revenue contribution

│── dashboard/

│ ├── dashboard.pbix <- Power BI interactive dashboard

│ └── dashboard_screenshot.png <- Preview of dashboard

---

### 🗄️ Dataset
- Source: [UCI Machine Learning Repository – Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- Transactions between **2010–2011**
- Fields: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

⚠️ Raw dataset is **not included** due to size. Please download directly from UCI.

---

### 🔧 Tools & Technologies
- **Python (Pandas, SQLite, Matplotlib)** → Data cleaning, SQL queries, segmentation, exports
- **SQL (via SQLite in Python)** → Aggregation, customer revenue & frequency, monthly trends
- **Google Sheets** → Pivot tables & charts (initial exploration)
- **Power BI** → Final dashboard (interactive visuals, slicers, KPIs)

---

### 📊 Key Analyses
1. **Customer Segmentation**
   - High Value (top 10% by revenue)
   - Frequent Low Spenders (top 25% by purchase frequency)
   - Other (remaining customers)

2. **Monthly Trends**
   - Revenue and unique customers tracked month by month

3. **Pareto Analysis (80/20 Rule)**
   - Top 10% customers contributed ~61% of revenue

---

### 📈 Dashboard Highlights (Power BI)
📌 **KPI Cards**: Total Revenue, Total Customers, Average Revenue per Customer

📌 **Revenue by Segment** (bar chart)

📌 **Customer Distribution** (pie chart)

📌 **Monthly Revenue Trend** (line chart with segment slicer)

📌 **Pareto Contribution** (top 10% vs others)

!

---

### 📑 Key Insights
- Top **10% of customers contributed ~61% of total revenue**
- **High Value** customers generate the majority of revenue despite being only ~10% of the base
- Seasonal spikes in **Nov–Dec** (holiday shopping effect)
- Large base of **“Other” customers** with low spend & low frequency

---

### 🚀 Business Recommendations
- Implement **loyalty programs** targeting **High Value** customers
- **Upsell & cross-sell** to **Frequent Low Spenders**
- Develop **re-engagement campaigns** for inactive customers
- Plan **inventory & marketing budgets** around seasonal peaks

---

### 📝 How to Reproduce
1. Download raw dataset from [UCI Online Retail](https://archive.ics.uci.edu/ml/datasets/online+retail)
2. Run `scripts/customer_segmentation.ipynb` in Jupyter/Colab
3. Export CSVs to `/data`
4. Open `dashboard/dashboard.pbix` in Power BI to explore the interactive dashboard

---

### 👨‍💻 Author
**Afsar** – MSc Statistics & Data Analytics  
Passionate about **Data Analytics, Business Insights & Applied AI**  
📧 [Your Email] | 🌐 [LinkedIn Profile] | 💻 [GitHub Profile]

---
