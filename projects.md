---
layout: default
title: Projects
---

# 🛠 Projects

## 📊 WhatsApp Report Automation {#whatsapp-report}

A system that pulls data from Tableau and Grafana dashboards, converts them into image/PDF, and sends reports via WhatsApp using the WhatsApp Business API. Fully automated with custom scheduling and fallback retries.

**Stack:** Python, Tableau API, Grafana API, WhatsApp Business API, YAML scheduler

---

## 🧱 Data Pipeline: FTP → Parquet → MinIO → Trino → Singlestore {#data-pipeline}

A production data lake architecture:
- Ingests CSV/Excel from SFTP via Airflow
- Converts to Parquet
- Stores in MinIO (S3-compatible)
- Trino queries Iceberg tables for analytics
- Singlestore for real-time dashboards via pipelines

**Stack:** Airflow, Python, MinIO, Trino, Iceberg, Singlestore

---

## 🔎 Apache Drill for Schema-less Data Preview {#drill-tool}

Drill-based tool to explore CSV/Parquet files quickly without predefining schemas. Useful for debugging, data profiling, or checking headers on mounted SFTP and MinIO buckets.

**Stack:** Apache Drill, rclone, Python CLI

---
