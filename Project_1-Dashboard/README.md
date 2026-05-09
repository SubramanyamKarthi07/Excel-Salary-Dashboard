# 📊 Excel Salary Dashboard
## 📌 Project Overview

This project is an interactive Excel dashboard designed to analyze global data science salaries. It helps users explore salary trends by job title, country, and employment type.

The dashboard was built using advanced Excel formulas, charts, and data validation techniques to provide dynamic insights from real-world 2023 job market data.

---

## 🎯 Objectives

- Analyze salary trends across data-related roles.
- Compare salaries by country.
- Explore differences by employment type.
- Build an interactive dashboard using Excel.

---

## 🛠️ Excel Skills Used

- Charts and Visualizations
- MEDIAN Formula
- FILTER Function
- IF Statements
- SEARCH Function
- Data Validation
- Dynamic Drop-down Lists

---

## 📂 Dataset Information

The dataset contains real-world 2023 data science job postings, including:

- Job Title
- Average Salary
- Country
- Employment Type
- Required Skills

---

## 📈 Dashboard Features

### 1. Salary by Job Title
A horizontal bar chart comparing median salaries for major data roles.

### 2. Country Salary Map
A global map showing salary differences across countries.

### 3. Dynamic Filters
Users can filter the dashboard by:
- Job Title
- Country
- Employment Type

---

## 🔍 Key Insights

- Senior roles such as Data Engineer and Senior Data Scientist earn the highest salaries.
- Salaries vary significantly by country.
- Full-time positions dominate the dataset.

---

## 🧮 Example Formula Used

```excel
=MEDIAN(IF((jobs[job_title_short]=A2)*(jobs[job_country]=country)*(ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*(jobs[salary_year_avg]<>0),jobs[salary_year_avg]))