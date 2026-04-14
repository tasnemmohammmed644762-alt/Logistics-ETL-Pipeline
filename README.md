# 🚚 Automated Logistics ETL Pipeline: Transforming Chaos into Insights

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

## 📌 Project Overview
In the fast-paced world of global logistics, raw data is often messy and scattered. This project implements a **Scalable ETL (Extract, Transform, Load) Pipeline** designed to process large-scale supply chain datasets. Using **Python, Pandas, and NumPy**, the pipeline automates the journey from raw CSV logs to structured, analysis-ready tables.

This project was developed as part of my training in the **Digital Egypt Pioneers Initiative (DEPI)**.

## 🚀 Key Features
- **Automated Data Cleaning:** Standardizing text fields (Risk Classifications) using Regex and handling duplicates.
- **Smart Feature Engineering:** - **Temporal Features:** Extracting year, month, day, and peak hour insights.
    - **Geospatial Zoning:** Rounding GPS coordinates to create logical "Geo-Zones" for regional performance tracking.
    - **Operational Risk Banding:** Implementing custom logic to categorize traffic, weather severity, and route risks (Low/Medium/High).
- **Dimensional Modeling:** Transforming a flat dataset into **Fact & Dimension tables** (Star Schema logic) for optimized BI reporting.
- **Filtering Logic:** Automated sliding window analysis (e.g., focusing on the last 6 months of operations).

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Pandas (Data manipulation), NumPy (Numerical operations & rounding), Datetime (Temporal analysis).
  
## 📊 Sample Insights Generated
The pipeline outputs three key files ready for any BI tool (Power BI/Tableau):
-Fact_Operations_Cleaned.csv: The main transactional table with all custom flags and bands.
-Agg_Daily_Summary.csv: Aggregated metrics (Shipping costs, Delay probabilities) per Geo-Zone.
-Dim_Date.csv: A dedicated date dimension for time-series analysis.

## 📂 Project Structure
```bash
├── Python-Logistics-Analytics.ipynb  # The core ETL & Analysis engine
├── Fact_Operations_Cleaned.csv        # Main cleaned dataset (Fact Table)
├── Agg_Daily_Summary.csv              # Aggregated metrics for daily reporting
└── Dim_Date.csv                       # Date Dimension for time-series analysis
├── Scripts/
│  
└── README.md
