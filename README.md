# Ghana Fisheries & Aquaculture Analysis (1990–2023)

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## Overview

Ghana's fisheries sector supports over **2 million livelihoods** and provides more than **60% of the nation's animal protein**. This project analyses 33 years of fisheries data across three interconnected dimensions:

- **Wild catch decline** — marine, inland, and Volta Lake catch trends since 1990
- **Aquaculture growth** — whether farmed fish production compensates for wild stock losses
- **Climate impact** — relationship between rising sea surface temperatures, rainfall decline, and fish production

---

## Key Findings

| Indicator | 1990 | 2023 | Change |
|-----------|------|------|--------|
| Wild Catch | 428,000 t | 168,000 t | -60.7% |
| Aquaculture | 1,200 t | 357,700 t | +29,708% |
| Fish Imports | 120,000 t | 548,000 t | +357% |
| Sea Surface Temp | 26.1°C | 29.6°C | +3.5°C |
| Volta Lake Catch | 85,000 t | 25,500 t | -70% |

Wild catch declines strongly correlate with rising SST (R² = 0.98, p < 0.0001).

---

## Visualisations

| Figure | Description |
|--------|-------------|
| `fig1_wild_vs_aquaculture.png` | Wild catch components vs aquaculture growth |
| `fig2_volta_lake_decline.png` | Volta Lake catch decline with trend line |
| `fig3_production_gap.png` | Production gap — wild catch, aquaculture & imports |
| `fig4_climate_vs_catch.png` | SST & rainfall correlation with wild catch |
| `fig5_imports_price.png` | Fish import dependency & price trends |
| `fig6_projection_2040.png` | Production projection to 2040 with 95% CI |
| `qgis_fisheries_map.png` | Professional GIS map — marine, inland & aquaculture sites (QGIS) |
## Interactive Fisheries Map

[![Ghana Fisheries Map](outputs/figures/ghana_fisheries_map_preview.png)](https://nbviewer.org/github/ChaseKelvin/ghana-fisheries-aquaculture/blob/main/outputs/ghana_fisheries_map.html)

> 👆 Click the image above to open the full interactive map — toggle between
> marine, inland and aquaculture layers using the top-right control.
> Click any marker for full site details including species, production volume and threats.

---

## Project Structure

```
ghana-fisheries-aquaculture/
│
├── data/
│   └── ghana_fisheries_aquaculture.csv    # 15 parameters, 34 years
│
├── notebooks/
│   └── analysis.ipynb                     # Full analysis (10 cells, 6 figures)
│
├── outputs/
│   └── figures/                           # All generated charts
│
├── requirements.txt
└── README.md
```

---

## Data Sources

- **FAO FishStat** — Global fishery and aquaculture production statistics
- **Ghana Fisheries Commission** — Annual sector reports
- **World Bank** — Fish production and trade, World Development Indicators
- **ERA5 / NASA POWER** — Sea surface temperature data
- Nunoo et al. (2014). Marine fisheries catches in Ghana. *Sea Around Us*
- Ofori-Danson et al. (2007). Causes of decline in Lake Volta yields. *WAJAE*

---

## How to Run

```bash
git clone https://github.com/ChaseKelvin/ghana-fisheries-aquaculture.git
cd ghana-fisheries-aquaculture
pip install -r requirements.txt
jupyter notebook notebooks/analysis.ipynb
```

Run **Cell → Run All** to generate all 6 figures.

---

## Related Projects

This project is part of a Ghana environmental data science portfolio:

- **Project 1:** [Galamsey Water Contamination](https://github.com/ChaseKelvin/galamsey-water-contamination-ghana)
- **Project 2:** [Lake Bosomtwe Risk Assessment](https://github.com/ChaseKelvin/lake-bosomtwe-water-quality)
- **Project 3:** [Urban Heat Wave Trends](https://github.com/ChaseKelvin/ghana-urban-heatwave-trends)
- **Project 4:** Ghana Fisheries & Aquaculture ← *this project*

---

## Author

**Kelvin Chase**  
Environmental Science | GIS & Remote Sensing | Ghana  
[GitHub](https://github.com/ChaseKelvin)
