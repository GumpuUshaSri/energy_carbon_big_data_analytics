Big Data Capstone Project

Cross-Device Energy Consumption & Carbon Footprint Analytics Using Databricks & Spark ML

This project focuses on analyzing energy usage across multiple device categories and estimating associated carbon emissions at scale using Apache Spark on Databricks. The project provides dashboards, predictive ML models, anomaly detection, sustainability recommendations, and ESG reporting support.

Project Structure

data_generation.ipynb – Synthetic IoT-like dataset creation
use_case_1.ipynb – Energy & Carbon Analytics Dashboard
use_case_2.ipynb – Adaptive Power Management (Clustering)
use_case_3.ipynb – Green Charging & Carbon Prediction
use_case_3_model_eval.ipynb – Model comparison for prediction models
use_case_4.ipynb – Forecasting and Anomaly Detection
use_case_5.ipynb – ESG Reporting and Sustainability Summary
master_pipeline.ipynb – End-to-end workflow pipeline execution

Technology Stack

Databricks (Community Edition)
Apache Spark (PySpark)
Delta Tables for optimized storage
Spark MLlib (Regression, Clustering, GBT, Random Forest)
Python
Databricks SQL Dashboards for visualization

Data Architecture & Processing Workflow

Raw device-level energy readings → Spark ETL (cleaning & feature engineering) → Delta Lake Storage → ML Modeling → Dashboards & Insights → Sustainability / ESG Reporting Outputs.

Data is generated at hourly granularity per device. Carbon footprint is calculated using standardized emission conversion factors. The architecture supports scalable time-series data and ML workflows.

Use Case Overview

Use Case 1: Energy & Carbon Dashboard

Visualizes consumption trends by device and location

Calculates total carbon emissions over time


Use Case 2: Adaptive Power Management using Clustering

K-Means clusters devices based on consumption behavior

Identifies high-consumption appliances for optimization


Use Case 3: Green Charging & Carbon-Aware Optimization

Predicts carbon footprint using:

Linear Regression

Random Forest Regressor

Gradient Boosted Tree Regressor (GBR with sampling to avoid model size overflow)


Random Forest delivered best R² and RMSE performance among evaluated models


Use Case 4: Forecasting & Anomaly Detection

Feature engineering extracts hour, day, and weekday signals

Linear Regression used for energy forecasting

Anomalies detected using residual thresholds

Helps detect abnormal behavior or energy leakage


Use Case 5: ESG / Sustainability Reporting

Aggregates carbon impact by device category and location

Outputs summary suitable for corporate carbon transparency reporting


Model Performance Comparison (Use Case 3)

Linear Regression: Baseline performance
Random Forest: Best accuracy, captures non-linear device behavior effectively
GBT (sampled): Good, but limited by compute constraints of free tier

Key Insights

• HVAC and Heating devices contribute the highest consumption load
• Energy patterns strongly follow daily usage cycles
• Carbon-aware scheduling can significantly reduce digital carbon footprint
• Residual anomaly detection identifies unusual spikes and inefficiencies

Green Charging Recommendations

• Schedule charging during low grid-carbon hours
• Automate heavy appliance operation to non-peak periods
• Replace high-load legacy devices to reduce long-term energy consumption
• Continuously monitor anomalies to prevent energy waste

How to Run

1. Import notebooks into Databricks

2. Run data_generation.ipynb to create dataset

3. Run use_case notebooks in sequence or execute master_pipeline.ipynb for automated execution

4. View dashboards inside Databricks workspace


Author

Gumpu UshaSri
Big Data Analytics Capstone Project
