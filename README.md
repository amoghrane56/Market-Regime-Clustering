# Market Regime Clustering using Gaussian Mixture Models (GMM)

## Overview

This project aims to identify distinct financial market regimes by applying Gaussian Mixture Models (GMM) to time-series data from the Nifty 50 index. The objective is to uncover hidden market states or regimes that can inform regime-specific investment strategies.

## Features

- **Market Regime Identification**: Use GMM to classify market regimes based on historical returns.
- **Visualization**: Plot the identified regimes over time with filled areas for each regime.
- **Performance Metrics**: Evaluate the model using BIC (Bayesian Information Criterion) and AIC (Akaike Information Criterion) scores.
- **Switch Frequency Analysis**: Calculate the average number of regime switches per year.

## Data

The data used in this project is sourced from the Nifty 50 index. The data file (`nifty50.xlsx`) should contain at least two columns:
- `Date`: The date of the observation.
- `Close`: The closing price of the Nifty 50 index.


Usage
1. Load and Preprocess Data:
Load the Nifty 50 data from an Excel file, calculate rolling percentage changes, and drop NaN values.

2. Model Training:
Train a Gaussian Mixture Model to identify market regimes.

3. Regime Prediction:
Use the trained model to predict market regimes and calculate the frequency of regime switches.

4. Visualization:
Plot the closing prices with filled areas representing different market regimes.


Evaluation
The model's performance is evaluated using BIC and AIC scores. Lower scores indicate a better model fit.

1. BIC: Bayesian Information Criterion
2. AIC: Akaike Information Criterion
