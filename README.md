# Neural City AQI Dashboard 🏙️

A prototype built for the **Neural City Full-Stack Product Engineering Internship Assignment**.

## 🔗 Live Demo
[https://prashantpiyush1111.github.io/neural-city-aqi](https://prashantpiyush1111.github.io/neural-city-aqi)

---

## 📌 What This Does

This dashboard overlays **CPCB Annual AQI 2023 data** on Neural City's street-level city rankings to reveal **hidden liveability gaps** across Indian cities.

Neural City ranks cities on street-level infrastructure — roads, footpaths, cleanliness, walkability, and mobility. But a city can score high on infrastructure and still have poor air quality. This prototype exposes that gap.

---

## 📊 Dataset Used

**CPCB Annual AQI Bulletin 2023**  
Sources: [data.gov.in](https://data.gov.in) / [urbanemissions.info](https://urbanemissions.info)

- Day-wise AQI readings across 271 Indian cities
- Station-level data aggregated to city-level annual averages

---

## 🧹 Data Cleaning Steps

1. Filtered to cities present in Neural City's ranking list
2. Dropped cities with fewer than 180 days of valid AQI readings
3. Computed annual mean AQI per city across all stations
4. Normalized city names (e.g. `"Bengaluru"` → `"Bangalore"`)
5. Output as clean JSON: `{ city, state, annual_avg_aqi, category }`

---

## 🎯 Use Cases

| User | Use Case |
|------|----------|
| Municipal Officer | Identify cities that score well visually but have poor air quality |
| Citizen | Get an honest view of liveability before relocating |
| Urban Planner | Correlate street score with AQI to prioritize interventions |
| City Comparison | Compare multiple cities across both dimensions |

---

## 🛠️ Tech Stack

- HTML, CSS, JavaScript (Vanilla)
- Chart.js for visualizations
- CPCB open data (JSON)

---

## 📁 Files

```
neural-city-aqi/
└── index.html      # Single-page dashboard (all-in-one)
└── README.md       # This file
```

---

## 👤 Author

**Prashant Maurya**  
Internshala — Neural City Product Engineering Assignment
