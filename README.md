Big Data Capstone Project

Cross-Device Energy Consumption & Carbon Footprint Analytics using Databricks & Spark ML

This project analyzes energy consumption across heterogeneous devices and estimates the associated carbon footprint using scalable distributed processing in Apache Spark on Databricks. It builds interactive dashboards, machine learning models, anomaly detection workflows, and ESG reporting outputs to support sustainability-driven decision-making.

---

Project Structure

Notebook	Description

data_generation.ipynb	Synthetic IoT-style energy dataset creation
use_case_1.ipynb	Energy & Carbon Monitoring Dashboard
use_case_2.ipynb	Adaptive Power Management using K-Means Clustering
use_case_3.ipynb	Green Charging & Carbon Prediction Models
use_case_3_model_eval.ipynb	Model comparison for carbon prediction
use_case_4.ipynb	Time-Series Forecasting & Anomaly Detection
use_case_5.ipynb	ESG & Sustainability Reporting Outputs
master_pipeline.ipynb	Automated end-to-end pipeline execution

---

Technology Stack

Databricks (Community Edition)

Apache Spark / PySpark

Delta Lake (Optimized Storage)

Spark MLlib (Linear Regression, Random Forest, GBT, K-Means)

Python / Pandas / Matplotlib

Databricks SQL Dashboards

---

Data Architecture & Workflow

Device Energy Data → Spark ETL → Delta Storage → ML Modeling 
→ Dashboards → Carbon Insights → ESG Reporting

Data generated hourly for multiple devices and locations

Carbon emissions calculated using standardized conversion factors

Supports scalable batch analytics and ML training

---

Use Cases

1. Energy & Carbon Dashboard

Visualizes energy consumption trends by device & location

Computes total carbon emissions over time


2. Adaptive Power Management (Clustering)

K-Means groups devices based on consumption patterns

Identifies high-load appliances for efficiency optimization


3. Green Charging & Carbon-Aware Optimization

Models evaluated to predict carbon emission (carbon_kg):

Model	Performance Summary

Linear Regression	Baseline reference model
Random Forest Regressor	✅ Best accuracy (highest R², lowest RMSE)
Gradient Boosted Trees (sampled)	Good but limited due to free-tier memory constraints


4. Forecasting & Anomaly Detection

Time-based feature engineering (hour, weekday, seasonality)

Linear Regression forecasting

Anomaly detection using residual thresholding → Detects inefficiencies & leaks


5. ESG / Sustainability Reporting

Summarizes device impact & carbon loads

Generates structured outputs usable for corporate ESG disclosure

---

Key Insights

HVAC & heating devices account for most energy load

Strong daily and hourly consumption cycles

Carbon-aware scheduling reduces energy cost + environmental impact

Residual anomaly monitoring identifies waste & abnormal usage early

---

Green Charging Recommendations

Recommendation	Impact

Shift high-load charging to low-carbon grid hours	Lower carbon intensity
Automate peak/off-peak scheduling	Reduces cost & emissions
Replace inefficient legacy devices	Long-term sustainability
Continuously monitor anomaly alerts	Prevents waste & failures

---

How to Run

1. Import notebooks into Databricks Workspace


2. Execute data_generation.ipynb to create dataset


3. Run use-case notebooks in sequence or execute master_pipeline.ipynb


4. Open dashboards via Databricks workspace panels

---

Project Demo Video

🔗 https://drive.google.com/file/d/11aoxNGh1hQdlEc3OusAFoCS5hIqAJFxu/view?usp=sharing

---

Author

Gumpu UshaSri
Big Data Analytics Capstone Project
