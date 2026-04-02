# Automating-EDA-with-GenAI-and-Python-Digital-Marketing-Campaign-Analytics

I automated EDA & Feature Engineering pipeline using Python and GenAI (LLMs). I reduced manual analysis time by ~40%. I was also able to optimize a $1.1M marketing budget by identifying behavioral 'High-Intent' customers towards the growth of the organization based on machine learning predictions.

## Project Overview
This project demonstrates an AI-augmented approach to Exploratory Data Analysis (EDA) and Feature Engineering. By integrating GenAI (LLM/RAG workflows) with Python, I automated the identification of hidden behavioral drivers within a high-dimensional digital marketing dataset (20+ variables). The goal was to accelerate the "Time-to-Insight" for campaign optimization and budget allocation.

## The Problem: The "Human Bottleneck" in EDA
Traditional EDA for multi-channel marketing campaigns **often takes days of manual slicing and dicing**. Identifying non-obvious correlations, such as **why conversion is driven by Time on Site and Loyalty Points rather than traditional demographics like Age or Income is often missed in standard manual workflows**.

## The Solution: GenAI-Augmented Workflow
I architected an automated EDA pipeline using Python and Large Language Models (LLMs) to handle:
- Automated Data Cleaning: Used **LLMs** to map inconsistent campaign channel names and handle missing values in the dataset.
- Rapid Feature Discovery: Leveraged LLMs to query data schemas and automatically generate hypotheses for multivariate testing.
- Imbalance Detection: Instantly identified an 85/15 conversion imbalance, allowing for immediate application of SMOTE/resampling techniques before model training.

## Technical Stack
Language: Python (Pandas, NumPy, Matplotlib, Seaborn)

## Data Source
Data Techcon dataset includes schemas such as, Customer ID, Ad Spend, Conversion Rate, Time on Site, etc.

## Methodology
The approach followed these three core phases:
- **Phase 1: Foundational Benchmarking** – Established performance baselines using Logistic Regression for conversion and Simple Linear Regression for Customer Lifetime Value (CLV) to provide a grounded starting point for model comparison.
- **Phase 2: High-Performance Modeling** – Implemented a dual-stream predictive architecture using XGBoost for precise conversion classification and Random Forest Regression to predict long-term CLV.
- **Phase 3: Refinement & Insight Synthesis** – Performed hyperparameter tuning to reach 84.2% model accuracy and utilized binned behavioral analysis to identify the "Golden Threshold" for user engagement.
**This end-to-end process was managed using Python for ETL and feature engineering, with Power BI serving as the final platform for executive and strategic data visualization**.

## Key Insights
- I found that the Behavior > Demographics: That is, **'Loyalty Points'** and **'Time on Site'** had a **3.5x higher correlation with conversion than Age or Income**.
- Results revealed that **60% of our current pay per click (PPC) and Social spend is being exhausted on "Low Priority"** segments with less than a 10% conversion probability
- Discovered a massive **4.2x increase in conversion once a user crosses the 3.5-minute threshold on the website**. However, **most users currently drop off at just 2.2 minutes**, missing this "Golden Threshold".
- Revealed that the **'Referral channel'** generates the **highest user equity at ~$220K** compared to other channels.

<img width="1651" height="917" alt="image" src="https://github.com/user-attachments/assets/704eaea0-c987-44dc-9d9e-92205460bf6e" />
<img width="1642" height="913" alt="image" src="https://github.com/user-attachments/assets/e8f7fe20-5f7b-4c3b-a7db-18d81180c525" />


  
## Business Impact
- 40% Reduction in manual data processing and cleaning time.
- Optimized $1.1M Ad Spend by shifting focus from low-intent demographic segments to high-intent behavioral segment.
- Improved Decision Speed: Provided the Head of Growth with real-time anomaly detection and Predicted ROI metrics.

## Recommendations
- Shift 15% ($6M) of the current marketing budget away from "Low Priority" segments & re-allocate it to retarget the High-Intent customers.
- Implement interactive features on the site to increase "Time on Site" from the current 2.2-minute average to at least 4 minutes, as crossing the 3.5-minute "Golden Threshold" triggers a 4.2x increase in conversion probability.
- Launch a specialized "Refer-a-Friend" incentive program targeting the top 5% of loyalty point holders to capitalize on the Referral channel, which are the highest concentration of VIP customers (over 40%) and drives 24.8% of total expected revenue.
