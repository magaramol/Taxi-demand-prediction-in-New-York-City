# Taxi Demand Prediction in New York City

This repository contains a machine learning project focused on predicting taxi demand in New York City. The project utilizes data from the NYC Taxi & Limousine Commission

## Objective
The main objective of this project is to develop a predictive model that can forecast taxi demand in different parts of New York City. By accurately predicting demand, taxi companies can optimize their fleet management and improve service efficiency.


## Data Source
__Download the data from here:__  
- [http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml](http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml) (2016 data) - Data provided by the NYC Taxi and Limousine Commission (TLC) in parquet format.
- [https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data](https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data) - Alternate data source containing NYC yellow taxi trip data in csv format.



## Data Analysis
- **Outlier Detection:** Performed univariate analysis to identify outliers in key variables such as pickup latitude, pickup longitude, dropoff latitude, dropoff longitude, trip duration, speed, trip distance, and total fare.
- **K-Means Clustering:** Utilized K-means clustering to cluster the data based on the pickup and dropoff locations, providing insights into the spatial distribution of taxi pickups and dropoffs.

## Baseline Models
- **Ratio of Last 2 Years' Data:** Used the ratio of taxi demand data from the last two years as a baseline model for comparison with more advanced models.
- **Previous Values for Future Prediction:** Leveraged previous taxi demand values to predict future demand, establishing another baseline for comparison.
- **Simple Moving Averages (SMA):** Implemented SMA as a baseline model, which calculates the average demand over a specified number of previous time periods.
- **Weighted Moving Averages (WMA):** Utilized WMA as a baseline model, which assigns weights to previous time periods to calculate the average demand.
- **Exponential Weighted Moving Averages (EWMA):** Employed EWMA as a baseline model, which gives more weight to recent time periods in calculating the average demand.

## Regression Models
- **Random Forest Regressor:** Applied Random Forest Regressor to the data to predict taxi demand.
- **XGBoost Regressor:** Utilized XGBoost Regressor as a regression model for taxi demand prediction. After evaluation, XGBoost Regressor was found to perform better than the other models.
- **Linear Regression:** Implemented Linear Regression as a baseline regression model for comparison with more complex models.

## Methodology
The project involves several key steps, including data preprocessing, exploratory data analysis (EDA), feature engineering, model selection, and evaluation. Various machine learning algorithms, such as regression and time series forecasting models, are explored to identify the most suitable approach for predicting taxi demand.

## Results
The results of the predictive models are evaluated based on metrics such as accuracy, precision, and recall. The best-performing model is selected for deployment, with the potential to improve taxi service operations and enhance customer satisfaction.

## Conclusion
Overall, this project demonstrates the application of machine learning techniques to address real-world problems in the transportation sector. By accurately predicting taxi demand, it has the potential to benefit both taxi companies and passengers in New York City.
