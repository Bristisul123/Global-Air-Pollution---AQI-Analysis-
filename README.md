# 🌍 Global Air Pollution Analysis — Power BI

An interactive **air pollution analysis dashboard** built to explore air quality patterns across countries and cities worldwide, evaluating AQI severity, pollutant composition, and regional distribution to support environmental awareness and data-driven insight.

The project follows a **data cleaning and dashboard development workflow**, starting with a raw global air quality dataset, followed by data cleaning and preparation, and an interactive **Power BI dashboard**.

The analysis evaluates AQI (Air Quality Index) levels, dominant pollutant types, country and city rankings, and regional distribution to help identify the most polluted areas and the primary pollutants driving poor air quality.

---

## 📊 Dashboard Overview

An interactive **Power BI dashboard** was developed to provide a comprehensive overview of global air pollution levels, pollutant breakdowns, and country/city rankings.

### 📸 Dashboard Preview

![Air Pollution Dashboard](https://github.com/Bristisul123/Global-Air-Pollution---AQI-Analysis-/blob/main/Air%20Pollution%20Dashboard.png?raw=true)

The Power BI dashboard provides an interactive view of key air quality metrics through KPI cards, country rankings, pollutant comparisons, regional distribution, and geographic visualizations.

### 📌 Dashboard KPIs

- **Total Countries**
- **Average AQI**
- **Highest AQI**
- **Lowest AQI**
- **Average PM2.5**
- **Average CO**

---

## ❓ Business Questions

The analysis was designed to answer the following questions:

- Which countries and cities have the worst air quality?
- What is the average AQI globally, and how does it vary by country?
- Which pollutant (PM2.5, CO, NO2, Ozone) is most responsible for poor air quality in a given city or country?
- How is air quality distributed across AQI categories (Good, Moderate, Unhealthy, Very Unhealthy, Hazardous)?
- How does air quality vary across regions/continents?
- Are there countries where pollution is concentrated in a specific pollutant rather than spread evenly?
- Which cities require the most urgent air quality intervention?

---

## 🔄 Project Pipeline

### 1. Raw Dataset

The project started with a **global air pollution dataset** (`global_air_pollution_data.csv`) containing city-level air quality records across 175 countries.

The dataset contains information related to:

- Country and city identifiers
- Overall AQI value and category
- CO AQI value and category
- Ozone AQI value and category
- NO2 AQI value and category
- PM2.5 AQI value and category

### 2. Data Cleaning & Preparation

Before building the dashboard, the dataset was cleaned and prepared, including:

- Removing/correcting malformed column headers (e.g. stray whitespace in `co_aqi_value`)
- Handling missing or blank country values
- Standardizing AQI category labels
- Validating numeric AQI fields
- Preparing the dataset for use in Power BI

### 3. Power BI — Dashboard Development

The cleaned data was imported into **Power BI** to build an interactive dashboard.

The report includes:

- KPI cards summarizing global air quality
- Country and city AQI rankings
- Pollutant comparison by country/region
- AQI category distribution (donut/pie)
- Dominant pollutant breakdown
- Geographic map of AQI by location
- Interactive filters and slicers (city, country, AQI category)

---

## 🗂️ Data Dictionary

### `global_air_pollution_data`

| Column | Description |
|--------|-------------|
| `country_name` | Country where the city is located |
| `city_name` | City name |
| `aqi_value` | Overall Air Quality Index value |
| `aqi_category` | Overall AQI severity category (Good, Moderate, Unhealthy, etc.) |
| `co_aqi_value` | Carbon monoxide AQI value |
| `co_aqi_category` | Carbon monoxide AQI category |
| `ozone_aqi_value` | Ozone AQI value |
| `ozone_aqi_category` | Ozone AQI category |
| `no2_aqi_value` | Nitrogen dioxide AQI value |
| `no2_aqi_category` | Nitrogen dioxide AQI category |
| `pm2.5_aqi_value` | PM2.5 AQI value |
| `pm2.5_aqi_category` | PM2.5 AQI category |

---

## 📊 Dashboard Features

- **Total Countries / Average AQI / Highest AQI / Lowest AQI / Average PM2.5 / Average CO KPIs**
- Top 10 countries by AQI
- AQI category distribution (Good, Moderate, Unhealthy, Very Unhealthy, Hazardous)
- Pollutant comparison across top countries (PM2.5, CO, Ozone, NO2)
- Dominant pollutant per city
- Regional distribution
- Geographic map of AQI by city
- Interactive filtering by country, city, and AQI category

---

## 📈 Key Metrics

### AQI Category Share

```text
AQI Category % = Cities in Category / Total Cities
```

### Dominant Pollutant

```text
Dominant Pollutant = Pollutant with the highest AQI value among PM2.5, CO, NO2, Ozone for a given city
```

These metrics provide a consistent framework for comparing pollution severity and pollutant composition across cities and countries.

---

## 💡 Key Insights

> Replace the placeholders below with your own findings once the dashboard is finalized.

- **[X]% of cities fall into the "Good" AQI category**, while **[X]%** fall into "Moderate," indicating [your interpretation].
- **PM2.5 is the dominant pollutant** in the majority of unhealthy-AQI cities, suggesting [your interpretation — e.g. traffic/industrial emissions].
- The most polluted countries by average AQI are **[Country 1, Country 2, Country 3]**.
- [Add any other pattern you noticed — e.g. regional concentration, pollutant-specific outliers, etc.]

---

## 🛠️ Tools & Technologies

- **Power BI**
- **DAX**
- **Excel / Power Query** (data cleaning)

---

## 📁 Project Structure

```text
Global Air Pollution Analysis/
│
├── README.md
│
├── data/
│   └── global_air_pollution_data.csv
│
├── powerbi/
│   └── air_pollution_dashboard.pbix
│
└── screenshots/
    └── dashboard_preview.png
```

---

## 🎯 Project Goal

The primary goal of this project is to build an interactive **Power BI dashboard** for exploring global air quality, identifying the most polluted regions, and understanding which pollutants drive poor air quality in different parts of the world.

### Project Workflow

```text
Raw Air Pollution Dataset
        ↓
Data Cleaning & Preparation
        ↓
Column & Category Standardization
        ↓
AQI Category & Dominant Pollutant Calculation
        ↓
Power BI Dashboard Development
        ↓
Air Quality Insights
```

Overall, the project demonstrates how **Power BI and DAX** can be used to transform raw environmental data into an accessible, interactive tool for understanding global air quality.
