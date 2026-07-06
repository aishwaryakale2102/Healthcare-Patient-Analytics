# Healthcare Patient Analytics Dashboard

## Project Overview

The Healthcare Patient Analytics Dashboard is a comprehensive healthcare analytics project developed using Python, SQL, and Power BI. The project focuses on analyzing patient healthcare data to identify trends, monitor patient health conditions, and generate meaningful business and healthcare insights through interactive dashboards and visualizations.

This project demonstrates end-to-end data analytics workflow including:
- Data generation and preprocessing
- Data cleaning and transformation
- Exploratory Data Analysis (EDA)
- SQL database analysis
- DAX calculations
- Power BI dashboard development
- Data storytelling and KPI reporting

The dashboard helps healthcare organizations analyze patient demographics, disease patterns, BMI trends, blood pressure analysis, cholesterol analysis, and treatment plans to support data-driven healthcare decisions.

---

# Problem Statement

Healthcare organizations manage large amounts of patient data daily. Analyzing this data manually becomes difficult and inefficient, especially when identifying disease trends, patient demographics, health indicators, and treatment patterns.

This project aims to build an interactive healthcare analytics dashboard that enables healthcare professionals and analysts to:
- Monitor patient statistics
- Analyze disease distribution
- Track health indicators
- Improve healthcare reporting
- Generate operational insights

---

# Objectives

- Analyze healthcare patient records
- Perform data cleaning and preprocessing
- Conduct exploratory data analysis
- Build SQL-based healthcare analysis queries
- Create interactive Power BI dashboards
- Generate KPI metrics and healthcare insights
- Visualize patient health trends

---

# Tools & Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Data generation & preprocessing |
| Pandas | Data manipulation |
| Matplotlib | Data visualization |
| SQLite | SQL database analysis |
| SQL | Data querying |
| Power BI | Dashboard development |
| DAX | KPI calculations |

---

# Dataset Description

The dataset contains synthetic healthcare patient records with the following features:

| Column Name | Description |
|-------------|-------------|
| Patient_ID | Unique patient identifier |
| Age | Patient age |
| Gender | Patient gender |
| Diagnosis | Disease/health condition |
| BMI | Body Mass Index |
| Blood_Pressure | Blood pressure reading |
| Heart_Rate | Heart rate value |
| Cholesterol_Level | Cholesterol measurement |
| Treatment_Plan | Assigned treatment |
| Follow_Up_Date | Patient follow-up date |

Additional business-related fields were added for analytics purposes:
- Facility_ID
- Dialysis_Station_ID
- Billing Analysis
- Patient Statistics

---

# Project Workflow

## 1. Dataset Creation
A synthetic healthcare dataset was generated using Python libraries such as:
- Pandas
- NumPy
- Random

---

## 2. Data Cleaning

The following preprocessing steps were performed:

- Removed duplicate records
- Handled missing values
- Converted data types
- Standardized categorical values
- Validated numerical columns
- Prepared data for SQL and Power BI analysis

---

# Python Data Cleaning Example

```python
df.drop_duplicates(inplace=True)

df['Treatment_Plan'].fillna(
    'Unknown',
    inplace=True
)

df['Gender'] = df['Gender'].str.title()
```

---

# Exploratory Data Analysis (EDA)

The following analyses were performed:

- Age distribution analysis
- Disease distribution analysis
- Gender analysis
- BMI trend analysis
- Blood pressure analysis
- Cholesterol analysis

---

# SQL Analysis

SQLite database was connected with Python to perform SQL analysis on healthcare data.

## SQL Queries Performed

### Total Patients

```sql
SELECT COUNT(*) AS Total_Patients
FROM patients;
```

### Disease Distribution

```sql
SELECT
    Diagnosis,
    COUNT(*) AS Patient_Count
FROM patients
GROUP BY Diagnosis;
```

### Average BMI

```sql
SELECT
    AVG(BMI) AS Average_BMI
FROM patients;
```

### Blood Pressure Analysis

```sql
SELECT
    Diagnosis,
    AVG(Blood_Pressure) AS Avg_BP
FROM patients
GROUP BY Diagnosis;
```

---

# Power BI Dashboard

An interactive Power BI dashboard was developed to visualize healthcare insights.

## Dashboard Components

### KPI Cards
- Total Patients
- Average Age
- Average BMI
- Diagnosis Count

### Charts & Visualizations
- Disease Distribution Chart
- Gender Distribution Pie Chart
- BMI Trend Analysis
- Blood Pressure Analysis
- Cholesterol Analysis

### Interactive Features
- Diagnosis slicer
- Gender slicer
- Treatment Plan slicer

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

## Male Patients

```DAX
Male_Patients =
CALCULATE(
    COUNTROWS('healthcare_dataset'),
    'healthcare_dataset'[Gender] = "Male"
)
```

---

# Dashboard Insights

The dashboard generated the following healthcare insights:

- Hypertension and Hyperlipidemia were among the most common diagnoses.
- Male patients represented a slightly higher proportion of total healthcare cases.
- Higher BMI values showed correlation with elevated blood pressure.
- Diabetes patients demonstrated increased cholesterol levels.
- Certain treatment plans were more frequently assigned to chronic patients.

---

# Dashboard Design

The dashboard was designed using:
- Professional healthcare color palette
- KPI-focused layout
- Interactive filters
- Clean visual hierarchy
- Responsive chart arrangement

---

# Project Structure

```bash
Healthcare-Patient-Analytics/
│
├── healthcare_dataset.csv
├── cleaned_healthcare_dataset.csv
├── healthcare_analysis.db
├── healthcare_dashboard.pbix
├── healthcare_analysis.ipynb
├── SQL_queries.sql
├── images/
└── README.md
```

---

# Key Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- SQL Query Writing
- Database Integration
- DAX Calculations
- Power BI Dashboarding
- Data Visualization
- KPI Reporting
- Business Intelligence
- Healthcare Analytics

---

# Future Enhancements

Future improvements planned for this project include:

- Machine Learning integration
- Patient risk prediction
- Real-time healthcare analytics
- Streamlit deployment
- Cloud database integration
- Advanced healthcare KPIs
- Predictive healthcare insights

---

# Conclusion

This project demonstrates a complete healthcare analytics workflow using Python, SQL, and Power BI. It highlights the ability to clean, analyze, visualize, and generate insights from healthcare patient data while building interactive dashboards for business intelligence and healthcare decision-making.

The project strengthens practical skills in:
- Data Analytics
- Healthcare Domain Analysis
- SQL
- Power BI
- Dashboard Development
- Business Intelligence

---

# Author

## Aishwarya Kale

B.Tech Artificial Intelligence & Data Science

---
