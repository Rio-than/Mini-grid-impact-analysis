# 🌞 **Renewvia‑Minigrid‑Impact‑Analysis** &nbsp;![status-badge](https://img.shields.io/badge/status-active-brightgreen) ![python-badge](https://img.shields.io/badge/Python-3.10-blue) ![license-badge](https://img.shields.io/badge/license-MIT-lightgrey)

> **value statement**

> *Data‑driven evidence showing how Renewvia’s solar‑minigrids cut kerosene spending by 45 %, add four extra lighting hours per night, and unlock new income opportunities in off‑grid Kenyan communities.*

---

## 📈 Project Overview

Most rural Kenyan households still rely on kerosene, candles, or small solar kits for light and cooking. 

This repository contains **Python notebooks, cleaned datasets, and ready‑made visuals** that measure the social and economic impact of Renewvia’s solar‑minigrids in 
**Marsabit, Turkana, Siaya, Kajiado, and Homa Bay**.

The analysis asks three core questions:

1. *Does minigrid access reduce household fuel costs?*  
2. *How does reliable electricity change evening light hours?*  
3. *Which occupations and income groups benefit the most?*

---

## 🎯 Goal 

> *Bridge the knowledge gap between pilot minigrid projects and real‑world outcomes.*
> 
> Stakeholders—investors, NGOs, and county governments—need **transparent metrics** to scale successful models and close remaining energy‑equity gaps.

---

## ✨ Key Features

| Category | Description |
|----------|-------------|
| 📊 **Interactive dashboards** | Power BI & Plotly dashboards (lighting hours, kerosene savings, appliance uptake) |
| 🔄 **Automated ETL scripts** | Python pipelines for raw survey & smart‑meter data → tidy analytics tables |
| 📐 **Custom metrics** | Appliance cost elasticities, fuel‑switch indices, per‑capita kWh distribution |
| 📜 **Reproducible notebooks** | Jupyter notebooks for exploratory analysis & report generation |

---

## 📂 Project Structure
### 🚀 Usage
### Step	Action
1. Prepare Data	Place raw CSVs in /data/raw/ and run:
python scripts/01_etl.py
2. Explore Notebook	Open notebooks/02_eda.ipynb for interactive charts
3. Build Dashboard	Open dashboards/MinigridImpact.pbix in Power BI Desktop
4. Generate Report	Run notebooks/99_report.ipynb → exports PDF/HTML

Sample command to reproduce Figure 4 (lighting hours distribution):

bash
Copy
Edit
jupyter nbconvert --execute notebooks/03_visuals.ipynb

## Technical Details

Languages/Tools : Python 3.10, Pandas, NumPy, Plotly, Power BI

Data volume : ≈ 90 MB (5 surveys + 1 smart‑meter dump)

Key challenges : fuzzy occupation labels, non‑matching survey IDs, skewed kerosene‑cost distribution

### Solution highlights :

Probabilistic ID matching (Jaro‑Winkler) between pre‑ and post‑surveys

Hourly load‑profile aggregation with dask for memory efficiency

Storytelling visuals styled with a green‑gold palette to reflect clean‑energy themes

📊 Results & Insights

Metric	Finding

Kerosene savings	‑ KES 320 / month average; 65 % households spend nothing on kerosene post‑connection

Lighting hours	+ 4.2 h per night in Marsabit & Turkana; + 2 h in Siaya

Appliance elasticity	Each new appliance adds ~ KES 195 to the bill, but per‑appliance cost drops 18 % after 4 units

Cooking fuel switch	38 % of minigrid users adopted electric pressure cookers within 12 months

(Full tables and plots in /docs/summary.pdf)

## 🔮 Future Work

Real‑time smart‑meter streaming via MQTT for live dashboards

ML model to predict future peak loads and inform battery‑size decisions

Expand study to include Kwale and West Pokot counties

## 🤝 Contributing

Fork the repo & create your feature branch: git checkout -b feature/amazing-feature

Commit your changes: git commit -m 'Add amazing feature'

Push to the branch: git push origin feature/amazing-feature

Open a Pull Request

## 🗄️ Data Sources

Dataset	Notes

Household pre‑survey	Courtesy of ["C:\Users\Administrator\Documents\power_leo.csv"] – anonymised

Household post‑survey	Courtesy of ["C:\Users\Administrator\Documents\power_leo.csv"] – anonymised

Smart‑meter logs	Exported by Renewvia IoT platform (Jan 2024 – Jun 2025)

See /docs/data_dictionary.md for schema details.

## 📞 Contact & Support 

For questions or collaboration, open an issue or reach blessingsziko@gmail.com

## 📚 References

Clean Cooking Alliance. Kenya Market Assessment (2024).

World Bank / MECS. Electric Cooking in Minigrids: Business Models (2023).

Renewvia Energy. Project Briefs & Annual Impact Report (2025).

<p align="center"><i>Made with ☀️ &nbsp;for cleaner, brighter communities.</i></p> ```

