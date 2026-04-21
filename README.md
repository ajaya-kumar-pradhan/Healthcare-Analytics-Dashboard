# 🏥 Healthstats — Healthcare Analytics Platform

<div align="center">

**Transforming raw hospital data into boardroom-ready decisions.**
*A full-stack Power BI analytics platform simulating real-world clinical, financial, and operational intelligence.*

<br>

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiM2FkOGQ5OWYtNzgyMC00MDM1LTk4ZmUtMzA5NGFhYjk1OTk3IiwidCI6IjdlMzEwODQ1LTg0ZTEtNGRiOC1hZjk4LTcwNDA0MTkwZDhkZSJ9&pageName=ce2f74c292644e048628)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)](https://github.com/ajaya-kumar-pradhan)
[![DAX](https://img.shields.io/badge/DAX-40%2B%20Measures-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://github.com/ajaya-kumar-pradhan)
[![Star Schema](https://img.shields.io/badge/Model-Star%20Schema-6C3483?style=for-the-badge)](https://github.com/ajaya-kumar-pradhan)

<br>

### 🚀 [View Live Power BI Dashboard →](https://app.powerbi.com/view?r=eyJrIjoiM2FkOGQ5OWYtNzgyMC00MDM1LTk4ZmUtMzA5NGFhYjk1OTk3IiwidCI6IjdlMzEwODQ1LTg0ZTEtNGRiOC1hZjk4LTcwNDA0MTkwZDhkZSJ9&pageName=ce2f74c292644e048628)

</div>

---

## 📌 Overview

**Healthstats** is a multi-layered healthcare analytics platform built for **HealthStat Solutions** — designed to mirror how enterprise hospitals actually make decisions.

The platform unifies **financial, clinical, and operational data** into a single Power BI solution. Stakeholders can drill from executive KPIs all the way down to individual doctor and patient performance — no spreadsheets, no silos, just fast, actionable insight.

> **The Business Problem:** Hospital leadership lacked a single source of truth across departments. Revenue was leaking, bed utilization was untracked, and patient risk wasn't visible until it was too late.
>
> **The Solution:** A 6-page interactive dashboard that surfaces the right metrics to the right audience — from CFO to clinician.

---

## 📊 Key Features

- 🔎 **Drill-through navigation** — Seamlessly explore from hospital-level → department → doctor → individual patient
- 💰 **Revenue intelligence** — Track $10M+ in billing with monthly trend analysis, insurance vs. out-of-pocket breakdowns, and diagnosis-level profitability
- 🛏️ **Operational efficiency monitoring** — Bed occupancy (82%), average discharge delay, wait time heatmaps, and length-of-stay distribution
- 🧬 **Clinical outcome tracking** — Treatment success rate (84.2%), readmission rate (0.12), and severity-adjusted performance benchmarking
- 👤 **Patient risk segmentation** — Auto-classify 1,000+ patients into Low / Moderate / High / Critical risk tiers
- 📅 **Time intelligence** — MoM and YoY revenue growth using advanced DAX time functions
- 📐 **40+ custom DAX measures** — Purpose-built KPIs covering every dimension of hospital performance

---

## 🛠️ Tech Stack

| Layer | Tool / Technology |
|---|---|
| **BI & Visualization** | Power BI Desktop + Power BI Service |
| **Data Modeling** | Star Schema (Fact + 4 Dimension Tables) |
| **Query & Calculation** | DAX (40+ measures), M Query |
| **Data Source** | SQL Server |
| **Deployment** | Power BI Service (Published Live) |

---

## 📈 Key Metrics & Impact

| Metric | Value |
|---|---|
| 💵 Total Revenue Tracked | **$10.06M+** |
| 🏥 Patient Encounters Analyzed | **1,000+** |
| 📋 DAX Measures Built | **40+** |
| ✅ Treatment Success Rate | **84.2%** |
| 🛏️ Bed Occupancy Rate | **82%** |
| 🔁 Readmission Rate | **0.12** |
| ⭐ Avg Patient Satisfaction | **4.91 / 5** |
| ⏱️ Avg Wait Time | **3.89 hrs** |
| 📊 Dashboard Pages | **6 Linked Views** |

> These metrics reflect a fully modeled, production-grade analytics environment — built to match the scale and complexity of real hospital data systems.

---

## 🧠 Insights & Business Value

**What the analysis revealed:**

- 🔴 **High-readmission segments** were concentrated in specific diagnosis categories — enabling targeted clinical intervention
- 💸 **Revenue concentration risk** identified: a small number of diagnosis types drove a disproportionate share of billing
- 🛏️ **Discharge delays** (avg 1 day) in certain departments were inflating length-of-stay and reducing bed turnover
- 👨‍⚕️ **Doctor performance** varied significantly by department — benchmarking revealed outliers in both satisfaction scores and encounter volume
- ⚠️ **20 Critical-risk patients** surfaced through segmentation, allowing proactive care escalation before adverse events

**Business value delivered:**
> Hospital administrators can identify cost leaks, track clinical KPIs, and benchmark department performance — all from a single dashboard — reducing the time to insight from days to seconds.

---

## 🖼️ Dashboard Preview

### 1️⃣ Executive Overview
*KPIs at a glance: Revenue, Encounters, Success Rate, Satisfaction | MoM & YTD Trends | Diagnosis Mix*

![Executive Overview](https://github.com/ajaya-kumar-pradhan/Healthcare-Analytics-Dashboard/blob/5bb7d8d38894822337e46ff1fc0917c1180d670a/overview.jpg)

---

### 2️⃣ Clinical Performance
*Treatment Success vs Severity | Doctor Performance Scatter | Diagnosis Outcome Table | Multi-KPI Toggle*

![Clinical Performance](https://github.com/ajaya-kumar-pradhan/Healthcare-Analytics-Dashboard/blob/a5f1f86cdf8d283a578009d0807855101d11876c/clinical_performance.jpg)

---

### 3️⃣ Operations
*Bed Occupancy | Discharge Delay Analysis | Wait Time Heatmap (Hospital × Diagnosis) | LOS Distribution*

![Operations Dashboard](https://github.com/ajaya-kumar-pradhan/Healthcare-Analytics-Dashboard/blob/31045d0b1d8a13ab1baf7c76f9f25cc08242e5e4/operations.jpg)

---

### 4️⃣ Finance
*Revenue by Hospital | Insurance vs Out-of-Pocket Split | Monthly Billing Trends | Diagnosis Revenue Concentration*

![Finance Dashboard](https://github.com/ajaya-kumar-pradhan/Healthcare-Analytics-Dashboard/blob/31045d0b1d8a13ab1baf7c76f9f25cc08242e5e4/finance.jpg)

*Finance — Revenue-Cost Matrix by Hospital × Bed Type (toggle view)*

![Finance — Bed Cost Matrix](images/finance_bed_cost.jpg)

---

### 5️⃣ Patient Analytics
*Demographics View | Risk Segmentation | Patient Leaderboard | Geographic Distribution | Clinical Profile Scatter*

| Demographics | Risk Segmentation |
|---|---|
| ![Patient Demographics](https://github.com/ajaya-kumar-pradhan/Healthcare-Analytics-Dashboard/blob/31045d0b1d8a13ab1baf7c76f9f25cc08242e5e4/patient_risk.jpg) | ![Patient Risk](images/patient_risk.jpg) |

| Patient Leaderboard | Clinical Profile |
|---|---|
| ![Patient Leaderboard](images/patient_leaderboard.jpg) | ![Patient Profile](images/patient_profile.jpg) |

---

## 🏗️ Data Architecture

**Star Schema Design:**

```
                       dim_date
                          │
dim_patients ── fact_encounters ── dim_doctors
                          │
                   dim_departments
```

```sql
-- Core Fact Table
fact_encounters (
    encounter_id, patient_id, doctor_id, department_id, date_id,
    revenue, cost, length_of_stay, readmission_flag, satisfaction_score
)

-- Supporting Dimensions
dim_patients    → patient_id, age, gender, risk_segment
dim_doctors     → doctor_id, doctor_name, specialization
dim_departments → department_id, department_name
dim_date        → date_id, full_date, month, quarter, year
```

---

## 💡 Sample DAX — Core Measures

```dax
-- Revenue Intelligence
Total Revenue = SUM('fact_encounters'[revenue])

YoY Revenue Growth =
VAR PrevYear = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('dim_date'[full_date]))
RETURN DIVIDE([Total Revenue] - PrevYear, PrevYear)

-- Clinical KPIs
Readmission Rate =
DIVIDE(
    CALCULATE(COUNTROWS('fact_encounters'), 'fact_encounters'[readmission_flag] = 1),
    COUNTROWS('fact_encounters')
)

Treatment Success Rate =
DIVIDE(
    CALCULATE(COUNTROWS('fact_encounters'), 'fact_encounters'[outcome] = "Success"),
    COUNTROWS('fact_encounters')
)

-- Operational Metrics
Bed Occupancy Rate = DIVIDE([Occupied Beds], [Total Beds])
Avg Length of Stay = AVERAGE('fact_encounters'[length_of_stay])
```

---

## 📂 Project Structure

```
ClinicalOps360/
│
├── 📁 data/                  # Source datasets (SQL exports / CSV)
│
├── 📁 images/                # Dashboard screenshots
│   ├── overview.jpg
│   ├── clinical_performance.jpg
│   ├── operations.jpg
│   ├── finance.jpg
│   ├── finance_bed_cost.jpg
│   ├── patient_demographics.jpg
│   ├── patient_leaderboard.jpg
│   ├── patient_risk.jpg
│   └── patient_profile.jpg
│
├── 📁 dashboards/            # Power BI .pbix file
│
└── 📄 README.md
```

---

## 👤 About Me

**Ajaya Kumar Pradhan** — Data Analyst | Power BI Developer

I specialize in turning complex datasets into clean, decision-ready analytics. My work focuses on building scalable data models, writing performance-optimized DAX, and designing dashboards that non-technical stakeholders actually use.

**Core Skills:** `Power BI` `DAX` `SQL Server` `Data Modeling` `Star Schema` `ETL` `KPI Design`

<br>

📧 [ajayapradhan.connect@gmail.com](mailto:ajayapradhan.connect@gmail.com)
🔗 [linkedin.com/in/ajayakumarpradhan](https://www.linkedin.com/in/ajayakumarpradhan/)
💻 [github.com/ajaya-kumar-pradhan](https://github.com/ajaya-kumar-pradhan)

---

<div align="center">

*If this project helped or inspired you, consider giving it a ⭐ — it helps others find it too.*

</div>
