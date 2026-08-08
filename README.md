# COVID-19 Global Case Analysis — Excel Project
**An Excel-based analytics project exploring global COVID-19 case data across 188 countries — built to practice and demonstrate core to advanced 
Excel skills: Power Query, PivotTables, slicers, timelines, lookup functions, and formula-driven risk classification.**

# Project Overview
**This project analyses country-level COVID-19 data (confirmed cases, deaths, recoveries, active cases, and population) to answer key questions:**

**Which countries and continents carry the highest case and death burden?**

**How did case trends evolve over time (by month/year)?**

**Which countries fall into High / Moderate / Low risk categories based on death rate?**

**How does case distribution vary by continent?**

**It's built as a standalone Excel workbook — no external BI tool — to specifically showcase Excel as a complete analysis and reporting layer, 
complementing a separate SQL + Python + Power BI insurance analytics project in my portfolio.**

# What Was Done
# 1. Data Preparation

**Loaded and structured the dataset (188 countries) as an Excel Table, sourced via Power Query, so all downstream formulas and PivotTables refresh automatically 
with the underlying data.**

# 2. Calculated Fields
**Death Rate = Deaths ÷ Confirmed**

**Recovery Rate = Recovered ÷ Confirmed**

**Infection Rate = Confirmed ÷ Population**

**Risk Factor — an IFS() formula classifying each country as High Risk (>5% death rate), Moderate Risk (2–5%), or Low Risk (<2%)**

# 3. Lookup Practice
**Built a dedicated sheet using VLOOKUP (vertical lookup against the main data table) and HLOOKUP (horizontal lookup against a transposed reference table) to 
retrieve Population and Continent for selected countries — deliberately structured to demonstrate both lookup orientations.**

# 4. PivotTables, Charts & Interactivity
**5 PivotTables summarizing confirmed cases, deaths, and recoveries by time period and continent**

**5 charts — bar, column, combo (area + line), and pie — visualizing case trends over time and continent-level distribution**

**2 slicers and 1 Timeline (filtering by "Date of First Case") for interactive, date-driven exploration of the dashboard**

# 5. Continent-Level Summary
**Aggregated case share by continent using SUMIF-based logic, visualized as a pie chart on the Visualisation sheet 
(e.g., North America ~30%, Asia ~24%, South America ~23% of total confirmed cases)**

# Key Insights
**North America and Asia together account for over half of global confirmed cases (~30% and ~24% respectively), with South America close behind (~23%).**

**Case growth was heavily concentrated in a short window — the Jan–Mar 2020 period alone accounts for the vast majority of case volume in the dataset, 
reflecting the initial global spread.**

**Death rate varies significantly by country regardless of case volume — several countries with comparatively lower confirmed case counts show disproportionately
high death rates, flagged automatically via the Risk Factor classification.**

**Australia/Oceania has minimal representation (~0.1% of global cases) compared to other continents, consistent with stricter early containment in that region.**

# Skills Demonstrated
**Power Query · Excel Tables · PivotTables & PivotCharts · Slicers & Timelines · VLOOKUP · HLOOKUP · IFS() · SUMIF · Formula-driven Risk Classification · Dashboard Design**

# Notes & Limitations
**Dataset reflects a snapshot of COVID-19 case data and is used here for analytical practice, not real-time reporting.**

**Risk Factor thresholds (2% / 5%) are illustrative classification bands, not epidemiological standards.**

**Lookup formulas are structured for demonstration; production use would wrap them in IFERROR() to handle unmatched lookup values gracefully.**

# Author
**Anuska Biswas**
