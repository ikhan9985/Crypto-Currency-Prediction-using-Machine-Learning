# Crypto-Currency-Prediction-using-Machine-Learning

## README
This Jupyter notebook contains code for extracting historical price data for Ethereum (ETH) from the CryptoCompare API, creating a machine learning model to predict the price of ETH based on the historical data, and storing the predictions in a SQLite database.

* Dependencies
* requests
* json
* pandas
* scikit-learn
* matplotlib
* sqlite3
Make sure to install these dependencies before running the code.

# Code Overview
## Cell1
* Imports the necessary libraries (requests and json)
* Defines the endpoint and parameters for the CryptoCompare API request
* Makes the API request and parses the response
* Prints the historical data extracted from the API

## Cell2
* Imports the necessary library (pandas)
* Loads the historical data into a pandas DataFrame
* Converts the DataFrame to a CSV file

## Cell3
* Imports the necessary libraries (scikit-learn and pandas)
* Loads the historical data from the CSV file into a pandas DataFrame
* Defines the features and target for the machine learning model
* Splits the data into training and test sets
* Creates a Linear Regression model
* Trains the model on the training data
* Uses the model to make predictions on the test data

## Cell4
* Evaluates the performance of the machine learning model on the test data
* Prints the R-squared score of the model

## Cell5
* Makes predictions using the trained model
* Converts the predictions to a DataFrame
* Imports the necessary library (sqlite3)
* Connects to a SQLite database
* Stores the predictions in a SQLite table

## Cell6
* Reads the 'predictions' table from the SQLite database into a pandas DataFrame
* Prints the first 5 rows of the DataFrame

## Cell7
* Imports the necessary libraries (scikit-learn, math, and matplotlib)
* Calculates the Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE) of the machine learning model on the test data
* Prints the results

## Cell8
* Imports the necessary library (scikit-learn)
* Calculates the R-squared score of the machine learning model on the test data
* Prints the R-squared score


Note: The code in Cell1 to Cell4 extracts the historical data from the API and trains the machine learning model. The code in Cell5 to Cell7 stores the predictions in a SQLite database and evaluates the performance of the machine learning model on the test data. If you only want to extract the historical data and train the machine learning model, you can skip Cell5 to Cell7. If you only want to store the predictions in a SQLite database and evaluate the performance of the machine learning model on the test data, you can skip Cell1 to Cell4.
