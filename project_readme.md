# Delivery Delay and Supply Chain Operations Analytics

## Overview

This repository houses an end-to-end supply chain analytics pipeline and predictive modeling framework designed to evaluate delivery performance, isolate fulfillment bottlenecks, and mitigate late shipment risks. Utilizing enterprise-grade transaction records from the DataCo Global Supply Chain dataset, this project translates raw logistics data into actionable operational insights and executive-level intelligence.

The project addresses a critical enterprise challenge: maintaining delivery predictability across global distribution networks. By evaluating fulfillment timelines, inventory movement across sectors, and modal efficiencies, the analysis provides a structured diagnostic tool for supply chain managers.

---

## Technical Stack and Dependencies

* **Programming Language:** Python
* **Data Manipulation & Processing:** Pandas, NumPy
* **Data Visualization:** Plotly Express, Plotly Graph Objects (Subplots)
* **Predictive Modeling:** Scikit-Learn (Decision Tree Classifier, Label Encoding, Train-Test Split)
* **Development Environment:** Google Colab / Jupyter Notebook

---

## Core Analytical Milestones

### 1. Data Ingestion, Cleaning, and Feature Engineering
* Processed over 180,000 transaction records, handling missing values and standardizing structural schemas.
* Engineered a binary target variable (`is_late`) to categorize fulfillment status based on delivery benchmarks.
* Computed explicit operational delay gaps (`delay_gap_days`) by calculating the arithmetic difference between actual shipping duration and scheduled delivery expectations.

### 2. Logistics Performance and Mode Segmentation
* Evaluated delivery efficacy across shipping tiers (Standard, Second Class, First Class, and Same Day).
* Uncovered a critical systemic anomaly: **First Class** shipping exhibited an unexpected failure rate exceeding **95%**, highlighting significant vulnerability in premium distribution channels.

### 3. Departmental and Warehouse Hotspot Analysis
* Segmented failure rates across product departments, identifying **Pet Shop** (58.9%) and **Book Shop** (56.5%) as primary operational bottlenecks.
* Isolated specific high-risk operational intersections, uncovering severe systemic breakdowns (e.g., 100% delay clustering within specific high-priority fulfillment pathways).

### 4. Predictive Risk Modeling
* Deployed a Scikit-Learn Decision Tree Classifier to predict late delivery probability based on operational features (shipping mode and department classifications).
* Achieved an overall model accuracy of **69.16%**, demonstrating strong predictive precision (`0.84`) for identifying high-risk delivery outcomes prior to dispatch.

---

## Executive Mini-Dashboard Architecture

The project integrates an executive-level analytical dashboard featuring:
* **High-Level KPI Banner:** Aggregated metrics tracking total volume, aggregate delay counts, enterprise-wide on-time delivery percentages, and mean delay gap durations.
* **Comparative Subplots:** Side-by-side comparative visualizations mapping failure distributions across transport modes and corporate departments to support rapid executive decision-making.

---

## Repository Structure

```text
├── Delivery_Delay_Operations_Analytics.ipynb   # Complete Google Colab analytical notebook
├── DataCoSupplyChainDataset.csv              # Underlying raw supply chain dataset
└── README.md                                 # Technical project documentation
```

---

## Execution Guide

1. Open a cloud notebook environment such as [Google Colab](https://colab.research.google.com/).
2. Upload the `Delivery_Delay_Operations_Analytics.ipynb` file and the `DataCoSupplyChainDataset.csv` source file.
3. Execute the code cells sequentially to replicate data preprocessing steps, interactive visual analyses, and the machine learning model.