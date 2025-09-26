# Cost of Living Pressures for Low-Income Households

## Introduction
The rising cost of living is a pressing issue, especially for low-income households earning less than RM3000 per month. 
Understanding how macroeconomic factors such as inflation, consumer prices, and population demographics intersect 
can help policymakers and businesses create strategies that improve affordability and economic resilience. 
This analysis integrates multiple datasets covering household CPI, state-level inflation, population demographics, 
and expenditure classification—to uncover meaningful insights into cost of living pressures in Malaysia.  

---

## Problem Statement
While consumer price inflation is widely monitored, there is limited focus on how these trends specifically affect 
low-income households at the state and demographic levels. Without linking general CPI trends to population structures 
and low-income household indices, it is difficult to identify which groups are most vulnerable to rising living costs.  

This project addresses the following questions:  
- How do national low-income CPI trends compare with state-level CPI trends across divisions of goods and services?  
- Which categories of goods (e.g., food, housing, transport) contribute most to cost of living increases for low-income households?  
- How do population demographics (sex, ethnicity, DUN-level structures) interact with inflationary pressures?  

---

## Objectives
The key objectives of this analysis are:  
1. **To measure cost of living pressures on low-income households** by comparing national-level CPI indices with 
   state-level inflation rates.  
2. **To identify categories of goods and services driving inflation** using the MCOICOP classification.  
3. **To examine demographic vulnerability** by linking population distributions (state, DUN, ethnicity, sex) with 
   inflation categories.  
4. **To uncover patterns and relationships** such as whether states with higher non-citizen populations or different 
   demographic balances face different inflation impacts.  

---

## Datasets
| Dataset | Key Columns                                                 |
|---------|-------------------------------------------------------------|
| Low-Income CPI | date, division, index                                       |
| State-Level CPI | state, date, division, inflation_yoy, inflation_mom         |
| Population by DUN | date, state, parlimen, dun, sex, age, ethnicity, population |
| MCOICOP Lookup | digits, division, group	class, subclass, desc_en, desc_bm   |

---

## Correlation & Sensitivity Analysis

[//]: # (# Patterns & Relationships to Explore)

1. The low-income CPI index shows how living costs rise over time, with some categories (e.g., food, housing) increasing faster than others.
2. Comparing national low-income CPI with state-level inflation reveals whether certain states face higher cost pressures than the national trend.
3. Linking population data (sex, ethnicity, DUN-level) with inflation highlights which groups may be more exposed to rising costs.
4. Identifying which divisions (food, housing, transport, etc.) drive most of the CPI increase shows which essentials hit low-income households hardest.
5. State-level comparisons uncover whether urban-heavy states face different inflation dynamics compared to rural-heavy ones.  

---

## Methodology
1. **Data Preparation**  
   - Clean and standardize datasets.  
   - Handle missing values and inconsistent formats.  
   - Align datasets by time (2010–2023 for macro data) and region/household attributes.  

2. **Analytical Approach**  
   - Descriptive statistics and visualization for each dataset.  
   - Correlation and regression analysis to link macroeconomic indicators with expenses and incomes.  
   - Household segmentation by demographics (`sex`, `ethnicity`, `state`).  
   - Trend analysis of inflation vs. population structures vs. household costs.  

3. **Expected Deliverables**  
   - Insights into macroeconomic pressures on household budgets.  
   - Identification of households most vulnerable to rising living costs.  
   - Visualizations (trends, correlation heatmaps, affordability gaps).  
   - Recommendations for policymakers and households to strengthen financial resilience.  

## Data Source:
- Low-Income CPI: https://data.gov.my/data-catalogue/cpi_lowincome
- State-Level CPI: https://data.gov.my/data-catalogue/cpi_state_inflation
- Population by DUN: https://data.gov.my/data-catalogue/population_dun
- MCOICOP Lookup: https://open.dosm.gov.my/data-catalogue/mcoicop
