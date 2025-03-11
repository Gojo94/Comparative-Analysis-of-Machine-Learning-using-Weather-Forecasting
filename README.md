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
### 1. Weather in Szeged, Temperature Prediction
- **Dataset:**
  - Hourly/daily weather records for Szeged, Hungary (2006-2016), consisting of 96,454 rows and 12 columns.
  - Features include temperature, apparent temperature, pressure, humidity, etc.
- **Methodology (KDD Process):**
  1. Data Selecting and Cleaning: Inspected dataset, checked data types and descriptive statistics.
  2. Data Preprocessing: Missing values in "Precip Type" were filled using the forward-fill method.
  3. Data Transformation: Removed redundant variables with high correlation (e.g., "Temperature" and "Apparent Temperature").
  4. Data Modelling: Split into 70% training and 30% testing.
  5. Model Evaluation: XGBoost performed the best with an Adjusted R-squared of 0.78 and RMSE of 4.91, while Elastic Net Regression performed the worst.

### 2. Weather in Delhi, Temperature Prediction
- **Dataset:**
  - Hourly weather records for Delhi, India (2009-2020), consisting of 96,433 rows and 25 columns.
  - Features include max temperature, min temperature, humidity, wind speed, etc.
- **Methodology (KDD Process):**
  1. Data Selecting and Cleaning: Analyzed dataset structure and summary statistics.
  2. Data Preprocessing: No missing values found in this dataset.
  3. Data Transformation: Dropped irrelevant columns based on correlation analysis.
  4. Data Modelling: Split into 70% training and 30% testing.
  5. Model Evaluation: Random Forest performed the best, followed by Elastic Net Regression. Multilayer Perceptron had the worst performance.

### 3. Weather in Kanpur, Humidity Prediction
- **Dataset:**
  - Hourly weather records for Kanpur, India (2009-2020), consisting of 96,433 rows and 25 columns.
  - Features include max temperature, min temperature, humidity, wind speed, etc.
- **Methodology (KDD Process):**
  1. Data Selecting and Cleaning: Explored dataset structure, data types, and statistics.
  2. Data Preprocessing: No missing values found in this dataset.
  3. Data Transformation: Dropped irrelevant columns based on correlation analysis. Dew point was removed due to high correlation with humidity.
  4. Data Modelling: Split into 70% training and 30% testing.
  5. Model Evaluation: Multilayer Perceptron, Random Forest, and XGBoost performed the best.

## Tools Used
- **Python**: Core programming language for data processing and model implementation.
- **Jupyter Notebook**: For exploratory data analysis and model development.
- **Pandas & NumPy**: For data manipulation and transformation.
- **Scikit-learn**: For implementing machine learning models.
- **XGBoost**: For advanced gradient boosting modeling.
- **Matplotlib & Seaborn**: For data visualization.

## Conclusions and Future Work
This study demonstrates the effectiveness of different machine learning models in weather prediction. The key findings include:
- XGBoost and Random Forest performed the best in terms of accuracy and generalization.
- Some models, such as Elastic Net Regression, struggled to capture complex patterns in weather data.
- The Mean Absolute Percentage Error (MAPE) metric was not used effectively due to division by zero errors when the real values were zero.

### Future Enhancements:
- Extend the study to include deep learning models such as LSTMs and CNNs for better predictive power.
- Consider classification approaches for categorical weather predictions.
- Improve feature engineering techniques to enhance model performance.
- Incorporate additional datasets to increase generalizability.

