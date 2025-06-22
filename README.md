# 🌦️ Weather & AQI Power BI Dashboard using WeatherAPI

This Power BI dashboard provides **real-time weather conditions** and **Air Quality Index (AQI)** for multiple cities using the **WeatherAPI**. It displays temperature, humidity, wind speed, pressure, UV index, precipitation, rain chance, sunrise/sunset timings, and AQI pollutants like PM2.5, CO, SO2, NO2, etc.

> 📊 Built using: Power BI Desktop + WeatherAPI.com

---

## 🚀 Project Overview

This dashboard enables users to:
- 📍 Monitor **current weather conditions** for multiple cities (e.g., Pune, Noida, Surat)
- 📈 Visualize **weekly forecast** trends
- 🌫️ Check **Air Quality Index (AQI)** components with severity color codes
- 🌦️ Estimate **rain chances**, visibility, and UV index
- 🌅 View **sunrise and sunset** timings
- 📌 Switch cities dynamically using slicers

---

## 🔧 Step-by-Step Development Process

### 1️⃣ Get the WeatherAPI Key 🔑

1. Go to [WeatherAPI.com](https://www.weatherapi.com/)
2. Create an account (Free or Paid)
3. Copy your **API key**

---

### 2️⃣ Build the API URL 🌐

Use this template:

```bash
https://api.weatherapi.com/v1/current.json?key=YOUR_API_KEY&q=CITY_NAME&aqi=yes
```

---

### 3️⃣ Connect Power BI to the API 🌍

1. Open **Power BI Desktop**
2. Go to `Home > Get Data > Web`
3. Paste your **WeatherAPI** URL, for example:

```bash
https://api.weatherapi.com/v1/current.json?key=YOUR_API_KEY&q=Pune&aqi=yes
```

4. Click **OK** to load the data

---

### 4️⃣ Transform JSON Data 🛠️

Power BI will open the **Power Query Editor**. Perform the following steps:

- ✅ Expand `current`, `condition`, and `air_quality` objects
- ✏️ Rename columns for clarity
- 📌 Keep only required columns:
  - `temp_c`
  - `humidity`
  - `wind_kph`
  - `uv`
  - `precip_mm`, `vis_km`, etc.
- 🔄 Format data types (e.g., Number, Text, DateTime)
- 💾 Click `Close & Apply` to load into Power BI

---

### 5️⃣ Create Visuals 📊

Use the following visuals in your dashboard:

- 📇 **Cards** → `Temperature`, `Humidity`, `Pressure`, `UV Index`
- 🎯 **Gauges** → `Wind Speed`, `AQI`
- 📈 **Line Chart** → `Forecast temperature` trend
- 📊 **Bar Chart** → `Rain Chances` by day
- 🖼️ **Icons/Images** → Dynamic visuals for current weather condition
- 🔘 **Filters/Slicers** → City Selector, AQI Levels

---

### 🎨 Final Dashboard Highlights

✅ Real-time weather data with API  
✅ Air Quality Index (AQI) using color-coded indicators  
✅ Interactive city-wise comparison  
✅ Forecast & rain probability trends  
✅ Real-time cards for temperature, humidity, wind, UV  
✅ Custom icons for weather types  

---

### 📦 Technologies Used

- 🖥️ **Power BI Desktop**
- 🌐 **WeatherAPI** (`https://www.weatherapi.com/`)
- ⚙️ **Power Query Editor**
- 💡 **DAX (Data Analysis Expressions)**
- 📦 **JSON Data Parsing**

---
