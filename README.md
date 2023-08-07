# Bitcoin Time Series Prediction with LSTM Models

Welcome to the Bitcoin Time Series Prediction project! In this repository, you'll find a collection of LSTM-based models designed to predict Bitcoin's price using historical data. Whether you're a crypto enthusiast, a data scientist, or just curious about predictive modeling, this project offers a fascinating journey into forecasting the dynamic world of cryptocurrency.

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Models](#models)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [Contributing](#contributing)

## Introduction

Cryptocurrency markets, especially Bitcoin, have captured the imagination of investors and researchers alike due to their highly volatile nature. Predicting Bitcoin's price movements can be a challenging yet rewarding endeavor. This project explores the application of Long Short-Term Memory (LSTM) neural networks, a type of recurrent neural network (RNN), to forecast Bitcoin prices.

## Data

The dataset used in this project is named `BTCUSDKRAKEN.csv`, which contains preprocessed Bitcoin price and trading volume data. We've carefully prepared the data, focusing on relevant columns like "Weighted Price," "Volume (BTC)," and "Volume (Currency)" to provide a comprehensive input for our models.

## Models

### Model 1 - Single Layer LSTM

The first model utilizes a straightforward architecture comprising a single LSTM layer followed by a Dense(1) output layer. This model provides a solid baseline for predicting Bitcoin prices using the "Weighted Price" feature.

### Model 2 - Multi-Layer LSTM

In this more complex configuration, we introduce a deeper architecture. The model consists of an LSTM layer followed by Dense(1), Dense(4), and Dense(1) layers. This setup enables the model to capture intricate temporal dependencies and potentially enhance prediction accuracy.

### Model 3 - Incorporating Additional Features

Recognizing that Bitcoin's price is influenced by more than just historical prices, we extend our analysis to include "Volume (BTC)" and "Volume (Currency)" features. Model 3 employs a similar single-layer LSTM architecture as Model 1 but uses a broader input.

### Model 4 - Enriched Multi-Layer LSTM

Expanding upon Model 2, this variant integrates the additional volume-related features. The architecture includes an LSTM layer followed by Dense(1), Dense(4), and Dense(1) layers. This model aims to leverage a wider range of input features for improved predictions.

## Evaluation

For each model, we employ two common evaluation metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

By assessing these metrics, we gauge the performance of our models and compare their predictive capabilities.

## Usage

To replicate or build upon our work, follow these steps:

1. Clone this repository to your local machine.
2. Ensure you have the required dependencies installed (you can find these in the code files).
3. Open the code files for each model to study the architecture, preprocessing steps, and evaluation metrics.
4. Feel free to modify, experiment, and adapt the models to suit your needs.

## Contributing

Your contributions are highly valued and encouraged! If you're inspired to enhance our models, explore new features, or fine-tune parameters, we welcome your input. Fork this repository, make your improvements, and submit a pull request. Let's collaborate to refine the art of Bitcoin price prediction!

Happy coding and predicting! 🚀📈
