# Stock Market Direction Prediction with ML Models

## Overview

This project builds a machine learning pipeline to predict the directional movement of a major ETF (VOO) based on engineered financial indicators. It evaluates multiple classification models and tracks their predictive accuracy and real-world performance.

## Business Relevance

Understanding and forecasting stock market trends — even in directional terms — can significantly impact:
- Investment timing and portfolio allocation
- Risk mitigation strategies
- Automated trading signals

This kind of model can be used to trigger alerts, support backtesting in trading platforms, or assist retail investors in decision-making.

## Tools & Technologies Used

- Python, pandas, yfinance, matplotlib, seaborn
- Scikit-learn for preprocessing and modeling
- XGBoost for gradient-boosted classification
- Logistic Regression and Support Vector Machines
- Confusion matrices and ROC AUC for evaluation

## Problem Statement

Can we accurately predict whether the price of a major market ETF (VOO) will go up or down tomorrow, based on technical indicators and recent price movements?

## Approach

1. **Feature Engineering**
   - Computed indicators like open-close difference, daily volatility (low-high), and quarter-end flags
   - Added lag features to capture short-term trends

2. **Data Preparation**
   - Retrieved historical data using Yahoo Finance
   - Scaled features and split into training/testing datasets

3. **Model Training**
   - Evaluated Logistic Regression, SVM, and XGBoost Classifier
   - Used ROC AUC to evaluate performance of each

4. **Iterative Prediction**
   - Built a simulation to predict stock direction for the next 60 business days using rolling lag updates
   - Compared confidence levels from multiple models

## Results

- XGBoost provided the highest ROC AUC on validation data
- Simulated future probabilities can assist in risk-aware decision making
- Model generalization was tested by using predictions iteratively over multiple days

## Future Improvements

- Incorporate macroeconomic indicators (e.g., CPI, interest rates)
- Use Recurrent Neural Networks (RNNs) or transformers for sequence learning
- Add backtesting module for simulated portfolio performance

## Contact

For firms or analysts interested in building stock prediction pipelines or enhancing financial modeling capabilities, feel free to reach out:

**Email**: [mmgupta2@wisc.edu](mailto:mmgupta2@wisc.edu)  
**LinkedIn**: [linkedin.com/in/mihirmgupta](https://www.linkedin.com/in/mihirmgupta/)

