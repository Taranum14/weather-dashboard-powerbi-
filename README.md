# weather-dashboard-powerbi-
An interactive, live-connected weather monitoring dashboard built in Power BI, showing real-time conditions, 7-day forecasts, air quality, and climate metrics across multiple cities.

<img width="965" height="547" alt="Screenshot 2026-07-13 004254" src="https://github.com/user-attachments/assets/7dcdc8ae-aa6f-4e27-8d58-be39a3fe62df" />

📌 Overview

This dashboard pulls live data from WeatherAPI.com and presents it in a single, clean, dark-themed view — current conditions, forecast trends, air quality breakdown, and rain probability — so a user can assess weather at a glance without digging through raw numbers.


✨ Features

FeatureDescriptionLive Weather SnapshotCurrent temperature, condition, and last-updated timestampMulti-City SelectorQuick-switch cards to compare cities (Ajmer, Akola, Bengaluru, etc.)7-Day Forecast StripDaily temperature cards, Monday–SundayForecast Trend ChartLine chart visualizing the week's temperature curveSunrise / SunsetDaily sun timing panelAir Quality Index (AQI)Gauge visual with category (Good / Moderate / Poor) + pollutant breakdown (PM2.5, PM10, NO2, SO2, CO, O3)Environmental MetricsVisibility, humidity, precipitation, pressure, wind speed, UV indexChance of RainDay-wise rain probability bar chart


🧠 Power BI Concepts Used


Data Connectivity – Web/API data source connection to WeatherAPI.com (JSON response)
Power Query (M Language) – data shaping: JSON parsing, expanding nested records/lists, unpivoting forecast data, renaming/reordering columns, changing data types
Data Modeling – structuring tables (current weather, forecast, air quality) and defining relationships between them
DAX Measures – calculated metrics such as average/min/max temperature, AQI category logic, rain probability aggregation
DAX Calculated Columns – derived fields like day name, weekday sorting order, temperature category
Conditional Formatting – color-coded values (e.g., AQI status colors, rain probability bar colors)
Card & Multi-Row Card Visuals – current temperature, humidity, pressure, wind speed, UV index tiles
Gauge Visual – Air Quality Index indicator with min/max/target
Line Chart – 7-day forecast temperature trend
Clustered Bar Chart – chance of rain by day
Slicers / Selection Cards – interactive city switcher acting as a filter
Bookmarks & Buttons (if used) – for navigation/interactivity between city views
Custom Tooltips – showing extra detail on hover over chart points
Sort By Column – ensuring days of week display in correct chronological order (not alphabetical)
Theme Customization – custom dark theme, fonts, and color palette for a cohesive UI
Data Refresh / Scheduled Refresh – keeping the report "live" via Power BI Service or gateway refresh
Tooltip Pages (optional, if built) – custom report-page tooltips for richer hover detail

🛠️ Tech Stack

ToolPurposePower BI DesktopDashboard design & visualizationPower Query (M)Data transformation & cleaningDAXCalculated measures & columnsWeatherAPI.comLive weather, forecast & air quality data source

🚀 How to Use


Clone this repository


bash   git clone https://github.com/<your-username>/weather-dashboard-powerbi.git


Open Weather_Dashboard.pbix in Power BI Desktop
Go to Transform Data → Data Source Settings and enter your own WeatherAPI.com key (free tier available)
Click Refresh to pull the latest live data
Use the city selector cards to explore weather across different locations

📊 What This Project Demonstrates


Connecting Power BI to a live external API and shaping real-time JSON data
Writing DAX measures/columns for dynamic categorization and calculations
Designing a clean, dark-themed, card-based UI for at-a-glance readability
Visualizing time-series forecast data with line and bar charts
Combining multiple related data domains (weather + air quality) into one report



🔮 Future Improvements


Historical trend analysis (month-over-month comparisons)
Weather alert notifications
Map visual for multi-city geographic view
Mobile-optimized report layout
Drillthrough page for detailed pollutant analysis
