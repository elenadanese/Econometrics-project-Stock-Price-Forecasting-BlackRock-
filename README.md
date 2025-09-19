## Econometrics project: Stock Price Forecasting (BlackRock)
## Project Overview

This group project, developed within the Econometrics course at the University of Padua, focused on forecasting the stock price of BlackRock and analyzing its volatility. A key feature of the assignment was the freedom granted to students: our team independently selected both the stock to forecast (BlackRock) and the exogenous variables to integrate (S&P500 index and VIX). Similarly, we decided which econometric models to implement, allowing us to design a tailored methodology that balanced theory with practical data analysis.

## Objectives

Forecast BlackRock stock prices using econometric methods.
Perform volatility modeling and risk assessment in financial time series.
Compare models in terms of forecast accuracy, robustness, and interpretability.
Investigate the role of external variables (S&P500, VIX) in improving predictive performance.
Bridge theory and practice by iteratively applying models and validating results on real financial data.

## Methodology

The project was implemented in R over multiple weeks, with progressively more advanced models being tested and compared. The analysis was structured in phases:
- Data preprocessing and stationarity checks
    -  Historical data: BlackRock prices (2014–2025).
    -  Transformations: differencing and log-returns.
    -  Statistical tests (ADF, Ljung-Box, Jarque-Bera) to assess stationarity, autocorrelation, and normality.

- Baseline models
    -  ARIMA / ARMA models for short-term price forecasting.
    -  Iterative specification, with diagnostics to refine model parsimony.

- Volatility modeling
    -  GARCH-family models to capture volatility clustering.
    -  Variants tested:
         -  Standard GARCH
         -  TGARCH and EGARCH (to account for asymmetry and leverage effects)
         -  Models under different error distributions (Normal, Student-t, skewed-t).

- ARMA-GARCH integrated models
    -  Joint estimation of mean and volatility processes.
    -  Comparison of competing specifications using AIC/BIC, log-likelihood, and residual analysis.

- Multivariate approaches
    -  VAR models to analyze dynamic interactions between BlackRock, S&P500, and VIX.
    -  Forecasting performance assessed against univariate benchmarks.

## Technologies

The project was entirely developed in R. We used the following main packages, grouped by purpose:
- Data Management & Visualization: readxl, here, ggplot2
- Stationarity & Statistical Tests: tseries, fBasics
- Time Series Forecasting: forecast, stats
- Volatility Modeling (GARCH-family): rugarch, fGarch
- Multivariate Models: vars

This was a group project, carried out collaboratively with fellow students. The teamwork aspect was crucial for: sharing model insights and coding strategies, critically interpreting results, and reaching common solutions through discussion and comparison.
