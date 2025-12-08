# 📊 Seoul Bike Sharing – Exploratory Data Analysis (EDA)

This project performs an in-depth exploratory data analysis (EDA) on the **Seoul Bike Sharing Dataset** to understand how environmental and temporal factors influence rental demand.

The notebook includes multiple visualizations, each uncovering patterns that help optimize bike availability, pricing, and operational planning.

---

# 📈 Visualizations & Insights (Graph-by-Graph Analysis)

Below is a detailed explanation of **every graph** plotted in the IPYNB notebook.

---

## 1️⃣ Bike Rentals vs Temperature (Bar Plot)

**Code:**  
`plt.bar(df['Temperature(°C)'], df['Rented Bike Count'])`

### 🔍 Insight:
- Rentals increase sharply between **20°C–30°C**.
- Low temperatures → fewer rentals.

### 💡 Implication:
- Increase bike supply during warm days.
- Use dynamic pricing during high-demand weather.

---

## 2️⃣ Bike Rentals per Hour (Bar Plot)

**Code:**  
`plt.bar(df['Hour'], df['Rented Bike Count'])`

### 🔍 Insight:
- Low demand from **0:00–10:00**.
- Peak demand from **10:00–20:00**.

### 💡 Implication:
- Provide morning discounts.
- Ensure maximum bike availability during peak hours.

---

## 3️⃣ Bike Rentals per Date (Bar Plot)

**Code:**  
`plt.bar(df['Date'], df['Rented Bike Count'])`

### 🔍 Insight:
- Daily rentals fluctuate based on weather, holidays, and seasonal conditions.

### 💡 Implication:
- Incorporate seasonal/weather factors in prediction models.

---

## 4️⃣ Rentals vs Dew Point Temperature (Bar Plot)

**Code:**  
`plt.bar(df['Dew point temperature(°C)'], df['Rented Bike Count'])`

### 🔍 Insight:
- High rentals for dew point between **–10°C and 20°C**.
- Very low dew points → discomfort → less demand.

### 💡 Implication:
- Dew point should be included in demand forecasting.

---

## 5️⃣ Dew Point vs Temperature (Line Plot)

**Code:**  
`plt.plot(df['Dew point temperature(°C)'], df['Temperature(°C)'])`

### 🔍 Insight:
- Shows expected relationship between dew point and temperature.

### 💡 Implication:
- Helps multivariate modeling of rider comfort.

---

## 6️⃣ Holiday vs Non-Holiday Rentals (Box Plot)

**Code:**  
`sns.boxplot(x=df['Holiday'], y=df['Rented Bike Count'])`

### 🔍 Insight:
- Rentals are **higher on non-holidays**.
- Holiday rentals show lower variation.

### 💡 Implication:
- Offer holiday-exclusive discounts or passes.

---

## 7️⃣ Holiday Rental Split (Pie Chart)

**Code:**  
`df.groupby("Holiday")["Rented Bike Count"].sum().plot(kind='pie')`

### 🔍 Insight:
- Non-holidays contribute the majority of rentals.

### 💡 Implication:
- Focus promotions on regular weekdays.

---

## 8️⃣ Rentals by Season (Box Plot)

**Code:**  
`sns.boxplot(x=df['Seasons'], y=df['Rented Bike Count'])`

### 🔍 Insight:
- Highest rentals: **Summer & Fall**  
- Lowest rentals: **Winter**

### 💡 Implication:
- Increase fleet capacity during high-demand seasons.
- Prepare winter-ready bikes for cold months.

---

## 9️⃣ Season Contribution (Pie Chart)

**Code:**  
`df.groupby("Seasons")["Rented Bike Count"].sum().plot(kind='pie')`

### 🔍 Insight:
- Summer and Autumn dominate rental share.

---

## 🔟 Snowfall vs Rentals (Scatter Plot)

**Code:**  
`sns.scatterplot(x='Snowfall (cm)', y='Rented Bike Count')`

### 🔍 Insight:
- Even small snowfall drastically reduces rentals.

### 💡 Implication:
- Promote winter gear or suspend service during heavy snowfall.

---

## 1️⃣1️⃣ Rainfall vs Rentals (Scatter Plot)

**Code:**  
`sns.scatterplot(x='Rainfall(mm)', y='Rented Bike Count')`

### 🔍 Insight:
- Rainfall → steady drop in rentals.

### 💡 Implication:
- Offer raincoats/umbrellas or rainy-day discounts.

---

## 1️⃣2️⃣ Visibility vs Rentals (Scatter Plot)

**Code:**  
`sns.scatterplot(x='Visibility (10m)', y='Rented Bike Count')`

### 🔍 Insight:
- Low visibility → fewer rentals due to safety concerns.

### 💡 Implication:
- Provide visibility-enhancing equipment (lights, reflectors).

---

## 1️⃣3️⃣ Humidity vs Rentals (Scatter Plot)

**Code:**  
`sns.scatterplot(x='Humidity(%)', y='Rented Bike Count')`

### 🔍 Insight:
- Optimal rental range: **20%–80% humidity**.
- Extremely high humidity → drop in rentals.

### 💡 Implication:
- Include humidity in demand prediction models.

---

# 🧠 Summary of All Findings

- Weather heavily impacts rental patterns.
- Ideal riding conditions lead to significant demand increases.
- Time of day and seasonality show strong behavioral trends.
- Extreme weather (snow, rain, low visibility) discourages bike usage.

---

# 📁 Notebook

All analysis and visualizations are in:  
`seoul_bike_sharing_eda.ipynb`

---
