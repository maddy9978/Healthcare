<div align="center">

<!-- ============================================================
     BANNER — SVG embedded directly for GitHub rendering
============================================================ -->

<svg width="900" height="220" viewBox="0 0 900 220" xmlns="http://www.w3.org/2000/svg" style="border-radius:12px;">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0a1628;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#0d2240;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0a1628;stop-opacity:1" />
    </linearGradient>
    <linearGradient id="accent" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0aa174;stop-opacity:1" />
    </linearGradient>
    <linearGradient id="bar1" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:0.9" />
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:0.2" />
    </linearGradient>
    <linearGradient id="bar2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#0aa174;stop-opacity:0.9" />
      <stop offset="100%" style="stop-color:#0aa174;stop-opacity:0.2" />
    </linearGradient>
    <linearGradient id="bar3" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#F2C811;stop-opacity:0.9" />
      <stop offset="100%" style="stop-color:#F2C811;stop-opacity:0.2" />
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="220" fill="url(#bg)" rx="12"/>

  <!-- Subtle grid lines -->
  <line x1="0" y1="55" x2="900" y2="55" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="0" y1="110" x2="900" y2="110" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="0" y1="165" x2="900" y2="165" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>

  <!-- Mini bar chart (decorative, right side) -->
  <rect x="700" y="140" width="18" height="50" fill="url(#bar1)" rx="3" opacity="0.7"/>
  <rect x="724" y="115" width="18" height="75" fill="url(#bar2)" rx="3" opacity="0.7"/>
  <rect x="748" y="130" width="18" height="60" fill="url(#bar3)" rx="3" opacity="0.7"/>
  <rect x="772" y="100" width="18" height="90" fill="url(#bar1)" rx="3" opacity="0.7"/>
  <rect x="796" y="120" width="18" height="70" fill="url(#bar2)" rx="3" opacity="0.7"/>
  <rect x="820" y="90" width="18" height="100" fill="url(#bar3)" rx="3" opacity="0.7"/>
  <rect x="844" y="108" width="18" height="82" fill="url(#bar1)" rx="3" opacity="0.7"/>

  <!-- Trend line over bars -->
  <polyline points="709,135 733,110 757,125 781,95 805,115 829,85 853,102"
    fill="none" stroke="url(#accent)" stroke-width="2.5" stroke-linecap="round"
    stroke-linejoin="round" filter="url(#glow)" opacity="0.9"/>
  <!-- Trend dots -->
  <circle cx="709" cy="135" r="3.5" fill="#00d4ff" filter="url(#glow)"/>
  <circle cx="733" cy="110" r="3.5" fill="#00d4ff" filter="url(#glow)"/>
  <circle cx="757" cy="125" r="3.5" fill="#0aa174" filter="url(#glow)"/>
  <circle cx="781" cy="95" r="3.5" fill="#0aa174" filter="url(#glow)"/>
  <circle cx="805" cy="115" r="3.5" fill="#F2C811" filter="url(#glow)"/>
  <circle cx="829" cy="85" r="3.5" fill="#F2C811" filter="url(#glow)"/>
  <circle cx="853" cy="102" r="3.5" fill="#00d4ff" filter="url(#glow)"/>

  <!-- Heartbeat / ECG line (left decorative) -->
  <polyline points="30,110 60,110 75,70 90,145 105,90 120,125 135,110 160,110"
    fill="none" stroke="#00d4ff" stroke-width="2" stroke-linecap="round"
    stroke-linejoin="round" filter="url(#glow)" opacity="0.5"/>

  <!-- Accent top bar -->
  <rect x="0" y="0" width="900" height="4" fill="url(#accent)" rx="2"/>

  <!-- Main Title -->
  <text x="200" y="78" font-family="'Segoe UI', Arial, sans-serif" font-size="26"
    font-weight="700" fill="#ffffff" letter-spacing="0.5">Healthcare Analytics Intelligence</text>

  <!-- Subtitle / Dashboard name -->
  <text x="200" y="108" font-family="'Segoe UI', Arial, sans-serif" font-size="14"
    font-weight="400" fill="#00d4ff" letter-spacing="1.5">REVENUE · RETENTION · REVENUE CYCLE MANAGEMENT</text>

  <!-- Divider line -->
  <rect x="200" y="120" width="440" height="1.5" fill="url(#accent)" opacity="0.5" rx="1"/>

  <!-- Tag line -->
  <text x="200" y="142" font-family="'Segoe UI', Arial, sans-serif" font-size="12"
    fill="#8ab4d4" letter-spacing="0.3">End-to-end Power BI dashboard · DAX · Power Query · Forecasting</text>

  <!-- Author -->
  <text x="200" y="168" font-family="'Segoe UI', Arial, sans-serif" font-size="13"
    font-weight="600" fill="#ffffff" opacity="0.9">Mahadev Pandey</text>
  <text x="200" y="186" font-family="'Segoe UI', Arial, sans-serif" font-size="11"
    fill="#8ab4d4">Data Analyst · Power BI · SQL · DAX · Python</text>

  <!-- Power BI logo-ish badge -->
  <rect x="200" y="198" width="82" height="16" rx="8" fill="#F2C811" opacity="0.15"/>
  <text x="241" y="210" font-family="'Segoe UI', Arial, sans-serif" font-size="10"
    font-weight="600" fill="#F2C811" text-anchor="middle">⚡ Power BI</text>
