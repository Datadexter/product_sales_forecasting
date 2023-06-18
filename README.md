# Product Sales Forecasting in Python

This project implements a time series forecasting model using Prophet to predict the future sales of a product. The goal is to improve forecast accuracy compared to a baseline model. The dataset used in this project contains 500,000 sales records.

## Overview

The code in this repository performs the following steps:

1. Loads the sales data from the CSV file.
2. Preprocesses the dataset by converting the date column to a pandas DateTime format and converting the sales values to numeric type.
3. Splits the dataset into train and test sets, with 80% of the data used for training and the remaining 20% for testing.
4. Performs hyperparameter tuning to find the optimal hyperparameters for the Prophet model using grid search and cross-validation.
5. Trains the best model on the entire training set with the optimized hyperparameters.
6. Generates future dates for forecasting.
7. Performs the forecasting using the best model.
8. Evaluates the model by calculating the mean absolute error (MAE) for both the baseline model and the Prophet model.
9. Calculates the improvement in forecast accuracy compared to the baseline model.
10. Plots the actual vs. predicted sales values for visualization.
11. Prints the improvement in forecast accuracy and the best hyperparameters found.

## Getting Started

To run the code on your local machine, follow these steps:

1. Clone this repository to your local machine.
2. Ensure you have Python 3 and the required libraries installed.
3. Place the "sales_data.csv" dataset file in the same directory as the code file.
4. Open a terminal or command prompt and navigate to the project directory.
5. Run the code using the command: `python sales_forecasting.py`.
6. View the improvement in forecast accuracy and the best hyperparameters printed on the console.
7. The plot showing the actual vs. predicted sales values will also be displayed.

## Dependencies

The code relies on the following libraries:

- `pandas`: For data manipulation and analysis.
- `fbprophet`: For time series forecasting with Prophet.
- `sklearn`: For hyperparameter tuning and evaluation metrics.
- `matplotlib`: For data visualization.

Install these dependencies using the following command:

```shell
pip install pandas fbprophet scikit-learn matplotlib
