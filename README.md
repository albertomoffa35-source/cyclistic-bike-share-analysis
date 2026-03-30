# 🚴 Cyclistic Bike-Share Analysis
### Google Data Analytics Professional Certificate — Capstone Project

This project is the final case study of the **Google Data Analytics Professional Certificate**.  
It analyzes behavioral differences between casual riders and annual members of Cyclistic, a fictional bike-share company based in Chicago, using real-world trip data from the Divvy Bike Share program.

The goal of the analysis is to generate **data-driven insights** that help the company increase annual memberships.

---

## 📌 Business Problem

Cyclistic offers two types of users:

- **Casual riders** — single rides or day passes
- **Annual members** — yearly subscription users

Annual members are more profitable and provide stable revenue.  
The marketing team wants to understand how casual riders use the service differently in order to design strategies that encourage membership conversion.

### Key Business Question

> How do casual riders and annual members use Cyclistic bikes differently, and how can these insights support marketing decisions to increase memberships?

---

## 🎯 Project Objectives

- Explore user behavior using historical trip data
- Identify usage differences between rider types
- Analyze ride frequency, duration, and temporal patterns
- Transform raw data into actionable business insights
- Provide strategic recommendations supported by analysis

---

## 🛠️ Tools & Technologies

- **Excel**
  - Power Query (data cleaning & transformation)
  - Data Model (large dataset handling)
  - Pivot Tables
  - Dashboard design
- **SQL (Google BigQuery)**
  - Data validation
  - Exploratory queries
- Data Visualization
- Business Analysis & Data Storytelling

---

## 📂 Data Source

Dataset: **Divvy Bike Share Trip Data**

🔗 https://divvy-tripdata.s3.amazonaws.com/index.html

**Location:** Chicago, USA  
**Period analyzed:** March 2025 – February 2026  
**Dataset size:** ~5.6 million rides  
**Format:** Monthly CSV files

The data is anonymized and does not contain personally identifiable information.

---

## 🧹 Data Preparation

Data preparation was performed using **Power Query**:

- Appended 12 monthly datasets into a single table
- Standardized column formats
- Converted timestamps to DateTime
- Removed null and invalid records
- Checked unrealistic ride durations

### Calculated Columns Created

- `ride_length` → trip duration
- `ride_length_minutes` → duration in minutes
- `weekday` → day name extraction
- `weekday_number` → chronological weekday sorting

Due to Excel row limits, data was loaded into the **Excel Data Model**, allowing analysis of all records without sampling.

---

## 🧪 Data Validation with SQL (BigQuery)

SQL queries were used to validate key metrics:

- Total ride count verification
- Ride distribution by user type
- Average ride duration comparison
- Weekly usage pattern analysis

This step simulated real-world workflows combining spreadsheet tools with database environments.

---

## 📊 Dashboard

The dashboard summarizes behavioral differences between casual riders and members.

![Cyclistic Dashboard](dashboard.png)

Key metrics visualized:

- Total rides by user type
- Average ride duration
- Weekly usage patterns
- Bike type preferences

---

## 🔎 Analysis Overview

The analysis focused on identifying behavioral trends that explain how each user type interacts with the service.

### Main Observations

- Members generate a higher number of rides overall.
- Casual riders take longer trips on average.
- Members ride consistently during weekdays.
- Casual riders show strong weekend activity.
- Electric bikes are slightly more popular among casual riders.

These patterns suggest commuting behavior for members and leisure-oriented usage for casual riders.

---

## 📈 Key Findings

### 1️⃣ Members Ride More Frequently
Annual members integrate Cyclistic bikes into daily routines, resulting in higher ride frequency.

### 2️⃣ Casual Riders Take Longer Trips
Longer durations indicate recreational or tourism-related usage.

### 3️⃣ Weekly Usage Patterns Differ
- Members → weekday commuting behavior  
- Casual riders → weekend leisure behavior

### 4️⃣ Conversion Opportunity Exists
Casual riders already engage with the service regularly, making them strong candidates for membership conversion.

---

## 💡 Business Recommendations

Based on the analysis:

- Promote memberships during peak weekend usage.
- Highlight cost savings for frequent casual riders.
- Design marketing campaigns around leisure experiences.
- Optimize bike availability in recreational areas.
- Offer trial memberships to reduce adoption barriers.

---

## ⚠️ Limitations

- No demographic or geographic user data available.
- Weather and seasonal variables not included.
- Analysis based on aggregated behavior rather than individual journeys.

Future work could integrate additional contextual data to enhance predictive insights.

---

## 📄 Full Analytical Report

The complete case study can be found here:

👉 **Project_report.pdf**

---

## 📁 Project Structure
cyclistic-bike-share-analysis
->Cyclistic_Project_Report.pdf
->dashboard.png
->README.md


---

## 👤 Author

**Alberto Moffa**  
Aspiring Data Analyst  

Google Data Analytics Professional Certificate

---

## ⭐ Project Workflow

This project follows the Google Data Analytics process:

**Ask → Prepare → Process → Analyze → Share → Act**

Demonstrating an end-to-end data analysis workflow from raw data to business recommendations.
