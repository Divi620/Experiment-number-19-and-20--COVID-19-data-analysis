# 📊 COVID-19 Data Analysis

## 📁 Project Overview
This project performs an in-depth analysis of COVID-19 data to understand the spread, severity, and recovery patterns of the pandemic across different countries and regions. Using time-series analysis and data visualization techniques, the project highlights key trends, growth patterns, and comparative insights.

The dataset contains daily records of confirmed, death, and recovered cases, making it suitable for temporal and geographical analysis.

---

## 🗂️ Dataset Information

- **File Name:** `covid_19_data.csv`
- **Data Type:** Time-series dataset
- **Granularity:** Daily records per country/province

### 📌 Columns Description:
| Column Name        | Description |
|-------------------|------------|
| SNo               | Serial number (unique row ID) |
| ObservationDate   | Date when the data was recorded |
| Province/State    | State or province (nullable) |
| Country/Region    | Country name |
| Last Update       | Timestamp of last update |
| Confirmed         | Total confirmed COVID-19 cases |
| Deaths            | Total deaths reported |
| Recovered         | Total recovered cases |

---

## 🎯 Project Objectives
- Track the global spread of COVID-19 over time  
- Identify the most affected countries and regions  
- Analyze mortality and recovery rates  
- Detect trends such as exponential growth or flattening curves  
- Build meaningful visualizations for better interpretation  

---

## ⚙️ Tech Stack
- **Programming Language:** Python  
- **Libraries Used:**
  - `pandas` – Data cleaning and manipulation  
  - `numpy` – Numerical computations  
  - `matplotlib` – Data visualization  
  - `seaborn` – Advanced visualizations  
- **Environment:** Jupyter Notebook / Google Colab  

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

1. **Date Conversion**
   - Converted `ObservationDate` into datetime format for time-series analysis.

2. **Handling Missing Values**
   - Checked for null values in `Province/State` and filled or ignored where necessary.

3. **Dropping Irrelevant Columns**
   - Removed `SNo` as it does not contribute to analysis.

4. **Aggregation**
   - Grouped data by `Country/Region` and `ObservationDate` to compute totals.

5. **Feature Engineering**
   - Created new columns:
     - Active Cases = Confirmed - Deaths - Recovered  
     - Mortality Rate = Deaths / Confirmed  
     - Recovery Rate = Recovered / Confirmed  

---

## 📊 Exploratory Data Analysis (EDA)

### 🌍 Global Analysis
- Total confirmed cases over time  
- Global death and recovery trends  
- Daily growth rate of cases  

### 🌎 Country-wise Analysis
- Top 10 countries with highest confirmed cases  
- Countries with highest mortality rates  
- Countries with highest recovery rates  

### 📈 Time Series Analysis
- Daily increase in confirmed cases  
- Moving averages (7-day rolling mean)  
- Trend line visualization  

### 📌 Correlation Analysis
- Heatmap showing correlation between:
  - Confirmed
  - Deaths
  - Recovered  

---

## 📉 Data Visualization

The following visualizations were created:

- 📈 Line plots for case trends over time  
- 📊 Bar charts for country comparisons  
- 🔥 Heatmaps for correlation analysis  
- 📉 Rolling average plots for smoothing trends  

---

## 📊 Key Insights

- COVID-19 cases initially showed **exponential growth** before stabilizing in some regions  
- Developed countries reported higher confirmed cases due to better testing  
- Mortality rates varied significantly depending on healthcare infrastructure  
- Recovery rates improved over time due to better treatment protocols  
- Some countries successfully flattened the curve earlier than others  

