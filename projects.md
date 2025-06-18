---
layout: default
title: Projects
---

# Projects

Below are a few highlights of the data engineering and automation work I've done.

---

## 🔗 WhatsApp Reporting via Tableau/Grafana

**Stack:** Go, Tableau REST API, Grafana Image Render API, Docker, WhatsApp Gateway  
**Description:**  
Built a Go-based backend to:
- Capture live snapshots from Tableau and Grafana (PNG, PDF)
- Schedule and send those images via WhatsApp using an API gateway
- Support on-demand requests and scheduled jobs

---

## 🏗️ FTP → Parquet → Iceberg → SingleStore

**Stack:** Apache Airflow, MinIO, Trino, Iceberg, SingleStore  
**Description:**  
Created a robust ETL pipeline:
```
FTP/SFTP → Airflow (convert to Parquet) → MinIO → 
  ├─> SingleStore via pipeline  
  └─> Trino (query hourly granularity) → Iceberg Table → SingleStore
```

---

## ⚙️ Apache Drill for Ad-Hoc File Inspection

**Stack:** Apache Drill, MinIO, SFTP  
**Description:**  
Used Apache Drill as an auxiliary tool to:
- Explore file structures without schema definition
- Query CSV/JSON/Parquet directly from SFTP and MinIO
- Validate file headers before loading
