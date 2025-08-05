# 🧪 Adventure Works Data Transformation – Silver Layer (Databricks + Azure)

This repository contains a Databricks notebook focused on **data transformation** of the Adventure Works dataset, specifically targeting the **Silver Layer** in a modern data lakehouse architecture using **Azure Data Lake Storage (ADLS)** and **PySpark**.

---

## 📌 Objective

Transform raw Adventure Works CSV data (from Bronze Layer) into clean, optimized Parquet format stored in the **Silver Layer**, ready for downstream analytics and machine learning tasks.

---

## 🔧 Technologies Used

- **Azure Data Lake Storage (ADLS Gen2)**
- **Databricks (PySpark Notebooks)**
- **Parquet File Format**
- **OAuth Authentication (Service Principal)**

---

## 📂 Project Structure

.
├── Transformation in Silver Layer.ipynb # Main Databricks notebook
├── data/
│ ├── bronze/ # Raw CSVs (source)
│ └── silver/ # Transformed Parquet files (target)
├── README.md # You're here!


---

## 🚀 Key Features

- Secure connection to **Azure Data Lake** using **OAuth-based Service Principal**
- Type-safe ingestion of CSV data
- Null value handling and schema standardization
- Application of PySpark transformations such as:
  - Data type casting
  - Column renaming
  - Filtering and deduplication
- Output saved in efficient, compressed **Parquet format** for optimized querying

---

## ⚙️ How to Run

### ✅ Prerequisites
- Databricks Workspace
- Access to Azure Data Lake (Bronze and Silver containers)
- Adventure Works CSV files in Bronze Layer

### ▶ Steps

1. **Open the notebook** in Databricks:  
   `Transformation in Silver Layer.ipynb`

2. **Configure Azure ADLS credentials** (Service Principal) in the notebook

3. **Run all cells** to:
   - Mount or access ADLS containers
   - Load CSV data
   - Apply transformations
   - Save cleaned data to Silver layer

---

## 📈 Outcome

- ✅ Cleaned, transformed dataset in **Parquet format**
- ✅ Data ready for analytics, reporting, or ML use cases

---

## 🔒 Security Note

> ⚠️ **Do NOT upload notebooks with exposed secrets or credentials.**  
> Replace client secrets with environment variables or secret scopes in production.


