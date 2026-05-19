# Time Series Analysis and Forecasting of Monthly Road Traffic Accidents

## Overview

This project analyses monthly road traffic accident counts in the UK from January 2020 to December 2024 using classical time series methods.

The analysis focuses on seasonality, stationarity, autoregressive structure, and short-term forecasting using a SARIMA model.

## Research Question

Can classical univariate time series models adequately capture the dynamics of road traffic accident data, or are more flexible models with external explanatory variables required?

## Methods

- Exploratory time series analysis
- Seasonal decomposition
- Augmented Dickey-Fuller stationarity test
- ACF and PACF diagnostics
- SARIMA(1,0,0)(1,0,0,12) modelling
- Twelve-month forecasting
- Qualitative comparison with a naive baseline forecast

## Data

The repository includes an aggregated monthly dataset derived from publicly available UK Department for Transport road safety statistics.

The original raw collision dataset is not redistributed because of its large file size. The included CSV contains monthly accident counts from January 2020 to December 2024 and is sufficient to reproduce the time series analysis.

## Key Findings

- The series shows a sharp decline in early 2020, likely related to reduced mobility during the COVID-19 pandemic.
- Seasonal decomposition suggests higher accident counts in late spring and summer and lower counts in winter.
- The Augmented Dickey-Fuller test suggests that the series is stationary.
- The SARIMA model captures short-term persistence and seasonal structure.
- Forecast uncertainty increases for longer forecast horizons.

## Limitations

The analysis is based on a univariate time series model and does not include external explanatory variables such as traffic volume, weather conditions, mobility patterns, or policy interventions.

Future work could extend the model using SARIMAX, tree-based machine learning models, or recurrent neural networks.

## Repository Structure

```text
traffic_accident_time_series.ipynb       Jupyter notebook with the analysis
traffic_accident_time_series_report.pdf  Project report
requirements.txt                         Python dependencies
README.md                                Project description
