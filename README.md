# Analytics Engineering Fundamentals — StroopwafelShop Project

⚡ **Note:** All work shown here is **personal / academic learning**.
It reflects my independent learning and upskilling as I transition into **Analytics Engineering**.

---

## 📘 Program Overview
In **September 2025**, I completed the book *Fundamentals of Analytics Engineering* by Joe Reis & Matt Housley.  
Alongside reading, I implemented the **Chapter 8 StroopwafelShop case study** hands-on with **dbt Cloud + BigQuery** to practice real-world analytics engineering workflows.  

This repo documents both my learning and implementation.  

---

## 🛠️ Tech Stack
- **Ingestion:** Airbyte (Google Sheets → BigQuery)  
- **Transformation:** dbt Cloud (staging → intermediate → marts)  
- **Warehouse:** Google BigQuery  
- **Analytics:** Tableau dashboards for BI  

---

## 📂 Repo Structure
- `dbt_stroopwafelshop/` → dbt project (models: staging, intermediate, marts)  
- `data/` → sample data provided in the book 
- `README.md` → this file  

---

## 🔹 StroopwafelShop Case Study
**Business Problem:** StroopwafelShop needs reliable reporting across sales, employees, products, and promotions. Raw data is fragmented and unmodeled, making BI reporting unreliable.  

**My Implementation:**  
- Modeled raw data into **staging tables** (`stg_sales`, `stg_employees`, `stg_products`, `stg_shifts`, `stg_promotions`)  
- Built **intermediate models** to join, clean, and prepare metrics  
- Designed a **star schema marts layer**:  
  - `fct_sales` (fact table)  
  - `dim_employees`, `dim_products`, `dim_promotions`, `dim_shifts` (dimension tables)  
- Validated transformations in **BigQuery**  
- Connected marts layer to **Tableau** to create reporting dashboards  

---

## 🚀 Skills Demonstrated
- **Analytics Engineering Principles** (staging → marts, modular SQL, testing)  
- **dbt Cloud** (models, lineage graphs, documentation)  
- **BigQuery SQL** (warehouse optimization, joins, transformations)  
- **Airbyte** ingestion pipelines  
- **Tableau** BI dashboards  
- **Version Control & Documentation** for reproducible workflows  

---

## 📌 Next Steps
- Expand dbt models with **tests & documentation**  
- Explore **CI/CD pipelines** for dbt (dbt Cloud jobs, GitHub Actions)  
- Apply Analytics Engineering patterns (dbt + warehouse + BI) to **real-world datasets**  

---
