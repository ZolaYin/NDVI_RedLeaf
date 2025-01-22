# NDVI_RedLeaf

## Project Overview
NDVI_RedLeaf is a project aimed at predicting autumn leaf color changes using NDVI (Normalized Difference Vegetation Index), elevation data, and short-term weather forecasts. This project focuses on Bear Mountain State Park as a case study and uses advanced random forest regression models combined with Empirical Orthogonal Function (EOF) analysis to achieve high-precision spatiotemporal predictions of leaf color dynamics.

---

## File Structure
- **Part1_NDVI__RedLeaf.ipynb**  
  Contains data preprocessing and initial analysis, including NDVI noise reduction, seasonal trend extraction, and input data generation for the dynamic model.

- **Part2_NDVI__RedLeaf.ipynb**  
  Focuses on model training and prediction, using EOF and random forest to predict the Brownness Index and determine key stages of leaf color change.

- **NDVI_RedLeaf_DATA/**  
  Stores raw data and intermediate results, including NDVI data, elevation data, and weather information.

- **README.md**  
  This file provides an introduction and guide to the project.

---

## Methodology
1. **NDVI Data Preprocessing**  
   - Extract the upper envelope of NDVI to reduce noise and remove outliers.  
   - Replace traditional NDVI with the Brownness Index to more accurately reflect autumn leaf color changes.

2. **Model Construction**  
   - Use EOF to extract major variability patterns from weather data, combined with NDVI and elevation as inputs.  
   - Train a random forest model to predict the Brownness Index for each pixel.

3. **Visualization**  
   - Provide spatiotemporal distribution maps of leaf color changes and highlight key time points such as the start of color change, near-peak, peak, and end.

---

## Data Sources
- **NDVI Data**: MODIS Aqua NDVI (2003–2022) with 500m spatial and daily temporal resolution.  
- **Elevation Data**: SRTM Digital Elevation Model (500m resolution).  
- **Weather Data**: ERA5 global reanalysis data, covering daily meteorological variables (temperature, precipitation, wind speed) from 2003 to 2022.

---

## Project Outcomes
- Model Mean Squared Error (MSE): 0.0624, demonstrating high prediction accuracy.  
- Results successfully capture spatiotemporal dynamics of autumn leaf color changes, supporting short-term travel planning and ecological monitoring.
