# 🚲 Bike Sharing Demand Prediction with LightGBM

This project predicts hourly bike rental demand using the **UCI Bike Sharing Dataset** and **LightGBM**, a gradient boosting framework optimized for speed and performance.

---

## 📊 Project Overview

The goal is to build a high-performing regression model that predicts the total count of bike rentals (`cnt`) based on time, weather, and user features. The model is built and evaluated using **LightGBM** for its efficiency in handling structured, tabular data.

---

## 🧠 Methods and Workflow

1. **Data Loading & Exploration**
   - Loaded `day.csv` and `hour.csv` datasets.
   - Created a combined datetime index from `dteday` and `hr`.
   - Explored correlations between user groups (`casual`, `registered`, `cnt`).

2. **Feature Engineering**
   - Extracted temporal features (hour, day, month, weekday, season).
   - Integrated weather data and categorical encodings.
   - Handled missing and duplicate values.

3. **Model Training**
   - Trained a **LightGBM Regressor**.
   - Hyperparameter tuning with grid/random search.
   - Used time-based train-validation splits.

4. **Evaluation**
   - Metrics: **RMSE**, **MAE**, and **R²**.
   - Visualized predictions vs. actual counts.
   - Generated feature importance plots.

---
