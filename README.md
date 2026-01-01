# 🛒 E-Commerce ETL Pipeline (AWS + PySpark + OOP + Medallion Architecture)

This project is a complete **end-to-end data engineering ETL pipeline** for e-commerce analytics.  
It uses **AWS services**, **PySpark**, and **OOP design patterns**, and follows the **Medallion architecture**.

---

## 🚀 Architecture Overview

```
Source → S3 Bronze → S3 Silver → S3 Gold → Athena → QuickSight
```

### AWS Services Used
- S3 (data lake)
- Glue Jobs (PySpark ETL)
- Glue Catalog (schema)
- CloudWatch (logs)
- Athena (analytics)

---

## 🧱 Medallion Layers

### Bronze (Raw)
Stores raw CSV/JSON files.

### Silver (Cleaned)
- Standardized schema  
- Null-handling  
- Deduplication  

### Gold (Curated)
- Aggregated business insights  

---

## 📊 Outputs

Gold layer produces analytics tables:
- Daily Sales
- Customer Lifetime Value
- Category Revenue
- Repeat Customer Rate
- Top Products

---

## 🧩 Orchestration via AWS Step Functions

Included:
`orchestration/step_functions_definition.json`

---

## 📝 Author
Designed by Yogesh Jore
