# 🛍️ Customer Purchase Behavior Analysis & Segmentation

## 📌 Project Overview
This project analyzes retail customer purchase data to:
- Identify **top-performing customer segments**
- Detect **purchasing patterns and trends** over time
- Provide **business recommendations** to improve sales & marketing strategies

The work combines **SQL + Python (Pandas) + Google Sheets + Power BI** into an end-to-end analytics pipeline.

---
Customer-Purchase-Behavior-Analysis/

│
├── data/

│   ├── Customer_Segmentation.csv

│   ├── Monthly_Trends.csv

│   ├── Segment_Counts.csv

│   ├── Segment_Revenue.csv

│   ├── Segment_Summary.csv

│   ├── Pareto_Summary.csv


│   ├── Customer_Month_Segment.csv

│
├── notebooks/

│   ├── customer_segmentation.ipynb   

│
├── dashboard/

│   ├── powerbi_dashboard.pbix        

│   ├── dashboard_screenshot.png     

│
├── README.md


## 📂 Dataset
- Source: [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- Transactions from a UK-based online retailer (2010–2011)
- Key fields: `InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country`

---

## 🛠️ Tools & Skills
- **Python (Pandas, SQLite)** → Data cleaning, segmentation, monthly trend analysis
- **SQL (SQLite in Colab)** → Customer aggregation, revenue calculation, Pareto analysis
- **Google Sheets** → Pivot tables for quick summaries
- **Power BI** → Interactive dashboards with segmentation & revenue insights

---

## 🔍 Methodology
1. **Data Cleaning (Python)**  
   - Removed missing `CustomerID` values  
   - Dropped cancelled invoices  
   - Created `Revenue = Quantity × UnitPrice`  

2. **Segmentation**  
   - Customers segmented into:
     - **High Value** → Top 10% by revenue  
     - **Frequent Low Spenders** → Top 25% by frequency  
     - **Other** → Remaining customers  

3. **SQL Analysis**  
   - Monthly revenue & customer counts  
   - Revenue per customer & segment  
   - Pareto analysis: Top 10% customers’ contribution  

4. **Visualization**  
   - Google Sheets pivot tables  
   - Power BI dashboard (interactive, with slicers & maps)

---

## 📊 Key Outputs

### 📈 Segment Summary
| Segment              | CustomerCount | TotalRevenue | RevenueShare (%) |
|----------------------|---------------|--------------|------------------|
| High Value           | 434           | 5.47M        | 61.38%           |
| Frequent Low Spender | 730           | 1.45M        | 16.25%           |
| Other                | 3175          | 1.99M        | 22.38%           |

### 📉 Pareto Analysis
| Metric                   | Value   |
|---------------------------|---------|
| Total Customers           | 4339    |
| Top 10% Customers         | 434     |
| Total Revenue             | 8.91M   |
| Top 10% Revenue           | 5.47M   |
| Top 10% Revenue Share (%) | 61.38%  |

### 📅 Monthly Trends (Sample)
| Month   | MonthlyRevenue | UniqueCustomers |
|---------|----------------|-----------------|
| 2010-12 | 572,713        | 885             |
| 2011-01 | 569,445        | 741             |
| 2011-02 | 447,137        | 758             |
| …       | …              | …               |

---

## 📊 Power BI Dashboard

Key visuals included:
- **Customer Distribution Pie Chart** (segment-wise counts)  
- **Revenue by Segment (Bar Chart)**  
- **Revenue Share (%) Donut Chart**  
- **Monthly Revenue Trend (Line Chart with Segment Slicer)**  
- **Customer Segmentation by Country (Map)**  
- **KPI Cards** → Total Revenue, Total Customers, Avg Revenue/Customer  

📸 Example screenshot:  

![Dashboard Screenshot](dashboard/dashboard_screenshot.png)

---

## 💡 Insights & Recommendations
- **Top 10% of customers generate ~61% of total revenue** → loyalty programs & personalized offers can maximize retention.  
- **Frequent low spenders (16% revenue)** → upselling and bundle strategies could increase revenue.  
- **Monthly trends** show seasonal spikes in **Nov–Dec** → targeted campaigns during festive periods are effective.  
- **Geographic analysis** → strong customer base in the UK; explore expansion in EU markets.

---

## 🚀 Outcome
This project demonstrates:
- Practical integration of **SQL, Python, Google Sheets, Power BI**  
- End-to-end **customer behavior analysis pipeline**  
- Strong **business insights** from data-driven methods  

---

## 📌 How to Use
1. Clone the repository  
   ```bash
   git clone https://github.com/AfsarJahan/Customer-Purchase-Behavior-Analysis.git
