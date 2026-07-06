# Healthcare Patient Analytics Dashboard

## Project Overview

The Healthcare Patient Analytics Dashboard is a data analytics and visualization project developed using Python and Power BI. The project focuses on analyzing healthcare patient data to identify disease patterns, patient demographics, BMI trends, blood pressure analysis, cholesterol analysis, and treatment insights through interactive dashboards.

This project demonstrates an end-to-end analytics workflow including:
- Dataset generation
- Data cleaning
- Exploratory Data Analysis (EDA)
- KPI analysis
- DAX calculations
- Interactive Power BI dashboard development

---

# Problem Statement

Healthcare organizations generate large amounts of patient data daily. Analyzing this data manually becomes difficult and time-consuming. This project aims to build an interactive healthcare analytics dashboard to monitor patient statistics, identify disease trends, and generate healthcare insights for better decision-making.

---

# Objectives

- Analyze healthcare patient records
- Perform data cleaning and preprocessing
- Conduct exploratory data analysis
- Create KPI metrics using DAX
- Build interactive Power BI dashboards
- Visualize healthcare trends and insights

---

# Tools & Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Data preprocessing |
| Pandas | Data manipulation |
| NumPy | Dataset generation |
| Matplotlib | Data visualization |
| Power BI | Dashboard development |
| DAX | KPI calculations |

---

# Dataset Features

The dataset contains healthcare patient information including:

| Column Name | Description |
|-------------|-------------|
| Patient_ID | Unique patient identifier |
| Age | Patient age |
| Gender | Patient gender |
| Diagnosis | Patient diagnosis |
| BMI | Body Mass Index |
| Blood_Pressure | Blood pressure reading |
| Heart_Rate | Heart rate value |
| Cholesterol_Level | Cholesterol measurement |
| Treatment_Plan | Assigned treatment |
| Follow_Up_Date | Follow-up appointment date |

---

# Project Workflow

## 1. Dataset Creation
Generated a synthetic healthcare dataset using Python libraries.

## 2. Data Cleaning
Performed:
- Duplicate removal
- Missing value handling
- Data formatting
- Column validation

## 3. Exploratory Data Analysis (EDA)
Analyzed:
- Disease distribution
- Gender distribution
- BMI trends
- Blood pressure analysis
- Cholesterol analysis

## 4. Power BI Dashboard Development
Created an interactive healthcare dashboard using:
- KPI cards
- Pie charts
- Bar charts
- Line charts
- Slicers and filters

---

# DAX Measures Used

## Total Patients

```DAX
Total_Patients =
COUNTROWS('healthcare_dataset')
```

## Average Age

```DAX
Average_Age =
AVERAGE('healthcare_dataset'[Age])
```

## Average BMI

```DAX
Average_BMI =
AVERAGE('healthcare_dataset'[BMI])
```

## Diagnosis Count

```DAX
Diagnosis_Count =
DISTINCTCOUNT('healthcare_dataset'[Diagnosis])
```

---

# Dashboard Features

- Total Patients KPI
- Average Age KPI
- Average BMI KPI
- Diagnosis Analysis
- Disease Distribution
- Gender Distribution
- Blood Pressure Analysis
- BMI Trend Analysis
- Interactive Filters & Slicers

---

# Key Insights

- Hypertension and Hyperlipidemia were among the most common diagnoses.
- Male patients represented a slightly higher percentage of total cases.
- Higher BMI values were associated with increased blood pressure levels.
- Diabetes patients showed elevated cholesterol measurements compared to healthy patients.

---

# Dashboard Design

The dashboard was designed using:
- Healthcare-themed color palette
- KPI-focused layout
- Interactive filtering
- Clean visual hierarchy
- Professional dashboard formatting

---

# Project Structure

```bash
Healthcare-Patient-Analytics/
│
├── healthcare_dataset.csv
├── healthcare_dashboard.pbix
├── healthcare_analysis.ipynb
├── screenshots/
└── README.md
```

---

# Key Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Power BI Dashboarding
- DAX Calculations
- KPI Reporting
- Data Visualization
- Healthcare Analytics
- Business Intelligence

---

# Future Improvements

Future enhancements planned:
- SQL integration
- Real-time healthcare data
- Machine Learning predictions
- Patient risk analysis
- Streamlit deployment
- Advanced healthcare KPIs

---

# Conclusion

This project demonstrates a complete healthcare analytics workflow using Python and Power BI. It highlights practical skills in data cleaning, analysis, visualization, KPI development, and dashboard creation for healthcare analytics and business intelligence applications.

---

# Author

## Aishwarya Kale

B.Tech Artificial Intelligence & Data Science
