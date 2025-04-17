# 🌬️ Investigating Air Quality in an Italian Region  
**Modeling • Time Series Forecasting • Clustering Analysis**

This project explores air quality patterns in an Italian city using data sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/air+quality). It contains 9,358 hourly measurements collected between March 2004 and April 2005. The dataset includes responses from five chemical sensors that measure:

- **Carbon Monoxide (CO)**
- **Non-methanic Hydrocarbons (NMHC)**
- **Benzene (C₆H₆)**
- **Nitrogen Oxides (NOₓ)**
- **Nitrogen Dioxide (NO₂)**

---

## 📌 Summary of Key Insights

- **Benzene and CO levels showed clear daily and weekly cycles**, peaking during commuting hours—suggesting strong links to traffic emissions.
- **SARIMAX models successfully forecasted pollutant levels**, particularly for CO and NO₂, with seasonality and trends clearly captured.
- **PCA revealed distinct variance across sensors**, helping reduce noise and highlight dominant pollutant behaviors.
- **K-Means clustering uncovered time-based groupings**, such as weekday vs. weekend air quality profiles.
- Visualizations enhanced interpretability of pollutant behavior across both short-term and long-term periods.

---

## 🧠 Methodology

- **Data Cleaning & Resampling**: Managed missing values, converted timestamps, and aggregated hourly averages.
- **Exploratory Data Analysis (EDA)**: Trend plots, heatmaps, and correlation matrices to understand pollutant behavior.
- **Dimensionality Reduction**: PCA applied to identify main directions of variance and reduce dimensional complexity.
- **Forecasting**: SARIMAX models used to predict future pollutant concentrations with seasonal components.
- **Clustering**: K-Means applied to both raw and PCA-transformed data to detect temporal or behavioral clusters.

---

## 🛠️ Technologies Used

- **Programming Language**: Python  
- **Libraries**:
  - `pandas`, `numpy` – Data handling
  - `matplotlib`, `seaborn` – Visualization
  - `statsmodels` – Time series modeling (SARIMAX)
  - `scikit-learn` – PCA, K-Means clustering

---

## 📂 Repository Structure

📦 air-quality-analysis ┣ 📊 notebooks/ ┃ ┗ 📓 Air_Quality_Analysis_Final.ipynb ┣ 📁 data/ ┃ ┗ air_quality_uci.csv ┣ 📁 images/ ┃ ┗ (Optional plots or PCA visuals) ┗ README.md