</svg>

<br/>

# Healthcare Analytics Intelligence
### Revenue · Retention · Revenue Cycle Management

**Mahadev Pandey** — Data Analyst | Power BI | SQL | DAX

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/your-profile)
[![Portfolio](https://img.shields.io/badge/Portfolio-View-0aa174)](https://github.com/maddy9978)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?logo=gmail&logoColor=white)](mailto:your-email@gmail.com)

---

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=000)
![DAX](https://img.shields.io/badge/DAX-Measures-2E86C1)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Cleaning-1f7a1f)
![Forecasting](https://img.shields.io/badge/Forecasting-Built--in%20PBI-6f42c1)
![Churn Analysis](https://img.shields.io/badge/Churn%20Analysis-Inactivity%20Model-ff7a59)
![Profitability](https://img.shields.io/badge/Profitability-Margin%20%25-0aa174)
![Drill-through](https://img.shields.io/badge/Drill--through-Detail%20Page-444444)
![Status](https://img.shields.io/badge/Status-Completed-0aa174)

</div>

---

## 📋 Table of Contents

1. [Project Overview](#1-project-overview)
2. [Business Questions Answered](#2-business-questions-answered)
3. [Dashboard Pages](#3-dashboard-pages)
4. [Key Metrics & Definitions](#4-key-metrics--definitions-business-logic)
5. [Data Model](#5-data--model)
6. [Power BI Features Used](#6-power-bi-features-used)
7. [How to Run](#7-how-to-run-this-project)
8. [Screenshots](#8-screenshots)
9. [Insights You Can Demonstrate](#9-insights-you-can-demonstrate)
10. [Assumptions & Limitations](#10-assumptions--limitations)
11. [Author](#11-author)

---

## 1) Project Overview

**Healthcare Analytics Intelligence** is a 4-page Power BI dashboard built to simulate the analytics workflows used by hospitals, clinics, and healthcare provider networks. It covers the full analytics spectrum — from executive-level revenue tracking to granular revenue cycle management and patient retention analysis.

| Analytics Domain | What It Covers |
|---|---|
| 💰 Revenue Performance | Charges, Allowed, Paid — month-over-month tracking |
| 📈 Revenue Forecasting | Built-in PBI forecast on monthly net revenue trend |
| 🚫 Denials & Leakage | Denied/Pending impact + denial reason breakdown |
| 📊 Profitability | Profit, Margin %, service line & payer profitability |
| 🔄 Patient Churn | Inactivity-based retention model with drilldowns |
| 🔍 Drill-through | Record-level root-cause investigation page |

> **Data Note:** Dataset is **synthetic / de-identified** and created for portfolio purposes only.

---

## 2) Business Questions Answered

### 💰 Revenue & Forecasting
- How is **Net Revenue** trending month-over-month?
- What is the **expected revenue** for upcoming months (forecast)?
- Which **facility / service line** is the primary revenue driver?

### 🚫 Revenue Cycle / Denials
- What is the current **Denial Rate**?
- Which **denial reasons** are contributing most to lost allowed revenue?
- Where exactly is **revenue leakage** happening? (Charges → Adjustments → Unpaid Allowed → Paid)

### 📊 Profitability
- Which service lines are **high revenue but low / negative margin**?
- How does margin vary across the **Payer Type × Service Line** matrix?

### 🔄 Patient Churn / Retention
- How many patients are **active in the last 6 months**?
- How many patients have **churned (gone inactive)** and what is the churn rate?
- Which **facility / service line** has the highest churn risk?

---

## 3) Dashboard Pages

### 📄 Page 1 — Executive Summary
> *The C-suite view — performance at a glance*

- KPI Cards: Net Revenue, Profit, Margin %, Denial Rate, Unique Patients
- Monthly Net Revenue trend line with **built-in forecast**
- Revenue breakdown by Facility and Service Line

---

### 📄 Page 2 — Churn & Retention
> *Patient retention intelligence powered by inactivity modelling*

- KPIs: Active Patients (Last 6M), Churned Patients, Churn Rate %
- Churn Rate by Facility (bar chart)
- Churn Rate by Service Line (bar chart)

---

### 📄 Page 3 — Profitability & Revenue Cycle
> *Where money is made — and where it leaks*

- KPI Cards: Net Revenue, Profit, Margin %, Denied Allowed Amount, Paid vs Allowed %
- **Revenue Leakage Waterfall:** Charges → Adjustments → Unpaid Allowed → Total Paid
- Denied Allowed Amount by Denial Reason
- **Margin % Matrix:** Payer Type × Service Line with red/green conditional formatting
- Profit by Service Line

---

### 📄 Page 4 — Detail (Drill-through)
> *Root-cause investigation at record level*

- Drill-through enabled from any visual across pages
- Record-level table: Claim Status, Denial Reason, Charge / Allowed / Paid amounts, Costs
- Back-button navigation

---

## 4) Key Metrics & Definitions (Business Logic)

### Revenue

| Measure | Formula |
|---|---|
| Total Charges | `SUM(ChargeAmount)` |
| Total Allowed | `SUM(AllowedAmount)` |
| Net Revenue | `SUM(PaidAmount)` *(cash-based simplification)* |

### Profitability

| Measure | Formula |
|---|---|
| Profit | `Net Revenue − Direct Cost − Overhead` |
| Margin % | `Profit / Net Revenue` |

### Denials

| Measure | Formula |
|---|---|
| Denied Claims | Claims where `ClaimStatus = "Denied"` |
| Denial Rate | `Denied Claims / Total Completed Claims` |

### Churn (Healthcare Inactivity Model)

| Term | Definition |
|---|---|
| **Churned Patient** | Had a completed visit in the prior 6-month window, but **no completed visit** in the most recent 6 months |
| **Churn Rate** | `Churned Patients / Active Patients (Previous 6M)` |

> Churn window is **configurable** — currently set to **180 days**.

---

## 5) Data & Model

### Data Source
- Single encounter-level fact table: `healthcare_analytics`
- Date dimension table: `DimDate`

### Model Relationship
```
DimDate[Date]  ──1:*──►  healthcare_analytics[EncounterDate]
```

### Core Columns

| Category | Columns |
|---|---|
| **Dimensions** | FacilityName, PayerType, ServiceLine, ProviderSpecialty, Region |
| **Revenue** | ChargeAmount, AllowedAmount, AdjustmentAmount, PaidAmount |
| **RCM** | ClaimStatus, DenialReason |
| **Costs** | DirectCost, OverheadAllocated |

---

## 6) Power BI Features Used

| Feature | Usage |
|---|---|
| **Power Query** | Data cleaning, column typing, date table creation |
| **DimDate Table** | YearMonth sorted by MonthStart for correct trend ordering |
| **DAX Measures** | Revenue, cost, margin, denials, churn logic |
| **Built-in Forecasting** | Applied to monthly Net Revenue trend visual |
| **Conditional Formatting** | Red/green Margin % in Payer × Service Line matrix |
| **Synced Slicers** | YearMonth, Facility, PayerType, ServiceLine across all pages |
| **Bookmarks** | Reset Filters button for one-click slicer reset |
| **Drill-through** | Detail page with record-level data for root-cause analysis |

---

## 7) How to Run This Project

```bash
# 1. Clone the repository
git clone https://github.com/maddy9978/Healthcare.git

# 2. Open the Power BI file
powerbi/Healthcare_Analytics_Dashboard.pbix

# 3. If prompted, update the CSV data source path
data/healthcare_analytics.csv

# 4. Click Refresh in Power BI Desktop

# 5. Use slicers to explore:
#    YearMonth | Facility | PayerType | ServiceLine
```

---

## 8) Screenshots

> 📁 Add your screenshots to `assets/screenshots/` and they will render here.

| Page | Preview |
|---|---|
| Executive Summary | ![Executive Summary](assets/screenshots/executive_summary.png) |
| Churn & Retention | ![Churn](assets/screenshots/churn_retention.png) |
| Profitability & RCM | ![Profitability](assets/screenshots/profitability_rcm.png) |
| Drill-through Detail | ![Detail](assets/screenshots/detail_drillthrough.png) |

---

## 9) Insights You Can Demonstrate

- 🔴 **Loss-making segments** — Use the Margin % matrix (Payer × Service Line) to instantly identify red-zone combinations requiring intervention
- 💧 **Revenue leakage quantification** — Trace the full waterfall from gross charges to net paid to spot where money disappears
- 🚫 **Denial root-cause** — Identify the top denial reason categories driving allowed revenue loss
- 📉 **Churn hotspots** — Surface the facilities and service lines with highest patient inactivity rates for targeted retention action

---

## 10) Assumptions & Limitations

- Synthetic / de-identified data — for portfolio demonstration only
- Net Revenue modelled as Paid Amount (cash-based simplification; not accrual)
- Churn definition based on **180-day inactivity windows** (configurable in DAX)
- No real-time data refresh — static CSV source

---

## 11) Author

<div align="center">

**Mahadev Pandey**
*Data Analyst · Power BI · SQL · DAX · Python*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mahadev%20Pandey-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/your-profile)
[![GitHub](https://img.shields.io/badge/GitHub-maddy9978-181717?logo=github&logoColor=white)](https://github.com/maddy9978)
[![Email](https://img.shields.io/badge/Email-your--email%40gmail.com-D14836?logo=gmail&logoColor=white)](mailto:your-email@gmail.com)

*If this project was helpful, consider giving it a ⭐ — it motivates continued open work!*

</div>

---

<div align="center">
  <sub>Built with ❤️ using Power BI · DAX · Power Query · Synthetic Healthcare Data</sub>
</div>
