# 🏥 HealthStat Solutions: Healthcare Analytics Platform (ClinicalOps360)

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)](https://github.com/ajaya-kumar-pradhan)
[![DAX](https://img.shields.io/badge/DAX-Star%20Schema-blue?style=for-the-badge)](https://github.com/ajaya-kumar-pradhan)

---

## 📌 Project Overview

**HealthStat Solutions (ClinicalOps360)** is a **multi-layer healthcare analytics platform** built using Power BI, designed to simulate real-world hospital decision-making systems.

It integrates **financial, operational, and clinical datasets** into a unified analytics solution, enabling stakeholders to move seamlessly from **executive-level KPIs to detailed doctor and patient-level insights**.

---

## 🎯 Business Objectives

| Pillar | Goal |
|---|---|
| **Operational Excellence** | Optimize bed occupancy, wait time, and discharge delays |
| **Financial Intelligence** | Monitor revenue (~$10M+), billing trends, and profitability |
| **Clinical Quality** | Improve treatment success rate, reduce readmissions, enhance patient satisfaction |

---

## 🧩 Dashboard Architecture

```
Executive Overview
       ↓
Financial Analytics
       ↓
Operational Insights
       ↓
Clinical Performance
       ↓
Doctor-Level Drill
       ↓
Patient-Level Drill
```

---

## 🏗️ Data Architecture (Star Schema)

```
                       dim_date
                          |
dim_patients — fact_encounters — dim_doctors
                          |
                   dim_departments
```

### Fact Table
```
fact_encounters (
    encounter_id, patient_id, doctor_id, department_id, date_id,
    revenue, cost, length_of_stay, readmission_flag, satisfaction_score
)
```

### Dimension Tables
```
dim_patients    (patient_id, age, gender, risk_segment)
dim_doctors     (doctor_id, doctor_name, specialization)
dim_departments (department_id, department_name)
dim_date        (date_id, full_date, month, year)
```

---

## 📊 Core KPIs (DAX)

```dax
Total Revenue = SUM('fact_encounters'[revenue])

Total Encounters = COUNTROWS('fact_encounters')

Avg Length of Stay =
AVERAGE('fact_encounters'[length_of_stay])

Readmission Rate =
DIVIDE(
    CALCULATE(
        COUNTROWS('fact_encounters'),
        'fact_encounters'[readmission_flag] = 1
    ),
    COUNTROWS('fact_encounters')
)

Patient Satisfaction =
AVERAGE('fact_encounters'[satisfaction_score])

Bed Occupancy Rate =
DIVIDE([Occupied Beds], [Total Beds])

YoY Revenue Growth =
VAR PrevYear =
    CALCULATE(
        [Total Revenue],
        SAMEPERIODLASTYEAR('dim_date'[full_date])
    )
RETURN
    DIVIDE([Total Revenue] - PrevYear, PrevYear)

MoM Revenue Growth =
VAR PrevMonth =
    CALCULATE(
        [Total Revenue],
        DATEADD('dim_date'[full_date], -1, MONTH)
    )
RETURN
    DIVIDE([Total Revenue] - PrevMonth, PrevMonth)
```

---

## 🧠 Analytical Capabilities

- ✅ Executive KPI Tracking (Revenue, Encounters, Growth, Satisfaction)
- ✅ Clinical Analysis (Treatment Success vs Severity)
- ✅ Operational Metrics (Wait Time, LOS, Discharge Delays)
- ✅ Patient Risk Segmentation (Low / Moderate / High / Critical)
- ✅ Doctor Performance Benchmarking
- ✅ Diagnosis-Level Outcome Analysis
- ✅ Trend Analysis (MoM, YoY)

---

## 🔍 Drill-Through Functionality

Navigate from **Overview → Hospital → Doctor → Patient**

Deep-dive into:
- Individual doctor performance
- Patient-level clinical details
- Diagnosis-specific outcomes

---

## ⚙️ Tech Stack

| Layer | Tool |
|---|---|
| BI Tool | Power BI Desktop |
| Data Source | SQL Server |
| Modeling | DAX, Star Schema |
| Deployment | Power BI Service |

---

## 🚀 Advanced Features

- Interactive multi-page dashboards
- Drill-through navigation across hierarchy levels
- Optimized fact-dimension data model
- 40+ DAX measures for analytics
- Real-world healthcare simulation

---

## 📈 Key Insights Generated

- Identified high readmission patient segments
- Detected operational bottlenecks in discharge process
- Highlighted high-cost vs low-profit hospital units
- Improved patient risk visibility across departments
- Enabled performance comparison across doctors

---

## 🖼️ Dashboard Preview

![Executive Overview](images/overview.png)
![Financial Analytics](images/finance.png)
![Operational Insights](images/operations.png)
![Patient Analytics](images/patients.png)
![Clinical Performance](images/clinical.png)

---

## 🔗 Live Dashboard

👉 [View Live Power BI Report](https://app.powerbi.com/view?r=eyJrIjoiM2FkOGQ5OWYtNzgyMC00MDM1LTk4ZmUtMzA5NGFhYjk1OTk3IiwidCI6IjdlMzEwODQ1LTg0ZTEtNGRiOC1hZjk4LTcwNDA0MTkwZDhkZSJ9&pageName=ce2f74c292644e048628)

---

## 📂 Project Structure

```
Healthcare-Analytics-Dashboard/
│── data/
│── images/
│── dashboards/
│── README.md
```

---

## 🤝 Contact

**Ajaya Kumar Pradhan**
Data Analyst | Power BI Developer

📧 [ajayapradhan.connect@gmail.com](mailto:ajayapradhan.connect@gmail.com)
🔗 [linkedin.com/in/ajayakumarpradhan](https://www.linkedin.com/in/ajayakumarpradhan/)
💻 [github.com/ajaya-kumar-pradhan](https://github.com/ajaya-kumar-pradhan)
