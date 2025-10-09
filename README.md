# Retail Demand Analysis: Corporación Favorita
![Sample Forecast](Output/Forecast%20Result.png)

## Overview

This project explores the Corporación Favorita time series dataset, focusing on daily sales across multiple stores and items.
We deliberately narrowed the data to a smaller region and time window to create more efficient learning conditions and enable deeper feature experimentation.

We selected XGBoost as our main model, since it is robust with categorical and sparse data, supports advanced feature engineering, and is well-suited for structured tabular datasets like this one. We implemented Rolling Forecasts, simulating real future predictions rather than just retrospective evaluation. This approach makes the analysis closer to real-world forecasting scenarios.
Our best score is MAE: 50.34, RMSE: 68.23.

## Notebooks

- [Data Preparation](https://github.com/LenaGeller/Favorita-forecast/blob/main/Notebooks/data_prep_Perischable.ipynb)
Loads and cleans the data, applies filters to narrow region and timeframe, and saves prepared dataset for further use.

- [Feature Engineering](https://github.com/LenaGeller/Favorita-forecast/blob/main/Notebooks/Best_EDA_and_Feature_Engineering_Perishable.ipynb)
Explores the cleaned dataset, creates calendar, rolling, holiday, and promotion features, and handles missing values.

- [Forecast](https://github.com/LenaGeller/Favorita-forecast/blob/main/Notebooks/Best_MAE_October_Forecast_Produce_XGBoost.ipynb)
Trains and evaluates XGBoost models, including hyperparameter tuning and rolling forecast simulations. Shows how forecasts differ at item-store level compared to aggregated evaluation.

## Data

The prepared data files are stored in the Data/ folder of this repository.

## Outputs

Contains selected plots and results generated from the notebooks.

## Project Walkthrough
A detailed video explanation of the project can be found [here](https://drive.google.com/file/d/1Qbn7r3tcOXRRPrLXTFk3xRLPrR4OyeQr/view?usp=sharing).

