# 🏥 Medical Equipment and Pharma Sales Dashboard

**Author:** Ankita Nademwar  
**Project Duration:** 15 Oct 2025 – 31 Oct 2025  
**Tool Used:** Microsoft Power BI  
**Repository Purpose:** To visualize and analyze sales performance across medical equipment and pharmaceutical products.

---

## 📊 Project Overview

This Power BI dashboard provides a detailed analysis of sales data from the medical and pharmaceutical domain.  
It helps management monitor sales trends, product performance, and regional insights for data-driven decision-making.

---

## 🎯 Objectives

- To combine **medical equipment** and **pharma sales** data into a unified analysis view.  
- To track **key performance metrics** such as Total Sales, Units Sold, and Gross Margin %.  
- To identify **top-performing regions, products, and hospitals**.  
- To enable quick **deep-dives** into specific product or region details.

---

## 🧩 Data Details

| Source | Description |
|--------|--------------|
| `data/PROJECT 1 ZAALIMA DATASET.csv` | Raw sales dataset including product, region, customer, and financial fields |

**Main Columns Used:**
- `Date`
- `Region`
- `Hospital_Name`
- `Product_Category`
- `Manufacturer`
- `Total_Sales`
- `Discount`
- `Units_Sold`
- `Gross_Margin`

---

## 🧠 Data Model & Measures

### Key Measures Created in Power BI:
- **Total Sales:** `SUM(Sales[Sales Amount]) - SUM(Sales[Discount Amount])`
- **Total Units:** `SUM(Sales[Units Sold])`
- **Gross Margin %:** `(SUM(Sales[Gross Margin]) / SUM(Sales[Sales Amount]))`

### Simplified Data Model:
A single main fact table was used (`Sales Data`), with date fields derived using Power BI’s built-in date hierarchy.

---

## 🖥️ Dashboard Pages

1. **Overview Page:**  
   Displays total sales, total units, and gross margin trends. Includes key KPIs and visuals like sales by category, sales by region, and top manufacturers.

2. **Product Deep-Dive Page:**  
   Allows detailed exploration by product category, manufacturer, and year. Includes bar chart of sales by product and matrix by hospital.

3. **Region / Hospital Page:**  
   Focuses on regional performance. Includes sales by region, hospital sales table, and interactive map visual.

---

## 💡 Key Insights

- **Top-performing categories:** Medical devices contributed the highest revenue share.  
- **High-margin manufacturers:** Certain pharma brands consistently showed stronger gross margins.  
- **Regional focus:** Urban regions generated more consistent sales volume.  
- **Sales trend:** Seasonal peaks around Q2 indicate hospital procurement cycles.

---

## 🚀 Recommendations

- Focus marketing campaigns on **high-margin products**.  
- Strengthen partnerships with **top 3 hospitals by volume**.  
- Review discounting policy for low-margin pharma products.  
- Add predictive analytics in the next phase using Power BI forecasting tools.

---

## 🗂️ Folder Structure
Healthcare-Sales-Dashboard/
├── data/ # raw + cleaned CSVs
├── powerbi/ # Power BI .pbix file
├── docs/ # report and documentation
│ ├── summary_report.docx
│ └── screenshots/
├── ppt/ # storytelling presentation
├── .gitignore
└── README.md


