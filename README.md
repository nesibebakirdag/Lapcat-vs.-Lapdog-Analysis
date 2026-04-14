# 🐾 Lapcat vs. Lapdog: Executive Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-005571?style=for-the-badge)
![DAX](https://img.shields.io/badge/DAX-DA1F28?style=for-the-badge)

## 📌 Project Overview
The **Waggle** company has safely dominated the pet tech market with their successful "Lapdog" smart collar. However, the Board of Directors asked a crucial business question: *"Should we leverage our technology and launch Lapcat, a smart collar variant for cats?"*

To answer this data-driven question, 1,000 Lapcat prototypes were deployed, and months of telemetry and customer synchronization data were collected. This project turns that raw data into an **End-to-End Executive Dashboard** to provide a direct strategic business recommendation to the C-Level management.

## ⚙️ The Tech Stack & Workflow
- **ETL Process:** Cleansed, transformed, and formatted raw datasets using **Power Query**.
- **Data Modeling:** Built a robust **Star Schema** architecture utilizing bi-directional cross-filtering.
  - *Fact Tables:* Tracker Data, Rating Data
  - *Dimension Tables:* Pet Data, Family Data, Date Table
- **DAX Calculations:** Engineered dynamic measures for KPI cards, custom conditions, and complex conditional formatting.
- **UI/UX Design:** Designed a corporate aesthetic utilizing modern interactive navigation flows, slicers, and calculated negative space.
- **Advanced Features:** Implemented hidden **Drillthrough** functionality to act as a micro-CRM for analyzing individual family/customer profiles directly from the executive summaries.

## 📊 Key Business Insights
After segmenting the behaviors and satisfaction rates across geographies and demographics, the data revealed a striking reality:
1. **Dog Dominance (Cash Cow):** Lapdog users walk an average of **12.2K steps/day** and evaluate the product with a stable **4.7/5** rating. The brand recommendation (NPS) rate stands at a massive **89%**.
2. **Lapcat Failure (The Prototype):** Lapcat users only log **2.8K steps/day**, and customer satisfaction plummeted to **1.8/5**. Only **11%** of users recommend the product.
3. **Executive Verdict:** The Lapcat prototype completely fails to align with feline behavioral nature (who prefer indoor activities over step-count goals). **Recommendation:** Cancel the launch in its current form to avoid severe brand devaluation. The product should be sent back to R&D to focus on cat-specific metrics like sleep tracking or heart rate.

## 🚀 How to Navigate the Dashboard
1. **Home Page:** Executive summary and drill-down analysis of behavioral/satisfaction differences between cats and dogs, driven by a dynamic Slicer.
2. **General Pet Data:** Geographic distribution (Map Visuals), top breeds, age, and gender demographics.
3. **Family Data:** Financial correlation between household income and pet expenses mapped via Scatter Charts.
4. **Drillthrough (Hidden Feature):** Right-click on any specific family name in the data table and select 'Drill through' to jump into their micro-profile to read direct customer reviews, purchase platforms, and individual telemetry data.



### 3. Family Profile (Drillthrough POV)
*(Add image here: `![Drillthrough](link)`)*

---
*Prepared by a passionate Data Analyst turning raw spreadsheets into strategic business decisions.*
