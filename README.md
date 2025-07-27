# 🚕 Uber Fares Data Analysis & Visualization Project

## 📌 Overview

This project explores and visualizes patterns in Uber ride fares using a cleaned and enhanced dataset. The goal is to extract actionable insights from temporal, spatial and fare-related trends to support decision-making in transportation data analytics.

---

## 🎯 Project Objectives

- Analyze fare patterns across time (hourly, daily, monthly)
- Examine ride demand and peak hours
- Identify seasonal and geographic trends
- Present findings through a professional Power BI dashboard
- Recommend insights for business improvement

---

## 🗂️ Repository Structure

```
📁 Uber-Fares-Analysis
├──📁 datasets
├   ├── Enhanced_Uber_Fares.csv            # Enhanced dataset
├   ├── uber.csv                           # Original dataset
├   ├── Cleaned_Uber_Fares.csv             # Cleaned dataset
├──📁 python
|   ├──boxplot.ipynb
|   ├──eda_uber.ipynb
|   ├──feature_engineering_uber.ipynb
|   ├──uber_data_preprocessing.ipynb
├── 📸 screenshots/
│   
├── 📁 DAX_Formulas.txt                   # Power BI DAX formulas used
├── 📁 PowerBI_Dashboard.pbix            # Interactive Power BI dashboard
├── 📄 Report_Presentation.pptx          # Final summarized PPT report
├── 📘 README.md                          # This markdown file
```

---

## 🧹 Data Cleaning & Preparation

The dataset was preprocessed in Python using pandas:

- Removed nulls and outliers (e.g., negative fares, impossible coordinates)
- Converted timestamps to datetime
- Extracted hour, day, month, year
- Created `fare_bin` for histogram analysis
- Exported cleaned dataset to `Enhanced_Uber_Fares.csv`

📸 _See screenshots/data_cleaning.png for reference_

---

## 📈 Power BI Analysis

### Key Visualizations:

- **KPI Cards**: Total Rides, Total Fares, Total Duration
- **Histogram**: Fare distribution by fare bins
- **Line Charts**: Ride volume by hour, day, and month
- **Box Plot**: Fare amount vs. hour of day
- **Map**: Geographic pickup distribution using lat/lon
- **Time-Based Analysis**: Duration vs. time patterns

### Filters & Slicers:
- Date range
- Hour of day
- Day of week
- Fare amount range

📸 _See screenshots/dashboard_overview.png_

---

## 📊 DAX Measures (Sample)

```dax
Total Rides = COUNT(Enhanced_Uber_Fares[ride_id])
Total Fares = SUM(Enhanced_Uber_Fares[fare_amount])
Avg Fare per Ride = AVERAGE(Enhanced_Uber_Fares[fare_amount])
```

📁 _Full list in DAX_Formulas.txt_

---

## 🧠 Key Insights

- Peak ride hours: 7–9 AM & 5–8 PM (commute times)
- Highest demand on Fridays and Saturdays
- Downtown areas show ride hotspots


---

## 📝 Recommendations

- Offer ride promotions during low-demand hours
- Optimize driver availability around peak times
- Improve service in high-fare but low-volume zones
- Enhance fare prediction models using hour & location

---

## 📝 Report

🖥️ See `Report_Presentation.pptx` for a complete summary of findings, visuals, and business implications.
 Here on google drive:: https://docs.google.com/presentation/d/1hUAYfDCighcM-XazZJNUL_MxonuryKxV/edit?usp=sharing&ouid=108426038661260792952&rtpof=true&sd=true

---
## PowerBI_Dashboard.pbix
https://drive.google.com/file/d/1JQ_RizyAQLjDe663UKgOylcBmMMBkTPO/view?usp=sharing

## 🔗 Author

**Faisal Shingiro**  
📧 Contact: [faisalshingiro10@gmail.com]  
🎓 Project submitted for: Intro to Big Data Course  
📅 July 2025

---
