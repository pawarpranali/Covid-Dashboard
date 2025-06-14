# COVID-19 Global Dashboard (Tableau)

A dynamic, interactive Tableau dashboard that tracks global COVID-19 cases, deaths, and infections as a percentage of each country’s population—complete with time-series forecasting.

---

## 📊 Overview

- **What it does:**  
  - Shows total cases, total deaths, and overall death rate globally.  
  - Compares death tolls by continent.  
  - Maps percent of population infected per country.  
  - Plots infection trends over time, with a built-in forecast to mid-2021.

- **Why it matters:**  
  Understand the pandemic’s scope at a glance, identify hotspots, and anticipate future infection levels.

---

## 🚀 Getting Started

### Prerequisites

- **Tableau Desktop** (2020.1 or later) _or_ **Tableau Reader** (free)  
- A modern browser if you publish to **Tableau Public**

### Repo Contents

- `COVID19_Global_Dashboard.twbx`  
  Packaged Tableau workbook (includes data extracts)

- `data/owid-covid-data.csv`  
  Raw CSV from Our World in Data

---

## 🔍 Data

- **Source:** Our World in Data COVID-19 dataset  
  (https://github.com/owid/covid-19-data)  
- **Key fields:**  
  - `date`  
  - `location` (country)  
  - `total_cases`, `total_deaths`  
  - `population`  
- **Processing steps:**  
  1. Calculated **Percent Population Infected** = `total_cases / population * 100`  
  2. Applied Tableau’s built-in exponential-smoothing forecast on monthly infection rates.

---

## 📈 Dashboard Components

1. **Global Numbers**  
   Large tiles displaying total cases, total deaths, and death rate.

2. **Total Deaths by Continent**  
   Bar chart ranking continents by cumulative death count.

3. **Infection Map**  
   Choropleth colored by percent of population infected (scale 0–17%+).

4. **Infection Trend & Forecast**  
   Line chart of monthly infection rates for top countries, with forecast shading to August 2021.

---

## 🔧 Launching the Dashboard

1. **Clone** or download this repo.  
2. **Open** `COVID19_Global_Dashboard.twbx` in Tableau Desktop or Reader.  
3. **Go to** the “Dashboard 1” tab.  
4. **Interact:** hover over map regions, zoom the time axis, or filter by country/continent.

---

## 💡 Insights & Next Steps

- **Key insight:**  
  By Dec 2020, the U.S. had infected nearly 9% of its population; forecast by Aug 2021 exceeds 19%.


- **Future enhancements:**  
  - Overlay vaccination rollout data against infection trends.  
  - Add custom date-range filters.  
  - Integrate hospital capacity or testing-rate metrics.


