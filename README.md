# Healthcare Analytics Dashboard (Power BI) — Revenue Forecasting, Churn & Profitability

A recruiter-ready **Power BI** project built to demonstrate end-to-end analytics skills in a healthcare provider context: **revenue performance**, **revenue cycle/denials**, **patient churn (inactivity)**, and **profitability** with interactive filtering, drill-through, forecasting, and clean reporting.

> **Note on data:** This project uses **synthetic / de-identified** encounter-level data for portfolio/demo purposes.

---

## Business Context (What this dashboard is about)

Healthcare organizations typically need to answer:
- How is revenue trending across facilities, payers, and service lines?
- What revenue leakage is happening due to **denials/pending claims**?
- Which services/facilities/providers are actually **profitable** after costs and overhead?
- Are patients returning (retention) or becoming inactive (**churn**)?

This dashboard is designed as a compact decision-support tool for leadership, operations, and finance teams.

---

## What You Can Demonstrate With This Project

### As a Data Analyst / BI Analyst, this project shows you can:
- Build a clean **data model** (DimDate + fact table) and make reports filter correctly.
- Write business-grade **DAX measures** (Revenue, Profit, Margin%, Denial Rate, Churn Rate).
- Create executive KPI views + drilldowns using **interactive visuals**.
- Implement usability features recruiters like:
  - **Slicer sync** across pages
  - **Bookmark-based Reset Filters button**
  - **Conditional formatting** (red/green) to highlight performance issues
  - **Drill-through detail page** for root-cause analysis
- Use built-in Power BI analytics for **revenue forecasting**

---

## Dashboard Pages

### 1) Executive Summary
**Goal:** Quick health check of the business and trends.
- KPI Cards: Net Revenue, Profit, Margin %, Denial Rate, Patient count
- Monthly trend line: **Net Revenue by MonthStart**
- Built-in **Forecast** applied to revenue trend
- Breakdown charts by Facility / Service Line (as added)

### 2) Churn & Retention
**Goal:** Identify patient inactivity and where retention is weak.
- KPIs: Active Patients (Last 6M), Churned Patients, Churn Rate
- Churn Rate by Facility
- Churn Rate by Service Line

### 3) Profitability & Revenue Cycle (RCM)
**Goal:** Profit analysis + claim leakage and denial drivers.
- KPI Cards: Net Revenue, Profit, Margin %, Denied Allowed, Paid vs Allowed %
- **Revenue leakage Waterfall** (Charges → Adjustments → Unpaid Allowed → Total(Paid))
- Profit by Service Line
- Denied Allowed by Denial Reason
- Matrix: **Margin % by PayerType × ServiceLine** with red/green conditional formatting

### 4) Detail (Drillthrough)
**Goal:** Investigate a selected Facility + Service Line in detail.
- Drill-through enabled from summary visuals
- Record-level table: EncounterDate, PatientID, ClaimStatus, DenialReason, Charges, Allowed, Paid, Costs
- Back button navigation

---

## Key Metric Definitions (Business Logic)

### Revenue & Profitability
- **Total Charges** = Sum of submitted charges  
- **Total Allowed** = Contract-allowed amount  
- **Total Paid / Net Revenue** = Payments received (simplified as Net Revenue)  
- **Profit** = Net Revenue − Direct Cost − Overhead  
- **Margin %** = Profit / Net Revenue  

### Revenue Cycle
- **Denial Rate** = Denied Claims / Total Claims (Completed encounters)

### Patient Churn (Inactivity-Based)
Healthcare churn is modeled as **patient inactivity**:

- **Active Patients (Last 6M):** patients with ≥1 completed encounter in last 180 days  
- **Active Patients (Prev 6M):** patients with ≥1 completed encounter in the 180 days before that  
- **Churned Patients:** active in previous 6M, but not active in last 6M  
- **Churn Rate:** Churned Patients / Active Patients (Prev 6M)

---

## Data Model Overview

This project uses:
- `DimDate` (Date table) related to:
- `healthcare_analytics` (encounter-level fact table)

Relationship:
- `DimDate[Date]` → `healthcare_analytics[EncounterDate]` (One-to-Many)

---

## Data Dictionary (Main Table Fields)

**Entity keys**
- EncounterID, PatientID, ProviderID, FacilityID, PayerID

**Dates**
- EncounterDate

**Dimensions**
- ProviderSpecialty, FacilityName, Region, PayerType, ServiceLine, VisitType, EncounterStatus

**Revenue cycle**
- ChargeAmount, AllowedAmount, AdjustmentAmount, PaidAmount
- ClaimStatus (Paid / Denied / Pending / NA)
- DenialReason

**Cost**
- DirectCost, OverheadAllocated

---

## Power BI Features Implemented

- Power Query: data type fixes, basic cleaning
- DAX Measures: revenue, profitability, denials, churn
- Forecasting: built-in forecast on monthly revenue trend
- Conditional formatting: Margin % red/green in matrix
- Drill-through: Facility + ServiceLine detail page
- Synced slicers across pages
- Reset Filters: bookmark + button action

---

## Repository Contents (Suggested)
