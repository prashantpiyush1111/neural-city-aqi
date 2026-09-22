# 🏙️ Neural City AQI Dashboard

> A data-driven dashboard prototype that combines Indian city AQI data with street-level liveability signals to reveal gaps between infrastructure and air quality.

## 📌 Overview

This project was built for the **Neural City Full-Stack Product Engineering Internship Assignment**.

The dashboard combines Neural City's city-ranking context with **CPCB Annual AQI 2023** data to help compare urban liveability from two perspectives: the quality of the built environment and air quality.

🔗 **Live Demo:** [neural-city-aqi](https://prashantpiyush1111.github.io/neural-city-aqi)

## 🎯 Problem

A city may appear highly liveable based on roads, footpaths, cleanliness, walkability, and mobility, while still having poor air quality.

This prototype surfaces that hidden gap by bringing the two dimensions together in one visual interface.

## 📊 Data Pipeline

```text
CPCB Annual AQI 2023
        ↓
Filter relevant cities
        ↓
Clean & normalize city names
        ↓
Aggregate valid station/day readings
        ↓
City-level annual AQI
        ↓
Dashboard visualizations
```

### Data Cleaning

1. Filter to cities included in the relevant city-ranking set
2. Exclude cities with fewer than 180 valid AQI-reading days
3. Aggregate station-level readings to annual city averages
4. Normalize naming differences such as `Bengaluru` / `Bangalore`
5. Export clean data with city, state, annual average AQI, and category fields

## 🧭 Use Cases

| Audience | Use Case |
|---|---|
| Municipal teams | Identify cities with strong infrastructure but poor air quality |
| Citizens | Compare liveability signals before relocation |
| Urban planners | Combine infrastructure and AQI signals when prioritizing interventions |
| Analysts | Compare cities across multiple quality-of-life dimensions |

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Chart.js
- CPCB open data

## 📁 Project Structure

```text
neural-city-aqi/
├── index.html      # Dashboard application
└── README.md       # Project documentation
```

## 🚀 Run Locally

Clone the repository:

```bash
git clone https://github.com/prashantpiyush1111/neural-city-aqi.git
cd neural-city-aqi
```

Open `index.html` directly in a browser, or serve the project with a simple local HTTP server.

## 🌐 Live Demo

[Open the deployed dashboard](https://prashantpiyush1111.github.io/neural-city-aqi)

## 👨‍💻 Author

**Prashant Maurya**  
Full-Stack Developer

## 📄 License

See the repository license for current usage terms.
