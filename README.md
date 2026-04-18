<!-- =========================
     HERO / HEADER SECTION
========================== -->

<p align="center">
  <!-- Replace with your banner image path -->
  <img src="assets/banner.png" alt="Healthcare Analytics Dashboard Banner" width="100%" />
</p>

<h1 align="center">Healthcare Analytics Dashboard (Power BI)</h1>

<p align="center">
  <b>Revenue Forecasting • Patient Churn (Inactivity) • Profitability • Denials / Revenue Cycle</b>
</p>

<p align="center">
  <b>Mahadev Pandey</b> — Data Analyst | Power BI | SQL | DAX
</p>

<p align="center">
  <!-- Replace # with your links -->
  <a href="#">LinkedIn</a> •
  <a href="#">Portfolio</a> •
  <a href="mailto:your-email@gmail.com">Email</a>
</p>

<!-- =========================
     BADGES
========================== -->

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=000" />
  <img src="https://img.shields.io/badge/DAX-Measures-2E86C1" />
  <img src="https://img.shields.io/badge/Power%20Query-Data%20Cleaning-1f7a1f" />
  <img src="https://img.shields.io/badge/Forecasting-Built--in%20PBI-6f42c1" />
  <img src="https://img.shields.io/badge/Churn%20Analysis-Inactivity%20Model-ff7a59" />
  <img src="https://img.shields.io/badge/Profitability-Margin%20%25-0aa174" />
  <img src="https://img.shields.io/badge/Drill--through-Detail%20Page-444" />
  <img src="https://img.shields.io/badge/Status-Completed-0aa174" />
</p>

---

## 1) Project Overview

This project is a **Healthcare Analytics Power BI dashboard** designed to demonstrate end-to-end analytics skills used by hospitals/clinics and healthcare provider networks:

- **Revenue performance tracking** (Charges, Allowed, Paid)
- **Revenue forecasting** (monthly trend + built-in forecast)
- **Denials & revenue leakage analysis** (Denied/Pending impact + denial reasons)
- **Profitability analysis** (Profit, Margin %, service line profitability)
- **Patient churn (inactivity-based retention)** with drilldowns by facility/service line
- **Drill-through detail page** for root-cause investigation

> **Data Note:** Dataset is **synthetic / de-identified** and created for portfolio purposes.

---

## 2) Business Questions Answered

### Revenue & Forecasting
- How is **Net Revenue** trending month-over-month?
- What is the **expected revenue** for upcoming months (forecast)?
- Which **facility / service line** drives revenue?

### Revenue Cycle / Denials
- What is the **Denial Rate**?
- Which **denial reasons** contribute most to lost allowed revenue?
- Where is **revenue leakage** happening (Charges → Adjustments → Unpaid Allowed → Paid)?

### Profitability
- Which service lines are **high revenue but low/negative margin**?
- How does margin vary across **Payer Type × Service Line**?

### Patient Churn / Retention
- How many patients are active in the last 6 months?
- How many patients churned (inactive) and what is the churn rate?
- Which facility/service line has the **highest churn**?

---

## 3) Dashboard Pages

### Page 1 — Executive Summary
- KPI Cards: Net Revenue, Profit, Margin %, Denial Rate, Unique Patients
- **Monthly Net Revenue trend + Forecast**
- Breakdown visuals (facility/service line)

### Page 2 — Churn & Retention
- KPIs: Active Patients (Last 6M), Churned Patients, Churn Rate
- Churn Rate by Facility
- Churn Rate by Service Line

### Page 3 — Profitability & Revenue Cycle
- KPI Cards: Net Revenue, Profit, Margin %, Denied Allowed Amount, Paid vs Allowed %
- **Revenue Leakage Waterfall** (Charges → Adjustments → Unpaid Allowed → Total(Paid))
- Denied Allowed by Denial Reason
- **Matrix:** Margin % by PayerType × ServiceLine (red/green conditional formatting)
- Profit by Service Line

### Page 4 — Detail (Drillthrough)
- Drill-through enabled from visuals for deeper analysis
- Record-level table: Claim status, denial reason, amounts, costs
- Back button navigation

---

## 4) Key Metrics & Definitions (Business Logic)

### Revenue
- **Total Charges** = Sum of ChargeAmount  
- **Total Allowed** = Sum of AllowedAmount  
- **Total Paid / Net Revenue** = Sum of PaidAmount (simplified cash-based net revenue)

### Profitability
- **Profit** = Net Revenue − Direct Cost − Overhead  
- **Margin %** = Profit / Net Revenue  

### Denials
- **Denied Claims** = Claims with ClaimStatus = Denied  
- **Denial Rate** = Denied Claims / Total Claims (Completed encounters)

### Churn (Healthcare-appropriate)
Churn is modeled as **patient inactivity**:
- **Churned Patient:** Active in previous 6 months but **no completed visit** in last 6 months  
- **Churn Rate:** Churned Patients / Active Patients (Previous 6 months)

---

## 5) Data & Model

### Data Source
- Single encounter-level fact table: `healthcare_analytics`  
- Date dimension: `DimDate`

### Model Relationship
- `DimDate[Date]` → `healthcare_analytics[EncounterDate]` (1:*)

### Core Columns (examples)
- Dimensions: FacilityName, PayerType, ServiceLine, ProviderSpecialty, Region
- Revenue: ChargeAmount, AllowedAmount, AdjustmentAmount, PaidAmount
- RCM: ClaimStatus, DenialReason
- Costs: DirectCost, OverheadAllocated

---

## 6) Power BI Features Used

- Data cleaning & typing in **Power Query**
- **DimDate** table creation, sorting (YearMonth by MonthStart)
- DAX measures: revenue, cost, margin, denials, churn
- **Forecasting** on monthly Net Revenue trend
- **Conditional formatting** (Margin % red/green) for decision-ready insights
- **Synced slicers** across pages
- **Reset Filters** button using bookmarks
- **Drill-through** detail page for root-cause analysis

---

## 7) How to Run This Project

1. Download / clone the repo
2. Open the Power BI file:
   - `powerbi/Healthcare_Analytics_Dashboard.pbix`
3. If prompted for a file path, update the CSV connection:
   - `data/healthcare_analytics.csv`
4. Click **Refresh**
5. Use slicers (YearMonth, Facility, PayerType, ServiceLine) to explore

---

## 8) Screenshots (Add yours)

Create a folder: `assets/screenshots/` and add images, then link them below:

- Executive Summary  
  `![Executive Summary](assets/screenshots/executive_summary.png)`

- Churn & Retention  
  `![Churn](assets/screenshots/churn_retention.png)`

- Profitability & Revenue Cycle  
  `![Profitability](assets/screenshots/profitability_rcm.png)`

- Drillthrough Detail  
  `![Detail](assets/screenshots/detail_drillthrough.png)`

---

## 9) Insights You Can Demonstrate (Examples)

- Identify loss-making segments using **Margin % matrix** across payers and service lines
- Quantify revenue leakage using the **waterfall** (charges → adjustments → unpaid allowed → paid)
- Pinpoint denial categories driving high leakage via **Denied Allowed by Denial Reason**
- Spot churn hotspots by facility/service line and prioritize retention improvements

---

## 10) Assumptions & Limitations
- Synthetic/de-identified data used for demo purposes
- Net revenue modeled as paid amount (cash-based simplification)
- Churn definition based on 180-day inactivity windows (configurable)

---

## 11) Author
**Mahadev Pandey**  
Data Analyst | Power BI | SQL | DAX  
- LinkedIn: <add-link>  
- Email: <add-email>

---
