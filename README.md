# Power BI Business Dashboard – Sales & Operations Analytics

## 📌 Project Overview
This project focuses on building an interactive **Power BI dashboard** to monitor business performance, analyze sales trends, and support operational decision-making.  
The dashboard is designed from an **operations and management perspective**, enabling stakeholders to quickly understand key metrics and performance drivers.

---

## 🎯 Business Objective
To provide a centralized dashboard that helps:
- Track key sales and profitability KPIs
- Monitor sales trends over time
- Compare performance across regions and product categories
- Enable data-driven operational and strategic decisions

---

## 📊 Dataset
The analysis is based on retail transaction data split across multiple tables:

- **Orders** – Order-level transactional data (sales, profit, order date)
- **Customers** – Customer details
- **Location** – Geographic information (region, state, city)
- **Products** – Product attributes (category, sub-category)

The same dataset is used in **Project 1 (SQL Operational Analytics)** to demonstrate an end-to-end analytics workflow.

---

## 🧹 Data Preparation & Cleaning
- Cleaned and validated data using **Power Query**
- Handled inconsistent date formats by creating a cleaned date column
- Removed invalid or null values impacting analysis
- Created a **dedicated Date Dimension** to support time-based analysis

---

## 🧱 Data Modeling
A **star schema** data model was implemented for optimal performance and clarity:

- Fact table: `Orders`
- Dimension tables: `Customers`, `Location`, `Dim_Products`, `Dim_Date`

Key modeling decisions:
- Created a separate **Product Dimension** to handle duplicate product IDs
- Established **Many-to-One** relationships from fact to dimensions
- Marked `Dim_Date` as a **Date Table** to enable time intelligence

---

## 📐 KPIs & DAX Measures
The following key metrics were created using DAX:

- **Total Revenue**
- **Total Orders**
- **Average Order Value (AOV)**
- **Total Profit**

These KPIs provide a high-level performance snapshot for stakeholders.

---

## 📈 Dashboard Visuals
The dashboard includes:

- **KPI Cards** – Executive summary of key metrics
- **Monthly Sales Trend** – Time-based revenue analysis
- **Sales by Region** – Regional performance comparison
- **Sales by Category** – Product mix contribution
- **Interactive Filters (Slicers)** – Region, Category, and Year

All visuals are designed to be clean, intuitive, and stakeholder-friendly.

---

## 🕒 Time Intelligence & Sorting
- Implemented a `Year-Month` column for trend analysis
- Used a numeric sort column to ensure correct chronological ordering
- Enabled consistent monthly and yearly trend evaluation

---

## 🛠 Tools Used
- **Power BI Desktop**
- **DAX**
- **Power Query**
- **Star Schema Data Modeling**


---

## 📁 Repository Structure

```
powerbi-business-dashboard/
│
├── data/
│ ├── Orders.csv
│ ├── Customers.csv
│ ├── Location.csv
│ └── Products.csv
│
├── dashboard/
│ ├── sales_dashboard.png
│ └── sales_dashboard.pbix
│
└── README.md
```

---

## 💡 Business Value
This dashboard enables:
- Faster performance monitoring
- Identification of regional and category-level trends
- Improved operational planning
- Clear communication of insights to non-technical stakeholders

---

## 👤 Author
**Pritesh Patil**  
Data Analyst | SQL | Power BI | Tableau | Operational Analytics


