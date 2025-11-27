# Delivery-Logistic-Analysis
Delivery Logistic Analysis optimizes shipment performance by examining distance, weight, transit time, carrier efficiency, and delivery modes. It identifies patterns causing delays, highlights high-cost routes, evaluates partner performance, and uncovers insights that improve speed, reduce cost, and enhance overall logistics efficiency.

Overview

This project focuses on analyzing transportation and logistics performance using a complete pipeline of Exploratory Data Analysis (EDA), feature engineering, predictive modeling, and Power BI dashboard visualization. The goal is to understand key operational drivers such as distance, weight, transit time, carrier performance, and mode of transport, and to build a machine learning model capable of predicting delivery time with strong accuracy. The Power BI dashboard is integrated with the model results to create an interactive, decision-oriented analytics system.

Problem Statement

Logistics companies face challenges related to delays, high operational costs, inconsistent carrier performance, and unpredictable delivery outcomes. This project aims to:

Identify patterns that influence delivery time

Predict shipment transit duration

Highlight inefficiencies across carriers, modes, and routes

Provide actionable insights to optimize logistics operations

Dataset Summary

The dataset includes:

Distance traveled

Package weight

Delivery mode

Carrier name

Region and origin

Weather condition

Delivery rating

Shipment status

Delivery cost

Delivery time (target variable)

A total of 25,000 entries with a mix of numerical and categorical features.

Machine Learning Approach
1. Data Preprocessing

Cleaning missing values

Converting delivery_time_hours to numeric

Encoding categorical variables

Handling outliers and standardizing distributions

2. Model Used

CatBoost Regressor (best performer for mixed categorical-numeric data)

3. Model Performance

MAE: 1.31 hours

RMSE: 1.65 hours

R² Score: 0.716

This indicates strong predictive capability and stable performance.

Key Insights from the Model

Distance and package weight were the strongest predictors of delivery time, showing direct influence on transit delays.

Weather conditions played a noticeable role in increasing travel time, especially in rainy and foggy scenarios.

Transport mode such as air, ship, and truck showed different levels of efficiency, with trucks having the highest variability.

Carrier performance varied significantly, revealing that a small set of carriers consistently delivered faster than others.

Certain regions had higher delays due to congestion or long-distance routes.

Cost patterns revealed that high-weight and long-distance shipments generated disproportionate cost increases.

SHAP analysis highlighted key features contributing to delays, enabling transparent model understanding.

Dashboard Insights (Power BI)

Clear visualization of shipment distribution by status, mode, origin, and carrier.

Average distance, weight, transit time, and total shipment cost are displayed for rapid performance assessment.

Bottleneck routes and underperforming regions become visible instantly.

Carrier-level comparison quickly identifies slow vs fast performers.

Integration of predicted vs actual delivery time enables proactive decision-making.

Tree maps and bar charts highlight transport efficiency patterns and cost contributors.

Key Features of This Project

End-to-end ML pipeline for logistics prediction

Highly interpretable feature importance using SHAP

Fully interactive Power BI dashboard

Clean and structured dataset transformation

Carrier, region, and mode-of-transport performance evaluation

Integrated analytics + predictive intelligence

Scalable architecture for future deployment

Technology Stack

Python (Pandas, NumPy, Scikit-learn, CatBoost, SHAP, Matplotlib)

Power BI

Jupyter Notebook

CSV dataset

Future Improvements

Deployment via Flask/FastAPI

Real-time delivery tracking and prediction

Automated alert generation for high-risk shipments

More advanced models like LightGBM and ensemble stacking

Integration with live route, traffic, and GPS APIs
