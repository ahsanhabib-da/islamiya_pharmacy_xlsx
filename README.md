# 💊 Healthcare Supply Chain Analytics: Islamia Pharmacy Optimization
A data engineering and logistics project transforming fragmented, manual pharmacy operations into an automated, relational database architecture using Microsoft Excel.

## 📌 Project Overview
Small-scale pharmacies often suffer from manual stock tracking, leading to critical stockouts or expired capital. This project establishes a scalable data pipeline for **Islamia Pharmacy**, tracking 137+ active pharmaceutical products to automate stock level tracking, sales analysis, and supply chain oversight.

---

## 📊 Database Architecture (3-Sheet Relational Model)
Instead of a single flat file, this system utilizes a relational model broken into three distinct operational data layers:

1. **`Medicine Master Table`**: The single source of truth containing universal product profiles, including unique Medicine IDs, Generic Names, Dosage Forms, and Indications.
2. **`Sales Log Table`**: A dynamic transactional ledger capturing day-to-day customer invoices, item quantities sold, transaction dates, and revenue metrics.
3. **`Stock In`**: An operational supply ledger recording incoming distributor shipments, unit costs, batches, and delivery logs.

### Key Data Engineering Actions Implemented:
* **Data Cleaning & Standardization**: Extracted and normalized structural errors from messy manual inputs, ensuring clean strings for generic components and structural alignment across dosage forms.
* **Relational Integrity**: Built pseudo-primary keys (`Medicine ID`) to cleanly link transactional sales and inventory receipts back to the master table using index-matching principles.
* **Operational Automation**: Integrated logical functions to dynamically calculate current stock balances, flag low-stock thresholds, and automatically trigger reorder signals.

---

## 🚀 Future Roadmap
* **Scale Volume**: Expand the core data model from 137 rows to thousands of global pharmaceutical stock-keeping units (SKUs).
* **Advanced Metrics**: Embed ABC inventory classification ($A$ = high value, $C$ = high turnover) to optimize working capital.
* **BI Dashboard**: Connect this clean Excel data engine directly to Power BI/Tableau for automated executive supply chain dashboards.
