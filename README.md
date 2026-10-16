# Delivery Delay & Operations Analytics

## Overview
This project provides a comprehensive supply chain and logistics analysis using specialized operations datasets to identify fulfillment bottlenecks, evaluate late delivery rates, and implement predictive risk models[cite: 9]. The pipeline covers data cleaning, custom metric calculations, interactive data visualizations, and machine learning classification to forecast operational risks[cite: 9].

## Key Objectives & Methodology
1. **Data Integration & Error Handling:** Loaded and processed enterprise supply chain datasets, configuring error-handling protocols and validating schema integrity.
2. **Core Operations Metrics:** Calculated promised versus actual delivery dates, delay gap days, and on-time delivery percentages.
3. **Segmented Analytics:** Performed exploratory data analysis across shipping modes, departments, product types, days of the week, seasons, warehouse blocks, and regional markets.
4. **Hotspot Analysis:** Isolated high-failure operational combinations (such as specific shipping-tier and department breakdowns) experiencing systemic delays.
5. **Predictive Machine Learning:** Trained a Scikit-Learn Decision Tree Classifier to estimate delivery delay risk based on operational features.
6. **Executive Mini-Dashboard:** Designed consolidated KPI summaries and side-by-side comparative subplots for executive presentation.

## Key Performance Indicators (KPIs) & Metrics
* **Total Orders Analyzed:** High-volume logistics transactions evaluated across global markets.
* **On-Time vs. Late Delivery Rates:** Quantified fulfillment friction across specific operational tiers.
* **Average Delay Gap:** Measured in days between promised fulfillment windows and actual delivery timestamps.
* **Decision Tree Model Accuracy:** Achieved ~69% overall classification accuracy with high precision (0.84) for flagging high-risk late shipments.

## Exploratory Data Analysis & Visualizations
* **Shipping Mode Bottlenecks:** Evaluates failure rates across shipping classes, highlighting severe degradation in premium tiers (e.g., First Class fulfillment failures).
* **Department & Category Breakdowns:** Identifies specific product departments (such as Pet Shop and Book Shop) suffering from the highest late delivery percentages[cite: 9].
* **Temporal & Seasonal Patterns:** Analyzes day-of-week and seasonal variations to isolate temporal fulfillment constraints.
* **Warehouse & Regional Distribution:** Assesses warehouse block efficiency and geographic market routes to pinpoint regional logistics bottlenecks.

## Strategic Business Recommendations
* **Restructure Premium Shipping Tiers:** Given that certain first-class shipping routes exhibit critical failure rates, carrier agreements and handling workflows require immediate operational auditing.
* **Proactive Risk Mitigation:** Integrate the Decision Tree classification model into order management systems to flag high-risk shipments *before* dispatch, enabling preemptive customer communication or carrier rerouting.
* **Warehouse Resource Reallocation:** Target fulfillment optimizations toward underperforming warehouse blocks and high-friction departments to stabilize throughput times.

## Tech Stack
* **Python** (Pandas, NumPy, Scikit-Learn)[cite: 9]
* **Google Colab** (Execution environment)[cite: 9]
* **Plotly** (Interactive data visualization & subplots)[cite: 9]
