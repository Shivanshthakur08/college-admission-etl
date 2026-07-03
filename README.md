# 🎓 College Admission Analytics ETL Pipeline

A production-ready ETL pipeline that extracts, validates, cleans, transforms, and loads multi-branch college admission data into a Star Schema Data Warehouse for Business Intelligence and reporting.

---

## 📖 Overview

This project automates the complete ETL workflow for a College Admission Analytics System using the **Bronze → Silver → Gold** architecture. It ensures data quality, masks sensitive information, and prepares analytics-ready datasets for Power BI dashboards.

---

## 🚀 Features

- Extract data from 10 CSV source files
- Load raw data into MariaDB staging tables
- Perform data validation and quality checks
- Mask Personally Identifiable Information (PII)
- Clean and standardize data
- Build a Star Schema Data Warehouse
- Generate Power BI-ready datasets
- Automated ETL orchestration with Apache Airflow

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | ETL Development |
| Pandas | Data Processing |
| MariaDB | Database |
| SQLAlchemy & PyMySQL | Database Connectivity |
| SQL | Data Transformation |
| Apache Airflow | Workflow Orchestration |
| Great Expectations | Data Quality |
| Power BI | Data Visualization |
| Git & GitHub | Version Control |

---

## 📂 Project Structure

```text
college-admission-etl/
│
├── extract/
├── staging/
├── transform/
├── warehouse/
├── data_quality/
├── orchestration/
├── config/
├── logs/
├── docs/
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## 🔄 ETL Workflow

```text
CSV Files
    │
    ▼
Extraction
    │
    ▼
Bronze (Staging)
    │
    ▼
Data Validation & PII Masking
    │
    ▼
Silver (Cleaned Data)
    │
    ▼
Gold (Star Schema)
    │
    ▼
Power BI Dashboard
```

---

## 📊 Data Warehouse

### Dimension Tables
- dim_student
- dim_campus
- dim_course
- dim_counselor
- dim_campaign
- dim_date

### Fact Tables
- fact_enquiries
- fact_applications
- fact_admissions
- fact_fee_payments

---

## ▶️ Getting Started

### Clone Repository

```bash
git clone https://github.com/nikitaRPS/college-admission-etl.git
cd college-admission-etl
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment

Create a `.env` file from `.env.example` and update your database credentials.

### Run ETL

```bash
python extract/load_staging.py
python data_quality/run_dq_checks.py
python transform/run_transforms.py
```

---

## 🔒 Data Quality & Security

- Schema Validation
- Duplicate Detection
- Null Value Handling
- Date & Data Standardization
- Range Validation
- PII Masking (Name, Email, Phone, Transaction ID)

---

## 📈 Output

- Cleaned & Validated Data
- Star Schema Warehouse
- Data Quality Reports
- Power BI Ready Dataset

---

## 👨‍💻 Author

Nikita Patel - Team Leader
Shivansh Thakur - Member 1
Umang Thakur - Member 2
Rishit Agrawal - Member 3

*Data Analyst | SQL | Python | Power BI | ETL*
