# 🚚 Automated Supply Chain Analytics Engine & Executive BI Pipeline

An end-to-end data engineering and business intelligence (BI) pipeline that extracts transactional supply chain data from a relational **PostgreSQL** database, processes critical warehouse/logistical KPIs using optimized type-casted SQL queries, and programmatically compiles a highly styled, executive-ready multi-sheet report using Python.

---

## 🛠️ System Architecture & Data Flow

1. **Extraction:** Establishes a secure database link via `SQLAlchemy`, handling special-character credential encoding safely.
2. **Transformation:** Rewrites legacy textual date-logs into true timestamps directly in the PostgreSQL engine to run historical operational drift formulas.
3. **Analytics Engine:** Merges disconnected datasets to evaluate vendor speed, stock replacement frequencies, and quality control metrics under a customized multi-weighted scoring algorithm.
4. **Automation & Delivery:** Programmatically designs a multi-tab corporate workbook complete with functional visual graphs, structured cell dimensions, and data-driven heatmapping.

---

## 📊 Core Business KPIs Tracked

The engine automates the tracking of four high-level operational performance metrics:

* **On-Time Delivery (OTD) Rate (%):** Calculates the precise percentage of line-item deliveries arriving on or before deadlines, alongside tracking average operational delays.
* **Inventory Turnover Ratio:** Divides the global **Cost of Goods Sold (COGS)** by the **Average Inventory Value** per vendor to track warehouse asset velocity.
* **Supplier Damage Rate (%):** Evaluates transit cargo quality issues by mapping total damaged items against initial quantity requisitions.
* **Supplier Performance Scorecard:** A proprietary metric assigning an algorithmic performance letter grade (**A, B, C, or D**) calculated via a multi-weighted formula:

$$\text{Performance Score} = (50\% \times \text{OTD}) + (30\% \times \text{Quality}) + (20\% \times \text{Turnover Velocity})$$

---

## 📂 Repository Structure

```text
├── Supply_Chain_Performance_Report.xlsx  # Final auto-generated styled corporate spreadsheet
├── supply_chain_pipeline.ipynb          # Core interactive Jupyter notebook with pipeline execution
├── README.md                             # Project documentation
