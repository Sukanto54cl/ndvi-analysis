# 🌿 NDVI Time Series Analysis

This project analyzes vegetation trends and deforestation signals using MODIS and Sentinel-2 imagery via Google Earth Engine and Python.

## ✨ Features

- NDVI time series analysis (2014–2024)
- Deforestation detection via NDVI drop events
- Exported NDVI composites and change maps
- Exploratory Data Analysis (EDA) with seasonal and rolling average trends

## 📁 File Overview

- `vegetation_analysis.ipynb`: Main Jupyter notebook with full analysis pipeline
- `requirements.txt`: Pip-based dependencies for the environment
- `data/`: Project folder containing spatial data and outputs:
  - `study_area.shp`: Shapefile of the study region
  - `NDVI_2019_before.tif`: Median NDVI image before deforestation
  - `NDVI_2021_after.tif`: Median NDVI image after deforestation
  - `NDVI_Diff_2019_2021.tif`: NDVI difference image (Before - After)
  - `study_area.qgz`: QGIS project file for spatial visualization

## 🛠 Requirements

- Google Earth Engine account with token authenticated locally
- Python 3.8+ environment (install dependencies via `requirements.txt`)
- Internet connection to run GEE Python API
- QGIS (for opening `.qgz` project file)

## 📌 Getting Started

Clone the repo, activate your environment, and open the notebook to explore vegetation changes over time.

```bash
pip install -r requirements.txt
jupyter notebook vegetation_analysis.ipynb

