# 🧠 Financial Transactions Fraud Detection – Data Analysis & Visualization

This project focuses on detecting and analyzing financial fraud patterns using transactional data. The objective is to identify the top fraud types, estimate financial losses, and visualize patterns that can guide future risk reduction strategies.

---

## 📌 Project Scope

The project is designed to support a real-world fraud detection system by performing:

- Comprehensive data preprocessing and feature cleaning  
- Fraud type inference based on business rules and transactional behavior  
- Exploratory data visualization to understand key fraud categories and their financial impact  
- Loss estimation and reduction target analysis to define actionable business goals  

---

## 🎯 Key Objectives

### 1. Identify Top 3–5 Fraud Types  
Detect and categorize transactions into key fraud types like:
- Account Takeover  
- Synthetic ID  
- Transaction Collusion  
- Money Laundering  
- Other/Unclassified Fraud  

### 2. Estimate Fraud Losses and Targets  
- Calculate total financial losses from inferred fraud transactions  
- Define target reduction goals (40–50%) for business impact analysis  

### 3. Visualize Fraud Insights  
Create multiple visual analytics reports to summarize fraud trends:
- **Horizontal Bar Chart** → Top Fraud Types by Count  
- **Pie Chart** → Fraud Distribution (%)  
- **Vertical Bar Chart** → Total Financial Losses by Fraud Type  
- **Heatmap** → Combined Summary (Counts and Losses)  

---

## 🧩 Data Integration & Preprocessing

The project merges and cleans multiple datasets to build a unified fraud analysis dataset.

**Data Sources Integrated:**
- User Profiles  
- Transactions  
- Real-Time Behavioral Features  
- ML Model Logs  
- Merchant Risk Data  
- External Data Feeds  
- Block Lists  
- Alert Cases  
- Aggregated Time Series Data  
- Account Status Changes  

The final merged dataset (`final_new.csv`) includes key features like:
- UserID, TransactionID  
- Transaction Amount & Timestamp  
- KYC Level and Current Risk Score  
- Velocity Score, Foreign Transaction Count  
- IP Risk Score and VPN Flag  
- Fraud Case Status and Resolution Code  
- Account Status Change History  

---

## 🧠 Data Processing & Feature Engineering

- Loaded and cleaned dataset from `final_new.csv`  
- Converted date fields (`Account_Open_Date`, `Transaction_Timestamp`)  
- Normalized risk scores and mapped KYC levels numerically  
- Converted boolean and numeric feature columns for analysis  
- Applied rule-based inference to classify transactions into probable fraud types using:  
  - Velocity  
  - IP Risk  
  - KYC Level  
  - Account Age  
  - Foreign Transactions  
  - Behavioral Patterns  

---

## 📊 Visualizations Generated

| Visualization | Description | Output File |
|----------------|-------------|--------------|
| **Top Fraud Types Bar Chart** | Shows fraud types ranked by frequency | `top_fraud_types_bar.png` |
| **Fraud Distribution Pie Chart** | Visualizes percentage distribution | `fraud_types_pie.png` |
| **Losses by Fraud Type Bar Chart** | Displays total monetary losses per fraud type | `losses_per_fraud_type_bar.png` |
| **Fraud Summary Heatmap** | Combines fraud count and loss metrics | `fraud_summary_heatmap.png` |

All plots are automatically saved as `.png` files for reporting and dashboard use.

---

## 📁 Files Generated

| File Name | Description |
|------------|-------------|
| `final_new.csv` | Unified and cleaned dataset |
| `fraud_types_summary.csv` | Summary of inferred fraud types and counts |
| `top_fraud_types_bar.png` | Bar chart visualization of top fraud types |
| `fraud_types_pie.png` | Pie chart of fraud distribution |
| `losses_per_fraud_type_bar.png` | Bar chart showing total losses per fraud type |
| `fraud_summary_heatmap.png` | Combined summary heatmap of fraud counts and losses |

---

## ⚙️ Tech Stack

- **Python 3.x**  
- **Pandas, NumPy** → Data Cleaning & Analysis  
- **Matplotlib, Seaborn** → Visualization  
- **Collections, Datetime** → Fraud inference logic  

---

## 🧾 Summary Output Example

**Top 5 Fraud Types (based on inferred signals in full dataset):**
- Account Takeover: 250 cases (32.1%)  
- Synthetic ID: 180 cases (23.1%)  
- Transaction Collusion: 140 cases (18.0%)  
- Money Laundering: 95 cases (12.3%)  
- Other Fraud: 45 cases (5.8%)  

**Current Estimated Fraud Losses:** $4,250,000.00  
**Target Reduction Rate:** 40–50%  
**Target Fraud Losses:** $2,550,000.00 – $2,125,000.00  

---

## 🌟 Project Impact

This project helps financial institutions:
- Improve fraud detection accuracy  
- Quantify and reduce monetary losses  
- Identify high-risk behaviors early  
- Generate actionable intelligence for compliance teams  

---

If you find this project useful, please **⭐ star the repository** on GitHub!  
Your support motivates further work on real-world data intelligence systems.
