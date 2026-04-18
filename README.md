# 🏥 HealthStats: Healthcare Analytics Dashboard (ClinicalOps360)
# 🏥 HealthStats: Healthcare Analytics Dashboard (HealthStats / ClinicalOps360)

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)](https://github.com/ajaya-kumar-pradhan)
[![Star Schema](https://img.shields.io/badge/Star%20Schema-Architecture-blue?style=for-the-badge)](https://github.com/ajaya-kumar-pradhan)

## 📌 Project Overview
**HealthStats (ClinicalOps360)** is an enterprise-grade Healthcare Analytics solution designed to provide hospital administrators and clinical leads with real-time insights into patient outcomes, operational efficiency, and financial performance. This project transforms raw clinical and billing data into a strategic decision-support system.

### 🎯 Key Objectives
- **Operational Excellence**: Monitor patient throughput, occupancy rates, and average length of stay (ALOS).
- **Financial Intelligence**: Track Average Daily Rate (ADR), Revenue per Available Room (RevPAR), and billing accuracy.
- **Clinical Quality**: Analyze patient outcomes and satisfaction scores to drive quality improvements.

---

## 🏗️ Data Architecture: Star Schema
The project implements a robust **Star Schema** to ensure high performance and precise filter propagation.

- **Fact Table**: `fact_encounters` (Granular patient-level visit data).
- **Dimension Tables**: 
  - `dim_patients`: Demographic intelligence.
  - `dim_departments`: Specialty-wise performance.
  - `dim_doctors`: Provider outcome tracking.
  - `dim_date`: Comprehensive time-intelligence (YTD, YoY, Moving Averages).

---

## 📊 Key DAX Measures & KPIs
Developed over 40+ custom DAX measures for deep-dive analytics:

- **Patient Throughput**: `Total Encounters = COUNTROWS('fact_encounters')`
- **Economic Value**: `RevPAR = DIVIDE([Total Revenue], [Total Available Room Nights])`
- **Clinical Efficiency**: `Occupancy Rate = DIVIDE([Occupied Room Nights], [Total Capacity])`
- **Financial Growth**: `YoY Revenue Growth = VAR PrevYear = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('dim_date'[Date])) RETURN DIVIDE([Total Revenue] - PrevYear, PrevYear)`

---

## 🛠️ Tech Stack
- **BI Tool**: Power BI Desktop
- **Data Engine**: SQL Server (ETL & Views)
- **Modeling**: DAX (Advanced Time Intelligence & RLS)
- **Deployment**: Power BI Service (Scheduled Refresh, RLS, Mobile Compatibility)

---

## 🚀 Key Features
- **Row-Level Security (RLS)**: Sensitive patient data is protected; department heads only see their respective specialty data.
- **Incremental Refresh**: Optimized for large datasets, ensuring only new encounter data is loaded.
- **Drill-Through Analytics**: Move from high-level hospital KPIs down to individual specialty or provider performance.
- **Automated Reporting**: Integrated with Power BI Service for daily automated data syncs.

---

## 🤝 Contact & Portfolio
- **Name**: Ajaya Kumar Pradhan
- **Role**: Power BI Developer | Data Analyst
- **LinkedIn**: [ajayakumarpradhan](https://www.linkedin.com/in/ajayakumarpradhan/)
- **Email**: [ajayapradhan.connect@gmail.com](mailto:ajayapradhan.connect@gmail.com)

---
> *"In God we trust; all others must bring data." — W. Edwards Deming*
