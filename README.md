# 🌦️ Live Weather Dashboard — Power BI Project

An interactive, live-connected weather monitoring dashboard built in **Power BI**, showing real-time conditions, 7-day forecasts, air quality, and climate metrics across multiple cities.

<img width="923" height="520" alt="Screenshot 2026-07-13 005332" src="https://github.com/user-attachments/assets/34d52c31-297d-4b41-a1dd-b1e9e9b8c536" />



---

## 📌 Overview

This dashboard pulls live data from **WeatherAPI.com** and presents it in a single, clean, dark-themed view — current conditions, forecast trends, air quality breakdown, and rain probability — so a user can assess weather at a glance without digging through raw numbers.

---

## ✨ Features

| Feature | Description |
|---|---|
| **Live Weather Snapshot** | Current temperature, condition, and last-updated timestamp |
| **Multi-City Selector** | Quick-switch cards to compare cities (Ajmer, Akola, Bengaluru, etc.) |
| **7-Day Forecast Strip** | Daily temperature cards, Monday–Sunday |
| **Forecast Trend Chart** | Line chart visualizing the week's temperature curve |
| **Sunrise / Sunset** | Daily sun timing panel |
| **Air Quality Index (AQI)** | Gauge visual with category (Good / Moderate / Poor) + pollutant breakdown (PM2.5, PM10, NO2, SO2, CO, O3) |
| **Environmental Metrics** | Visibility, humidity, precipitation, pressure, wind speed, UV index |
| **Chance of Rain** | Day-wise rain probability bar chart |

---

## 🧠 Power BI Concepts Used

- **Data Connectivity** – Web/API data source connection to WeatherAPI.com (JSON response)
- **Power Query (M Language)** – JSON parsing, expanding nested records/lists, unpivoting forecast data, renaming/reordering columns, changing data types
- **Data Modeling** – structuring tables (current weather, forecast, air quality) and defining relationships between them
- **DAX Measures** – average/min/max temperature, AQI category logic, rain probability aggregation
- **DAX Calculated Columns** – day name, weekday sorting order, temperature category
- **Conditional Formatting** – color-coded values (e.g., AQI status colors, rain probability bar colors)
- **Card & Multi-Row Card Visuals** – current temperature, humidity, pressure, wind speed, UV index tiles
- **Gauge Visual** – Air Quality Index indicator with min/max/target
- **Line Chart** – 7-day forecast temperature trend
- **Clustered Bar Chart** – chance of rain by day
- **Slicers / Selection Cards** – interactive city switcher acting as a filter
- **Bookmarks & Buttons** *(if used)* – navigation/interactivity between city views
- **Custom Tooltips** – extra detail on hover over chart points
- **Sort By Column** – ensuring days of week display in correct chronological order (not alphabetical)
- **Theme Customization** – custom dark theme, fonts, and color palette
- **Data Refresh / Scheduled Refresh** – keeping the report "live" via Power BI Service or gateway refresh
- **Tooltip Pages** *(optional, if built)* – custom report-page tooltips for richer hover detail

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design & visualization |
| **Power Query (M)** | Data transformation & cleaning |
| **DAX** | Calculated measures & columns |
| **[WeatherAPI.com](https://www.weatherapi.com/)** | Live weather, forecast & air quality data source |
| **Power BI Service** *(optional)* | Publishing & scheduled refresh |


---

## 🚀 How to Use

1. Clone this repository
```bash
   git clone https://github.com/<your-username>/weather-dashboard-powerbi.git
```
2. Open `Weather_Dashboard.pbix` in **Power BI Desktop**
3. Go to **Transform Data → Data Source Settings** and enter your own [WeatherAPI.com](https://www.weatherapi.com/) key (free tier available)
4. Click **Refresh** to pull the latest live data
5. Use the city selector cards to explore weather across different locations



---

## 📊 What This Project Demonstrates

- Connecting Power BI to a **live external API** and shaping real-time JSON data
- Writing **DAX measures/columns** for dynamic categorization and calculations
- Designing a clean, **dark-themed, card-based UI** for at-a-glance readability
- Visualizing **time-series forecast data** with line and bar charts
- Combining multiple related data domains (weather + air quality) into one report

---

## 🔮 Future Improvements

- Historical trend analysis (month-over-month comparisons)
- Weather alert notifications
- Map visual for multi-city geographic view
- Mobile-optimized report layout
- Drillthrough page for detailed pollutant analysis

---
