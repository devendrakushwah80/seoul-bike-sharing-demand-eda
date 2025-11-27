# 🚲 Seoul Bike Sharing Demand – Exploratory Data Analysis

## 📌 Project Overview
This project focuses on **Exploratory Data Analysis (EDA)** of the **Seoul Bike Sharing Demand** dataset obtained from Kaggle.  
The main objective is to understand how **weather conditions, time-based features, and environmental factors** influence bike rental demand.

Through **correlation analysis, heatmaps, and multiple visualizations**, we identify key patterns that affect the total number of bike rentals.

---

## 📂 Dataset Information
- **Source:** Kaggle – Seoul Bike Sharing Demand  
- **Target Variable:** `Rented Bike Count`  
- **Data Type:** Time-series + Weather data  
- **Time Period:** Hourly data across multiple dates  

### Key Features
- Temperature (°C)  
- Dew Point Temperature (°C)  
- Humidity (%)  
- Wind Speed (m/s)  
- Visibility (10m)  
- Solar Radiation  
- Rainfall (mm)  
- Snowfall (cm)  
- Hour  
- Date  
- Seasons & Holidays  

---

## 🔍 Exploratory Data Analysis (EDA)

The EDA process includes:
- Data cleaning and formatting  
- Feature understanding  
- Correlation analysis  
- Heatmap visualization  
- Trend analysis using line and bar plots  

---

## 📊 Key Insights & Findings

### 1️⃣ Correlation & Heatmap Analysis
- **Temperature (°C)** has a strong positive correlation with total bike rentals.  
- **Dew Point Temperature (°C)** also shows a positive relationship with rentals, indicating higher usage during comfortable weather.  
- **Humidity (%)** is negatively correlated, meaning higher humidity reduces bike usage.  
- **Rainfall and Snowfall** have a negative impact on bike demand.  
- **Visibility and Solar Radiation** show a mild positive influence on rentals.  

✅ The heatmap clearly highlights which features most strongly influence bike rental demand.

---

### 2️⃣ Total Bike Rentals vs Temperature
- Bike rentals increase consistently with rising temperature.  
- Very low temperatures result in minimal rentals.  
- Moderate to warm temperatures are ideal for high bike usage.  

📈 **Insight:** Weather comfort plays a crucial role in bike-sharing demand.

---

### 3️⃣ Total Bike Rentals vs Dew Point Temperature (°C)
- Higher dew point temperatures (indicating moist but warm air) correlate with increased rentals.  
- Extremely low dew point values correspond with fewer rentals.  

📌 **Insight:** Dew point temperature is an overlooked but meaningful indicator of rental demand.

---

### 4️⃣ Total Bike Rentals per Hour
- A clear daily usage pattern is observed.  
- **Peak demand hours:**
  - Morning: **7–9 AM** (office commute)
  - Evening: **5–8 PM** (return commute)
- Lowest demand occurs during late night and early dawn hours.

⏰ **Insight:** Bike rentals are heavily influenced by working hours and commuting patterns.

---

### 5️⃣ Total Bike Rentals per Date
- Bike rentals vary seasonally across different dates.  
- Higher rentals occur during warmer months.  
- Lower demand is observed during winter and adverse weather periods.

📆 **Insight:** Bike usage follows strong seasonal trends.

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## 📈 Conclusion
- Weather variables, especially **Temperature and Dew Point Temperature**, have a significant impact on bike rental demand.  
- Time-based features such as **Hour and Date** reveal strong commuting and seasonal patterns.  
- Exploratory Data Analysis and correlation techniques provide valuable insights before building predictive models.

---

## ✅ Future Scope
- Feature engineering for improved prediction  
- Machine learning and regression modeling  
- Time-series forecasting for bike demand
