# Cost of Living Pressures for Low-Income Households

## Introduction
---
The rising cost of living is a pressing issue, especially for low-income households earning less than RM3000 per month. Understanding how macroeconomic factors such as inflation, consumer prices, and population demographics intersect can help policymakers and businesses create strategies that improve affordability and economic resilience. This analysis integrates multiple datasets covering household CPI, state-level inflation, population demographics, and expenditure classification—to uncover meaningful insights into cost of living pressures in Malaysia.

## Problem Statement
The rising cost of living is a pressing issue, especially for low-income households earning less than RM3000 per month. Understanding how macroeconomic factors such as inflation, consumer prices, and population demographics intersect can help policymakers and businesses create strategies that improve affordability and economic resilience. This analysis integrates multiple datasets covering household CPI, state-level inflation, population demographics, and expenditure classification—to uncover meaningful insights into cost of living pressures in Malaysia.
This project addresses the following questions:

- How do national low-income CPI trends compare with state-level CPI trends across divisions of goods and services?  
- Which categories of goods and services (e.g., food, housing, transport) contribute most to cost of living increases for low-income households?  
- How do population demographics (sex, ethnicity, DUN-level structures) interact with inflationary pressures?  

---

## Objectives
The key objectives of this analysis are:

1. **Measure cost of living pressures on low-income households** by comparing national CPI indices with state-level inflation rates.  
2. **Identify categories of goods and services driving inflation** using the MCOICOP classification.  
3. **Examine demographic vulnerability** by linking population distributions (state, DUN, ethnicity, sex) with inflation categories.  
4. **Uncover patterns and relationships** such as whether states with higher non-citizen populations or different demographic balances experience different inflation impacts.  

---

## Datasets

| Dataset           | Key Columns                                                 | Notes |
|-------------------|-------------------------------------------------------------|-------|
| Low-Income CPI    | date, division, index                                       | National CPI for low-income households; trends by division. |
| State Level CPI   | date, division, index                                       | CPI at the state level for comparison with national trends. |
| Inflation CPI     | state, date, division, inflation_yoy, inflation_mom         | State-level inflation data by division. |
| Population by DUN | date, state, parlimen, dun, sex, age, ethnicity, population | Demographic analysis; can calculate population ratios to measure vulnerability. |
| MCOICOP Lookup    | digits, division, group, class, subclass, desc_en, desc_bm  | CPI division hierarchy; used to map divisions into general categories. |

---

## Correlation & Sensitivity Analysis

1. National and low-income CPI trends show how living costs rise over time, with certain categories (e.g., food, housing) increasing faster than others.  
2. Comparing national CPI with state-level inflation reveals which states face higher cost pressures.  
3. Linking population demographics (sex, ethnicity, DUN-level) with inflation highlights which groups may be most exposed.  
4. Identifying divisions driving CPI increases shows which essentials hit low-income households hardest.  
5. State-level comparisons uncover whether urban-heavy states face different inflation dynamics than rural-heavy states.  

---

## Methodology

### 1. Data Preparation
- Clean and standardize all datasets.  
- Handle missing values and inconsistent formats.  
- Align datasets by time (2010–2023) and by region/household attributes.  

### 2. Analytical Approach
- Perform descriptive statistics and visualization for each dataset.  
- Conduct correlation and regression analysis to link macroeconomic indicators with household expenses and incomes.  
- Segment households by demographics (`sex`, `ethnicity`, `state`).  
- Analyze trends of inflation vs. population structures and household costs.  

### 3. Expected Deliverables
- Insights into macroeconomic pressures on household budgets.  
- Identification of households most vulnerable to rising living costs.  
- Visualizations: trend charts, correlation heatmaps, and affordability gaps.  
- Recommendations for policymakers and households to strengthen financial resilience.  

---

## Data Sources
- Low-Income CPI: [https://data.gov.my/data-catalogue/cpi_lowincome](https://data.gov.my/data-catalogue/cpi_lowincome)  
- State-Level CPI: [https://data.gov.my/data-catalogue/cpi_core](https://data.gov.my/data-catalogue/cpi_core)  
- Inflation CPI: [https://data.gov.my/data-catalogue/cpi_state_inflation](https://data.gov.my/data-catalogue/cpi_state_inflation)  
- Population by DUN: [https://data.gov.my/data-catalogue/population_dun](https://data.gov.my/data-catalogue/population_dun)  
- MCOICOP Lookup: [https://open.dosm.gov.my/data-catalogue/mcoicop](https://open.dosm.gov.my/data-catalogue/mcoicop)  
