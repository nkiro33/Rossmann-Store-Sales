# Rossmann Store Sales Prediction

## Introduction
This repository is dedicated to forecasting daily sales for 1,115 Rossmann stores located across Germany. The objective is to provide store managers with accurate sales predictions up to six weeks in advance, aiding in efficient staff scheduling and inventory management. This project utilizes LSTM (Long Short-Term Memory) networks to model time series sales data influenced by promotions, holidays, seasonality, and other factors.

## Dataset
The dataset used in this project is the Rossmann Store Sales dataset, available on Kaggle. It comprises historical sales data, store information, and promotional details. The challenge is to predict six weeks of daily sales for different stores, factoring in various sales influencers.

## data-proc.ipynb
Objective: The primary goal of this notebook is to prepare the raw data for modeling. It focuses on cleaning, transforming, and feature engineering necessary to optimize the dataset for the forecasting model.

### Key Features:

__Data Cleaning__: Addresses missing values, removes outliers, and fixes data inconsistencies to ensure the quality and reliability of the dataset.
__Feature Engineering__: Enhances the dataset with new features derived from existing data, such as time components (e.g., day of the week, month, year) and store-specific attributes, which are critical for understanding sales patterns.
__Data Merging__: Combines multiple data sources into a single dataset, aligning store information with historical sales and promotional details, providing a holistic view of each store's context.
Encoding and Scaling: Applies necessary transformations such as one-hot encoding for categorical variables and normalization or scaling for numerical features to prepare the data for neural network processing.
__Outcome__: The notebook outputs a preprocessed dataset ready for training and testing in the machine learning model, ensuring that the data is in the proper format and structure to optimize model performance.

## Rossman_LSTM.ipynb
Objective: This notebook is dedicated to developing and evaluating the LSTM model to forecast daily sales for Rossmann stores. It focuses on constructing a time series forecasting model that accounts for various features influencing sales.

### Key Features:

__Model Architecture__: Outlines the structure of the LSTM network, including the number of layers, units per layer, activation functions, and other relevant hyperparameters tailored to time series forecasting.
Data Preparation: Describes how the preprocessed data is split into training and validation sets, ensuring that the model can learn from a representative sample and be evaluated on unseen data.
__Training and Evaluation__: Details the process of training the LSTM model, including setting the loss function, optimizer, and evaluation metrics. It also explains the methodology for assessing the model's performance on the validation set.
__Feature Importance__: Analyzes the impact of various features on the model's predictions, offering insights into which factors most significantly influence sales forecasts.
__Predictions and Analysis__: Demonstrates how to use the trained model to make sales forecasts and provides an analysis of the results, comparing predicted values with actual sales data to gauge accuracy.
__Outcome__: The notebook results in a trained LSTM model capable of forecasting future sales for the Rossmann stores. It provides a detailed evaluation of the model's performance and insights into the sales dynamics captured by the model.

Both notebooks together provide a comprehensive approach to solving the Rossmann Store Sales forecasting challenge, from raw data processing to developing and evaluating a sophisticated time series forecasting model. 
