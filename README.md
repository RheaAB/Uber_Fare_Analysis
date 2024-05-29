# Optimizing Ride-Hailing Fares with Predictive Analytics

## Project Overview

In the competitive landscape of ride-hailing services, strategic fare pricing is critical for business success and customer satisfaction. This project explores the potential of data science to create a predictive model for taxi fares, empowering ride-sharing companies to optimize their pricing models dynamically.

## About the Dataset

The dataset is a rich compilation of ride details from a ride-sharing service, with each entry capturing the essence of urban commutes. The key attributes include:

- **key**: Unique identifier for each trip, derived from ride timestamps or generated hashes.
- **fare_amount**: Total fare charged, serving as the target variable for prediction.
- **pickup_datetime**: Start date and time of the ride, key for analyzing fare trends.
- **pickup_longitude**: Longitude of the pickup point, crucial for location-based analysis.
- **pickup_latitude**: Latitude of the pickup point, determines the ride's starting location.
- **dropoff_longitude**: Longitude of the drop-off point, aids in calculating travel distances.
- **dropoff_latitude**: Latitude of the drop-off point, completes the route data for analyses.
- **passenger_count**: Count of passengers, affects fare due to different pricing for passenger numbers.

[Dataset Link](https://www.kaggle.com/datasets/yasserh/uber-fares-dataset)

## Objectives

The overarching goal of this project is to accurately predict taxi fares to aid ride-sharing companies in:
- Refining their pricing strategies.
- Improving the overall customer experience.
- Achieving operational excellence.

## Methodology

### Data Preprocessing
- Transformed geospatial data for precise mapping and analysis.
- Split the date column into multiple columns like Year, Month, Weekday, Hour, Monthly_Quarter, and Hourly_Segments to enrich the dataset.

### Exploratory Data Analysis (EDA)
- Conducted in-depth statistical reviews to understand fare distribution and key contributing factors.

### Visualization
- Employed a variety of graphical representations to showcase insights and foster a deeper understanding of the data.

### Model Evaluation
- Assessed multiple regression models using key performance indicators to identify the most accurate predictive model.

## Key Features

- **Novel Engineering**: Split the date column into multiple segments for clearer analysis.
- **Innovative Visualization Techniques**: Used folium for geographic analysis visualization.
- **Interactive Dashboards**: Created dynamic, user-interactive dashboards for real-time data exploration using dash.
- **Novel Feature Engineering**: Devised new features like rush-hour and fare efficiency for nuanced insights.
- **Algorithmic Innovation**: Employed `RandomizedSearchCV` and `GridSearchCV` for hyperparameter tuning.
- **Boosting Methods**: `HistGradientBoostingRegressor` and `GradientBoostingRegressor` showed superior performance, indicating strong generalization capabilities.

## Significant Findings

1. **Boosting Methods Outperform Other Models**: Models like `HistGradientBoostingRegressor` and `GradientBoostingRegressor` displayed superior performance due to their iterative error correction capabilities.
2. **Overfitting in Complex Models**: `DecisionTreeRegressor` showed significant overfitting, highlighting the importance of ensemble techniques to mitigate this issue.
3. **Consistency Between Train and Test Performance**: Models like `XGBoost` and `Gradient Boosting` demonstrated a good balance between bias and variance.
4. **Merit of Simpler Models**: Simpler models like `Linear Regression` offer advantages in interpretability and faster prediction times, making them suitable for scenarios where explainability and efficiency are crucial.

## Conclusion

This project highlights the effectiveness of boosting methods in predicting taxi fares and underscores the need for a balanced approach in model complexity. The insights gained can guide future iterations of the modeling process, prompting considerations such as additional feature engineering, alternative model selection, or further hyperparameter tuning to enhance predictive performance.
