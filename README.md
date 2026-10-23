# Logistics_Data_Analyst_Intern
Supply Chain &amp; Logistics Data Analyst Internship portfolio showcasing end-to-end data cleaning, SQL queries, Python analysis, and interactive Power BI dashboards for operational efficiency.

🚚 End-to-End Supply Chain Analytics & Predictive Freight Cost Optimization

YuvaIntern Logistics Data Science & Machine Learning Internship Portfolio Project

📌 Executive Summary

Fluctuations in transportation tariffs, unpredictable carrier surcharges, and inefficient route dispatch logic directly compromise operational margins in modern 3PL/4PL supply chain networks.

This repository houses an end-to-end analytics and machine learning pipeline built over a 4-week structured internship framework. The project ingests raw fulfillment transactions, performs automated data preprocessing and outlier scrubbing, executes exploratory statistical analysis (EDA), and deploys predictive regression models to forecast Freight Shipping Fees (freight_cost_inr).
Key Quantified Outcomes
Prediction Accuracy: Reached an $R^2$ score of 99.25% with a Mean Absolute Error (MAE) of ₹15.50, outperforming ensemble decision trees for linear freight pricing matrices.
Cost Leakage Mitigation: Built an Automated Overbill Audit Trigger framework to flag carrier invoices exhibiting $>15\%$ positive variance from model predictions.
Operational Strategy: Formulated 3 actionable logistics strategies expected to reduce baseline freight spend by 8–12%.
🏗️ End-to-End System Architecture                                  
                      DATA PIPELINE FLOW
                                  
[ Order Management ] ──► [ Week 1: Strategy ] ──► [ Week 2: Cleaning ]
      System               • Business KPIs          • Imputation / Outlier (IQR)
                           • Data Contract          • Categorical OHE Encoding
                                                                │
                                                                ▼
[ Deployable Insights ] ◄─ [ Week 4: ML Models ] ◄─ [ Week 3: EDA & Correlation ]
  • Dynamic Routing          • Linear Regression      • Multi-collinearity Matrix
  • Overbill Audits          • Random Forest          • Cost-per-distance Drivers
  • Load Consolidation       • Evaluation (MAE/RMSE)  • Hub Latency Profiling

🗂️ Weekly Internship Deliverables & Technical Scope
📍 Week 1: Business Understanding & Data Strategy Design
Strategic Focus: Formulated domain problem statement and analytical roadmap for enterprise logistics networks.
Key Achievements:Map baseline data contract consisting of mass (order_weight_kg), route distance (distance_km), operational transit time (cycle_time_hrs), 3PL carriers (carrier_partner), and origin fulfillment nodes (fulfillment_hub).
Identified key operational failure points: carrier billing inaccuracies, delayed route dispatches, and unoptimized weight-class assignments.

📍 Week 2: Data Preprocessing, Cleaning & Pipeline Engineering
Strategic Focus: Transformed unstructured/synthetic raw order data into an ML-ready analytical dataset.
Key Achievements:
Anomalous Scrubbing: Applied Interquartile Range (IQR) clipping to remove non-physical outlier spikes in weight and distance variables.
Categorical Encoding: Leveraged One-Hot Encoding (pd.get_dummies(drop_first=True)) to represent multi-class categorical features (carrier_partner, fulfillment_hub) without introducing dummy variable traps.
Feature Engineering: Scaled continuous metrics and verified matrix ranks to eliminate multi-collinearity.

📍 Week 3: Exploratory Data Analysis (EDA) & Statistical Profiling
Strategic Focus: Extracted empirical relationship patterns across geographic regions and transit partners.
Key Achievements:
Correlation Mapping: Uncovered dominant positive linear dependency of distance_km ($r \approx 0.78$) and order_weight_kg ($r \approx 0.54$) on freight_cost_inr.
Vendor Benchmarking: Evaluated vendor delivery reliability vs. cost tiers, identifying higher cost variance in specific long-haul carrier corridors.
Data Visualizations: Built univariate distribution plots, bivariate scatter plots, and correlation heatmaps utilizing seaborn and matplotlib.

📍 Week 4: Predictive Modeling, Metric Evaluation & Optimization
Strategic Focus: Built, benchmarked, and evaluated machine learning models to forecast freight expenses and guide business strategy.
Key Achievements:
Model Implementations: Trained Multiple Linear Regression against Random Forest Regressor using an 80/20 train-test split cross-validation strategy.
Feature Importance Insights: Isolated distance_km (62%) and order_weight_kg (31%) as primary drivers of transport expenditure.

✅ Definition of Done (DoD) Verification
[x] Data Pipeline: Complete missing value imputation, outlier handling, and one-hot encoding.
[x] EDA & Profiling: Comprehensive statistical distribution charts and correlation heatmaps built.
[x] Predictive Machine Learning: Comparative evaluation of Linear Regression and Random Forest models.
[x] Evaluation Metrics: Quantitative metrics ($MAE$, $RMSE$, $R^2$) validated on test datasets.
[x] Enterprise Readiness: Professional documentation and clear repository structure ready for recruiter review.
Project developed as part of the YuvaIntern Logistics Analytics Program.
