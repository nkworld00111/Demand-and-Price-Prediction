Dynamic Price Prediction & Demand Forecasting:

This project implements dynamic price prediction and demand forecasting using 
classical machine learning and time series models on sales data with multiple product and market features.

Project Overview:
This notebook provides a framework to predict dynamic prices and forecast demand using historical POS (point-of-sale) data,
combining regression models with ARIMA and Exponential Smoothing for time series analysis.

Key Features:

End-to-end workflow from preprocessing to evaluation

Machine learning price predictors: Random Forest, Gradient Boosting, Linear Regression

Time series forecasting: ARIMA, Exponential Smoothing

Feature engineering for categorical and time fields

Visualization of results and feature importances


Data Description:

The model is applied to a tabular dataset with columns:

Order ID, Order Date, Unit Cost, Price, Order Qty, Cost of Sales, Sales, Profit,

Channel, Promotion Name, Product Name, Manufacturer, Product Sub Category, Product Category, Region, City, Country.


Installation
Requirements:

Python 3.7+

pandas, numpy, matplotlib, seaborn

scikit-learn

statsmodels

How It Works:

Data cleaning: Label encoding for categorical fields, handling missing values, extracting date parts

Regression models for price prediction, with feature selection and scaling

Time series demand forecasting for selected products using ARIMA and Exponential Smoothing models

Visualization: feature importance, historical vs forecasted demand, price-vs-demand scatter plots

Sample Results:

Best price prediction model: Random Forest (R2R 2~0.80, MAE ≈ 61.59)

Demand forecast visualizations and average demand statistics per product

Feature importances plotted for top predictors


Customization:

Adapt the pipeline for your own sales/demand datasets by:

Updating feature selection/exclusion in selectfeaturesforprice

Modifying categorical fields for label encoding

Changing target forecasting product in demand forecast functions


Project Structure:

Data loading and preprocessing functions

Price prediction feature selection and training

Demand forecasting routines

Visualization utilities

Example usage workflow in main block

