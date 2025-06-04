# 🚀 SpaceX Data Science Project

A comprehensive end-to-end data science pipeline focused on analyzing SpaceX launch data. This project leverages web scraping, REST APIs, SQL queries, interactive visualizations, and machine learning to extract insights and predict launch success.

## 📁 Repository

[🔗 GitHub Repository](https://github.com/Rayan-Alam-UOIT/Space-X-Data-Science-Project.git)

---

## 📌 Table of Contents

- [Overview](#overview)
- [Data Collection](#data-collection)
- [Data Wrangling](#data-wrangling)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Interactive Visualizations](#interactive-visualizations)
- [Predictive Modeling](#predictive-modeling)
- [Results](#results)
- [Conclusion](#conclusion)

---

## 🛰️ Overview

This project investigates SpaceX’s historical launch data to answer questions such as:

- Which launch sites are most active?
- What is the relationship between payload mass, orbit type, and launch success?
- Can we build a model to predict mission success?

We collected and processed data from Wikipedia and SpaceX’s public API, analyzed it using SQL and visualization tools, and built several machine learning models for prediction.

---

## 📥 Data Collection

Data sources:

- **Wikipedia Web Scraping**: Extracted HTML table rows and cells using `requests` and `BeautifulSoup`.
- **SpaceX REST API**: Fetched launch, rocket, payload, and launchpad data using endpoints like `/v4/launches`.

Data was converted into structured Pandas DataFrames for downstream tasks.

---

## 🧹 Data Wrangling

- Removed HTML tags, citations, and missing values.
- Parsed date/time fields, extracted booster versions, and converted payload mass to numeric format.
- Applied feature engineering such as dummy encoding and data standardization.

---

## 📊 Exploratory Data Analysis

Performed EDA using:

- **Seaborn & Matplotlib**: Scatter plots, bar charts, success trends over time.
- **SQL**: Used subqueries, `GROUP BY`, `MIN()`, and filtering to answer questions about launches, boosters, and payloads.

---

## 🗺️ Interactive Visualizations

- **Folium Maps**:
  - Plotted launch sites and individual mission outcomes.
  - Used marker clustering and geographic distance calculations to nearby infrastructure.
  
- **Plotly Dash Dashboards**:
  - Dropdowns to filter by launch site.
  - Range slider for payload selection.
  - Pie charts and scatter plots for mission success and failure analysis.

---

## 🤖 Predictive Modeling

Used `scikit-learn` to train and evaluate classification models:

- **Models**: Logistic Regression, SVM, Decision Tree, K-Nearest Neighbors
- **Techniques**:
  - Feature scaling with `StandardScaler`
  - Categorical encoding with `get_dummies()`
  - Hyperparameter tuning with `GridSearchCV` (10-fold CV)
  
All models achieved an accuracy of **0.84**, with **Logistic Regression** selected as the best model for its interpretability and efficiency.

---

## 📈 Results

- Identified that some launch sites and orbits are more successful than others.
- Observed payload patterns related to mission success.
- Developed interactive tools to explore data geographically and temporally.
- Built accurate classification models to predict launch success.

---

## ✅ Conclusion

This project demonstrates a full data science lifecycle:

1. **Data acquisition** from public sources
2. **Wrangling and cleaning** to structure raw inputs
3. **Exploratory and interactive analysis** using SQL, plots, and dashboards
4. **Predictive modeling** to forecast launch success

The approach highlights how technical and analytical skills combine to extract actionable insights from real-world aerospace data.

---

## 📎 Appendix

All source notebooks, scripts, and assets are available in the [project repository](https://github.com/Rayan-Alam-UOIT/Space-X-Data-Science-Project.git). Each component is documented and reproducible.

---

