# 📊 E-Commerce Data Engineering Project

## 🚀 Overview

In today’s e-commerce ecosystem, customer data is often fragmented across multiple platforms such as websites, mobile apps, customer support, and order management systems. This makes it challenging to understand the complete customer journey, identify high-value customers, and deliver personalized experiences.

This project builds a **Unified Customer 360 View** by integrating data from these disparate sources into a single, comprehensive profile.

In this project we are building a complete end-to-end **data engineering pipeline** built using Microsoft Fabric. The goal is to ingest, clean, transform, and analyze e-commerce data using a modern **Lakehouse architecture (Bronze → Silver → Gold)**.

The project showcases real-world data engineering practices including data cleaning, schema management, and building analytical datasets for reporting.

---

## 🧰 Tech Stack

* Microsoft Fabric (Lakehouse, Pipelines)
* PySpark
* Delta Lake
* Power BI
* SQL

---

## 🏗️ Architecture

The project follows the **Medallion Architecture**:

```
Raw Data → Bronze Layer → Silver Layer → Gold Layer → Power BI Dashboard
```

* **Bronze Layer**: Raw ingested data
* **Silver Layer**: Cleaned and transformed data
* **Gold Layer**: Aggregated data for analytics

---

## 🔄 Pipeline Workflow

### 1️⃣ Data Ingestion (Bronze)

* Raw data is ingested into the Lakehouse
* Stored without transformations

### 2️⃣ Data Cleaning (Silver)

* Trimmed whitespace
* Standardized text fields (name, email, location)
* Normalized categorical values (gender)
* Converted date formats
* Removed nulls and duplicates

### 3️⃣ Data Transformation (Gold)

* Aggregated datasets created for reporting
* Optimized for analytics queries

---

## 📂 Project Structure

```
ecommerce-data-engineering-project/
│
├── notebooks/              # PySpark notebooks
├── lakehouse/
│   ├── schema/             # Extracted schema
│   ├── sql/                # Table creation scripts
│
├── reports/                # Power BI dashboards
├── docs/                   # Architecture & documentation
├── scripts/                # Python/PySpark scripts
└── README.md
```

---

## 🧾 Data Cleaning Logic

Key transformations implemented:

* `initcap()` for proper casing
* `lower()` for email standardization
* `trim()` to remove whitespace
* `when()` for categorical normalization
* `to_date()` for date conversion
* `dropDuplicates()` to remove duplicate records
* `dropna()` to remove null values

---

## 📊 Schema Management

* Extracted full Lakehouse schema using PySpark
* Stored schema in `schema.txt`
* Ensured structured and consistent data storage

---

## 📈 Dashboard

A Power BI dashboard was created to visualize:

* Customer insights
* Transaction trends
* Business KPIs

(Screenshots available in `/reports/dashboard_screenshots`)

---

## 💡 Key Features

* End-to-end data pipeline
* Lakehouse architecture implementation
* Data quality handling
* Schema extraction and documentation
* Integration with Power BI for reporting

---

## 🧠 Learnings

* Hands-on experience with Microsoft Fabric
* Understanding of Medallion Architecture
* Data transformation using PySpark
* Managing structured data using Delta Lake
* Building analytics-ready datasets

---

## 🔮 Future Improvements

* Add real-time data ingestion
* Implement incremental data loading
* Automate pipeline scheduling
* Add data validation checks

---

## 👩‍💻 Author

**Shubhi Jain**
Aspiring Data Engineer

---


