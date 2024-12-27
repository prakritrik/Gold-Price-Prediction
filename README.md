# Gold Price Prediction Using Machine Learning

## Overview

This project predicts gold prices using a dataset that includes financial indicators such as the S&P 500 Index (SPX), crude oil price (USO), silver price (SLV), and the EUR/USD exchange rate. The model is built using the Random Forest Regressor algorithm, providing accurate predictions based on historical data.

---

## Dataset Details

- **Number of rows:** 2290
- **Number of columns:** 6
- **Features:**
  - `Date`: The date of the record.
  - `SPX`: S&P 500 Index.
  - `GLD`: Gold price (target variable).
  - `USO`: Crude oil price.
  - `SLV`: Silver price.
  - `EUR/USD`: EUR/USD exchange rate.

---

## Project Workflow

1. **Data Preprocessing:**
   - Missing value check: No missing values in the dataset.
   - Statistical summary analysis.
   - Correlation analysis using a heatmap to understand feature relationships.

2. **Exploratory Data Analysis:**
   - Visualization of feature distributions.
   - Analysis of the `GLD` price correlation with other features.

3. **Model Training:**
   - Algorithm: Random Forest Regressor.
   - Train-Test split: 80% training, 20% testing.
   - Random Forest hyperparameters: Default with `n_estimators=100`.

4. **Evaluation:**
   - Predictions made on the test dataset.
   - Visualization of prediction accuracy.

---

## Key Findings

- **High Correlation:** 
  - Silver price (`SLV`) has the strongest positive correlation with gold price (`GLD`).
  - Oil price (`USO`) has a weak negative correlation with `GLD`.
  
- **Model Performance:**
  - Random Forest Regressor provided accurate predictions based on feature relationships.

---

## Requirements

### Python Libraries:
```bash
numpy
pandas
matplotlib
seaborn
scikit-learn
