# 📊 Supply Chain & Inventory Analysis Dashboard (Power BI)

## 🚀 Project Overview

This project focuses on analyzing supply chain and inventory performance using Power BI. The goal is to monitor stock levels, identify risks such as stock-outs and overstocking, and support data-driven inventory decision-making.

The dashboard provides insights into warehouse performance, inventory health, reorder optimization, and product movement trends.

---

## 🎯 Business Problem

A manufacturing company manages inventory across multiple warehouses and faces the following challenges:

* Stock-outs causing delayed customer deliveries
* Overstocking leading to high holding costs
* Manual inventory decisions without analytical insights

This dashboard helps supply chain analysts monitor inventory and optimize decision-making using data visualization and analytics.

---

## 📌 Key Objectives

* Monitor stock levels across warehouses
* Identify low-stock and excess inventory products
* Optimize reorder decisions
* Improve inventory turnover
* Detect slow-moving products
* Analyze warehouse shortages

---

## 📈 Dashboard Features

### ✅ Inventory Monitoring

* Low stock identification (Below reorder point)
* Stock status classification (Low, Optimal, Excess)
* Inventory distribution analysis

### ✅ Supply Chain Insights

* Warehouse shortage analysis
* Shipping and delivery tracking
* Supplier performance analysis

### ✅ Performance KPIs

* Total Sales
* Total Orders
* Inventory Turnover Rate
* Average Delivery Time

---

## 📊 Key DAX Measures Used

```DAX
Total Sales = SUMX(Orders, Orders[Quantity] * Orders[UnitPrice])

Inventory Turnover =
DIVIDE([Total Quantity Sold], [Average Inventory])

Stock Status =
SWITCH(
TRUE(),
Inventory[StockLevel] < Inventory[ReorderLevel], "Low",
Inventory[StockLevel] <= Inventory[ReorderLevel] * 1.5, "Optimal",
"Excess"
)
```

---

## 🛠 Tools & Technologies

* Power BI
* DAX (Data Analysis Expressions)
* Data Modeling
* Data Visualization

---

## 📂 Dataset Structure

* Products
* Suppliers
* Inventory
* Orders
* Shipments

---

## 📷 Dashboard Preview

(Add screenshots of your Power BI dashboard here after uploading.)

---

## 💡 Business Insights

* Early identification of low-stock items prevents stock-outs.
* Detection of excess inventory reduces holding costs.
* Inventory turnover analysis improves supply chain efficiency.
* Slow-moving product detection helps optimize purchasing decisions.

---

## 👨‍💻 Author

Created as part of a Supply Chain & Inventory Analytics project using Power BI.

---
