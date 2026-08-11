# 📱 Bellabeat Smart Device Usage Analysis

## 📌 Project Overview

This project is a data analytics case study focused on analyzing Fitbit smart-device usage data to understand patterns in users' activity, sedentary behavior, hourly movement, and sleep.

The objective is to use these insights to develop data-driven marketing recommendations for Bellabeat and improve user engagement with its wellness products.

---

## 🎯 Business Problem

Bellabeat wants to understand how consumers use smart wellness devices and identify behavioral trends that could help inform its marketing strategy.

### Business Question

> What are some trends in smart-device usage, and how can these trends be used to develop marketing strategies for Bellabeat?

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Power BI
- DAX
- Jupyter Notebook
- GitHub

---

## 📂 Dataset

- **Source:** Fitbit Fitness Tracker Data – Kaggle
- **Period Covered:** April 12, 2016 – May 12, 2016
- **Original Files:** 18 CSV files
- **Core Datasets Used:** 4
- **Derived Dataset:** Activity & Sleep Analysis

### Selected Datasets

- `dailyActivity_merged.csv`
- `sleepDay_merged.csv`
- `hourlySteps_merged.csv`
- `hourlyIntensities_merged.csv`

### Derived Dataset

- `activity_sleep_analysis.csv`

The derived dataset was created by combining daily activity and sleep observations using user ID and date.

---

## ⚙️ Data Preparation

- Loaded and inspected the Fitbit datasets using Pandas.
- Checked data types, missing values, duplicates, and unique users.
- Converted date columns to datetime format.
- Created Day of Week variables.
- Created Total Sleep Hours and Time in Bed Hours.
- Created Total Active Minutes.
- Categorized activity records into Low, Moderate, and High activity levels.
- Removed three duplicate sleep records.
- Combined activity and sleep data for correlation analysis.
- Exported cleaned datasets for Power BI.

---

## 📊 Dashboard 1 – User Activity & Behavior

### Included Metrics

- Average Daily Steps
- Average Calories
- Average Active Minutes
- Average Sleep Duration

### Visualizations

- Activity Level Distribution
- Average Daily Steps by Day of Week
- Average Hourly Steps

### Key Insight

Activity peaked around **6 PM**, with the **5–7 PM period** showing the highest recorded hourly step activity.

### Dashboard Preview

<img width="1470" height="956" alt="User Activity & Behavior" src="screenshots/Screenshot 2026-08-11 143209.png" />

<p align="center">
  <b>Figure 1.</b> User Activity & Behavior Dashboard
</p>

---

## 📈 Dashboard 2 – Sleep & Wellness Insights

### Included Metrics

- Average Sleep Duration
- Average Time in Bed

### Visualizations

- Average Sleep Duration by Day of Week
- Daily Steps vs Sleep Duration
- Correlation Analysis

### Key Insight

Daily steps and sleep duration showed a **weak negative association (r = -0.19)**, indicating little meaningful linear relationship in the observed sample.

### Dashboard Preview

<img width="1470" height="956" alt="Sleep & Wellness Insights" src="screenshots/Screenshot 2026-08-11 143447.png" />

<p align="center">
  <b>Figure 2.</b> Sleep & Wellness Insights Dashboard
</p>

---

## 🔍 Key Findings

- Users recorded an average of approximately **7,638 daily steps**.
- Average sedentary time was approximately **991 minutes per day**.
- High-activity days averaged approximately **13,337 steps**, compared with **2,128 steps** on low-activity days.
- Low-activity days recorded approximately **244 more sedentary minutes** than high-activity days.
- Activity peaked around **6 PM**.
- **Saturday** recorded the highest average daily steps at approximately **8,153**.
- **Sunday** recorded the lowest average daily steps at approximately **6,933**.
- Average sleep duration was approximately **6.99 hours**.
- **Sunday** had the highest average sleep duration at approximately **7.55 hours**.
- **Thursday** had the lowest average sleep duration at approximately **6.69 hours**.
- Steps and sleep showed a weak negative correlation of **-0.19**.
- Activity levels were relatively evenly distributed:
  - Moderate: **35.53%**
  - High: **32.23%**
  - Low: **32.23%**

---

## 💡 Business Recommendations

### 1. Launch Time-Based Evening Activity Engagement

Use the observed **5–7 PM activity window** to test personalized engagement through:

- Activity reminders
- Progress updates
- Movement prompts
- Wellness content

The 6 PM peak should be treated as a testable opportunity rather than assuming every user has the same activity schedule.

### 2. Target Low-Activity and High-Sedentary Users

Use behavioral segmentation to identify users who repeatedly demonstrate low activity and high sedentary behavior.

Potential engagement strategies include:

- Personalized movement reminders
- Activity challenges
- Progress tracking
- Personalized wellness content

### 3. Increase Sleep & Wellness Engagement

Use the observed weekday variation in sleep to support:

- Personalized sleep insights
- Weekly wellness summaries
- Sleep-awareness content
- Routine-building prompts
- Sleep-focused educational content

This could help position Bellabeat as a broader wellness platform rather than focusing only on physical activity.

---

## 📊 Key Metrics

| Metric | Result |
|---|---:|
| Average Daily Steps | **7,638** |
| Average Calories | **2,304** |
| Average Sedentary Minutes | **991** |
| Average Active Minutes | **227.54** |
| Average Sleep Duration | **6.99 hours** |
| Average Time in Bed | **7.64 hours** |
| Peak Activity Hour | **6 PM** |
| Steps vs Sleep Correlation | **-0.19** |

---

## 📄 Project Workflow

1. Ask
2. Prepare
3. Process
4. Analyze
5. Share
6. Act

---

## ⚠️ Limitations

- The dataset represents a relatively small Fitbit user sample.
- The observation period covers approximately one month.
- Sleep data is available for fewer users than activity data.
- The dataset is from 2016 and may not represent current smart-device usage behavior.
- Fitbit users may not represent Bellabeat's target customers.
- The analysis identifies associations rather than causal relationships.
- The findings should be treated as directional insights rather than definitive statements about Bellabeat customers.

---

## 📑 Project Report

The detailed case study report containing the analysis, findings, dashboard documentation, and marketing recommendations is available here:

[View the Bellabeat Case Study Report](report/bellabeat_Smart_Device_Usage_report.pdf)

---

## 📁 Repository Structure

```text
Bellabeat-Smart-Device-Analysis/
│
├── README.md
│
├── data/
│   ├── dailyActivity_cleaned.csv
│   ├── sleepDay_cleaned.csv
│   ├── hourlySteps_cleaned.csv
│   ├── hourlyIntensities_cleaned.csv
│   └── activity_sleep_analysis.csv
│
├── notebooks/
│   └── bellabeat_analysis.ipynb
│
├── powerbi/
│   └── Bellabeat_Dashboard.pbix
│
├── report/
│   └── Bellabeat_Smart_Device_Usage_Analysis_Report.docx
│
└── screenshots/
    ├── dashboard_page1.png
    └── dashboard_page2.png
