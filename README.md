# Store-Sales-Univariate-Time-Series-Forecasting


This project is about forecasting the sales of a product family at a given store. 
### Dataset Description
The training data, comprising time series of features store_nbr, family, and onpromotion as well as the target sales. store_nbr identifies the store at which the products are sold. family identifies the type of product sold. sales gives the total sales for a product family at a particular store at a given date. Fractional values are possible since products can be sold in fractional units (1.5 kg of cheese, for instance, as opposed to 1 bag of chips). onpromotion gives the total number of items in a product family that were being promoted at a store at a given date.

The test data, having the same features as the training data. You will predict the target sales for the dates in this file. The dates in the test data are for the 15 days after the last date in the training data.

## Goal
The goal of this project is to build a time series forecasting model that can accurately predict the sales of a product family at a given store for the next 15 days based on historical sales and promotional data.

### Dataset
The dataset used for this project is available on Kaggle: [dataset](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/)

The dataset contains two CSV files: train.csv and test.csv.

train.csv
This file contains the training data, comprising time series of features store_nbr, family, and onpromotion as well as the target sales.Sales gives the total sales for a product family at a particular store on a given date. Fractional values are possible since products can be sold in fractional units.

test.csv
This file contains the test data, having the same features as the training data. You will predict the target sales for the dates in this file. The dates in the test data are for the 15 days after the last date in the training data.

## Models
In this project, we have used three different models to forecast sales. These models are:

* CNN Model
* LSTM Model
* CNN-LSTM Model

**CNN Model**\
The CNN model takes the time series data as input and uses a 1D convolutional layer to extract features from the time series. The output of the convolutional layer is then passed through a fully connected layer and a final output layer to generate the forecast.

**LSTM Model**\
The LSTM model takes the time series data as input and uses a sequence of LSTM layers to extract features from the time series. The output of the LSTM layers is then passed through a fully connected layer and a final output layer to generate the forecast.

**CNN-LSTM Mode**l\
The CNN-LSTM model combines the advantages of both CNN and LSTM models. The time series data is first passed through a 1D convolutional layer to extract features.The output of the convolutional layer is then passed through a sequence of LSTM layers to extract temporal dependencies in the data. Finally, the output of the LSTM layers is passed through a fully connected layer and a final output layer to generate the forecast.

## Methodology
The methodology used in this project involves the following steps:

**Data preprocessing**: The first step is to preprocess the data to ensure that it is suitable for analysis. This involves tasks such as data cleaning, imputation of missing values, and feature engineering.

**Exploratory data analysis**: The next step is to perform exploratory data analysis to gain insights into the data and identify any patterns or trends that may exist.

**Time series forecasting model selection**: Once the data has been preprocessed and explored, the next step is to select a suitable time series forecasting model such as the CNN, LSTM, and CNN-LSTM models for time series forecasting.

**Model training and evaluation**: The selected model is then trained on the training data and evaluated using a suitable performance metric such as appropriate evaluation metrics like Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), or Mean Absolute Percentage Error (MAPE).

![image](https://user-images.githubusercontent.com/130960032/232423271-cb4eef09-0e0c-46b1-9bea-8daa095af9ef.png)

### -------
### Tools Used
The following tools were used in this project:

Python\
Pandas\
NumPy\
Scikit-learn\
Matplotlib\
TensorFlow/Keras
### Files

'store_sales_forecasting.ipynb': a Jupyter Notebook containing the code for this project

### Conclusion
This project involves building a time series forecasting model to predict the sales of a product family at a given store. The data used in this project is provided by Kaggle and consists of historical sales and promotional data. The methodology used in this project involves data preprocessing, exploratory data analysis, time series forecasting model selection, model training and evaluation, and model deployment. The final model can be used to make predictions about future sales based on historical data.
