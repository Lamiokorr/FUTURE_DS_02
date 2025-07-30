# FUTURE_DS_02
# 📊 Campaign Performance Analysis with Power BI
This project is part of a data analytics learning journey where I analyzed a digital ad campaign dataset to uncover performance insights using **Power BI**.

## 🔍 Project Overview
The goal of this project was to build an interactive dashboard that enables stakeholders to:

- Measure how well the ad campaign performed
- Identify top-performing ads and audience segments
- Calculate key performance metrics using **DAX**
- Discover actionable recommendations for future campaigns

## 🧠 Key Questions Addressed

- How well did the ad campaign perform?
- Which posts or ads had the highest engagement?
- What can we improve for the next campaign?

## 📈 Dashboard Features

- **Campaign KPIs**: Total impressions, clicks, conversions, CPC, and ROI
- **Engagement Insights**: Top-performing ads and demographics by engagement
- **Interactive Filters**: Slice by age, gender, campaign ID, and more
- **Recommendations Panel**: Data-driven insights for future marketing strategy

## 🧮 DAX Measures Used

```DAX
CPC = DIVIDE(SUM('data'[spent]), SUM('data'[clicks]))

ROI = 
VAR Revenue = SUM('data'[approved_conversion]) * 10
VAR Cost = SUM('data'[spent])
RETURN DIVIDE(Revenue - Cost, Cost)
