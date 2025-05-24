# Time Series Forecasting for Retail Sales

## Overview
This project uses advanced time series modeling to forecast daily sales for a chain of retail stores, incorporating calendar effects, oil prices, holidays, and store-level metadata. The final model is designed to generate accurate predictions at scale for multiple locations across time.

## Business Relevance
Accurate demand forecasting enables retailers to:
- Optimize inventory and reduce overstocking or stockouts
- Align staffing with expected traffic
- Improve supply chain efficiency
- Make data-driven revenue projections

This solution can be directly adapted by retail chains, e-commerce platforms, or logistics companies looking to improve planning and operational agility through predictive analytics.

## Tools & Technologies Used
- Python, NumPy, pandas
- Statsmodels for ARIMA modeling, PACF, ACF
- LightGBM for boosting-based forecasting
- Plotly & Seaborn for exploratory visualizations
- Custom helper module for data wrangling and submission formatting

## Problem Statement
Given historical sales data across hundreds of stores in Ecuador, the task is to forecast daily sales for the next several weeks. The data includes:
- Store metadata
- Local/national holiday calendars
- Oil price fluctuations
- Sales and transactions history

## Approach
1. **Exploratory Data Analysis**
   - Trends and seasonality were analyzed at both store and category levels.
   - Holiday effects and oil prices were examined for correlation with sales.

2. **Feature Engineering**
   - Created lag-based features and calendar-derived features (e.g., weekday, month-end).
   - Incorporated oil prices, national/local holidays, and events.

3. **Modeling**
   - Applied ARIMA models for individual time series analysis.
   - Tuned and trained LightGBM models using a custom RMSLE loss function to handle skewed sales values.
   - Cross-validation strategies were used to ensure robustness across time.

4. **Evaluation**
   - Performance was evaluated using Root Mean Squared Logarithmic Error (RMSLE).
   - Submission files were generated for downstream leaderboard validation.

## Results
- Final validation RMSLE: **0.87**
- Model showed strong performance across both high-traffic and low-traffic stores.
- Interactive plots helped visualize forecast vs. actual trends.

> Note: Some data paths reference Kaggle directories. Modify for local use if needed.

## Future Improvements
- Integrate Prophet or transformer-based forecasting models
- Automate feature pipelines for real-time forecasting
- Deploy as an API or Streamlit dashboard for stakeholder use

## Contact
If you're a business looking to implement similar forecasting solutions, feel free to reach out:

**Email**: [mmgupta2@wisc.edu](mailto:mmgupta2@wisc.edu)  
**LinkedIn**: [linkedin.com/in/mihirmgupta](https://www.linkedin.com/in/mihirmgupta/)

