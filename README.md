# Comparative Analysis of Machine Learning Algorithms using Weather Forecasting

## Project Overview
This project explores various machine learning algorithms for predicting temperature and weather patterns. The primary goal is to compare the performance of different supervised learning models in forecasting weather conditions.

### Algorithms Considered:
- Elastic Net Regression
- K-Nearest Neighbour Regression
- Random Forest Regression
- XGBoost Regression
- Multilayer Perceptron (MLP)

### Evaluation Metrics:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Adjusted R-squared
- Mean Absolute Percentage Error (MAPE)

### Datasets:
The datasets used in this project were sourced from Kaggle and contain historical weather data from multiple Indian cities and Szeged, Hungary.

[Kaggle Dataset - Szeged Weather](https://www.kaggle.com/datasets/budincsevity/szegedweather)

[Kaggle Dataset - Indian Cities Weather](https://www.kaggle.com/datasets/hiteshsoneji/historical-weather-datafor-Indiancities)

## Workflow
### 1. Szeged, Temperature Prediction
- **Dataset:** Weather data (2006-2016), 96,454 rows, 12 columns.
- **Process:** Data cleaning, missing value handling, correlation analysis, feature selection, model training (70/30 split).
- **Results:** XGBoost performed best (Adjusted R² = 0.78, RMSE = 4.91). Elastic Net Regression performed worst.

### 2. Delhi, Temperature Prediction
- **Dataset:** Weather data (2009-2020), 96,433 rows, 25 columns.
- **Process:** Data exploration, correlation analysis, feature selection, model training (70/30 split).
- **Results:** Random Forest performed best. Multilayer Perceptron had the lowest accuracy.

### 3. Kanpur, Humidity Prediction
- **Dataset:** Weather data (2009-2020), 96,433 rows, 25 columns.
- **Process:** Data analysis, feature selection (dropped dew point), model training (70/30 split).
- **Results:** Multilayer Perceptron, Random Forest, and XGBoost performed best.

## Tools Used
- **Python, Jupyter Notebook** for data processing & modeling.
- **Pandas, NumPy** for data manipulation.
- **Scikit-learn, XGBoost** for ML models.
- **Matplotlib, Seaborn** for visualization.

## Key Findings & Future Work
- XGBoost and Random Forest performed best overall.
- Elastic Net Regression struggled with complex patterns.
- Future improvements: deep learning models (LSTMs, CNNs), feature engineering, additional datasets.


