# Medallion Data Engineering Pipeline for AI Model Training

> End-to-end Data Engineering project built with **PySpark** following the **Medallion Architecture (Bronze, Silver and Gold)** to process more than **12 million records** and prepare a high-quality dataset for training a Deep Learning model capable of predicting gender from personal names.

---

## 📌 Project Overview

This project demonstrates how a modern **Data Engineering pipeline** can be designed using the **Medallion Architecture** to transform raw data into reliable, production-ready datasets for Machine Learning.

The pipeline processes a dataset containing more than **12 million records** of names, countries and gender labels. Using **PySpark**, the data is ingested, validated, standardized and transformed into optimized Parquet datasets before being used to train a neural network built with **TensorFlow/Keras**.

Although the final objective is gender prediction, the primary focus of the project is demonstrating **Data Engineering best practices**, including scalable data processing, modular pipeline design, data quality validation and reproducible workflows.

---

## 🎯 Objectives

- Design an end-to-end Data Engineering pipeline.
- Implement the Medallion Architecture (Bronze, Silver and Gold).
- Process large datasets efficiently using Apache Spark.
- Apply data quality validations and standardization.
- Convert raw CSV files into optimized Parquet datasets.
- Prepare production-ready datasets for Deep Learning.
- Build a reproducible and modular project following Data Engineering best practices.

---

## 🏗️ Architecture

The project follows the **Medallion Architecture**.

```
                    Raw Dataset
                        │
                        ▼
                ┌─────────────────┐
                │     BRONZE      │
                │ Data Ingestion  │
                │ CSV → Parquet   │
                └─────────────────┘
                        │
                        ▼
                ┌─────────────────┐
                │     SILVER      │
                │ Data Cleaning   │
                │ Standardization │
                │ Data Validation │
                └─────────────────┘
                        │
                        ▼
                ┌─────────────────┐
                │      GOLD       │
                │ Feature Dataset │
                │ Train / Valid   │
                │ Test Split      │
                └─────────────────┘
                        │
                        ▼
              TensorFlow / Keras Model
```

---

## 📂 Project Structure

```text
medallion-name-gender-pipeline/

├── data/
│   ├── raw/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── notebooks/
│
├── models/
├── README.md
└── requirements.txt
```

---

## ⚙️ Pipeline Stages

### 🟤 Bronze

- Read raw CSV files.
- Validate schema.
- Initial data profiling.
- Convert data to Parquet.
- Preserve raw information.

---

### ⚪ Silver

- Remove invalid records.
- Remove duplicates.
- Standardize names.
- Normalize country information.
- Standardize gender labels.
- Filter Latin American records.
- Apply data quality validations.

---

### 🟡 Gold

- Feature preparation.
- Label encoding.
- Dataset generation.
- Train / Validation / Test split.
- Final datasets ready for Machine Learning.

---

## 🛠️ Technologies

- Python
- PySpark
- Apache Spark
- Parquet
- TensorFlow
- Keras
- Jupyter Notebook
- Git
- GitHub

---

## 🚀 Current Status

Completed:

- ✅ Project architecture
- ✅ Medallion pipeline design
- ✅ Bronze layer
- ✅ Initial data profiling
- ✅ Silver layer
- ✅ Data quality framework
- ✅ Gold dataset generation
- ✅ Deep Learning model
- ✅ Model evaluation

---

## 💡 Key Learning Goals

This project focuses on demonstrating practical skills in:

- Data Engineering
- Big Data Processing
- PySpark
- Medallion Architecture
- Data Quality
- Data Pipeline Design
- Machine Learning Data Preparation
- Software Engineering Best Practices

---

## 📬 Contact

**Hugo Cabrera**

- LinkedIn: https://www.linkedin.com/in/hugo-cabrera-324272191/
- GitHub: https://github.com/CabHug

---

> **Note:** This repository is intended as a portfolio project to demonstrate Data Engineering and Machine Learning engineering practices using modern data processing technologies.