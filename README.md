# Stock Price Forecast

## Problem statement
Stock market prediction aims to determine the future movement of the stock value of a financial exchange. The accurate prediction of share price movement will lead to more profit investors can make. Predicting stock prices is an uncertain task which is modelled using machine learning to predict the return on stocks. Over the years, various machine learning techniques have been used in stock market prediction, but with the increased amount of data and expectation of more accurate prediction, the deep learning models are being used nowadays which have proven their advantage over traditional machine learning methods in terms of accuracy and speed of prediction.

## Getting started
In this project, the future stock prices of Bombay Stock Exchange (BSE) are predicted using the LSTM Recurrent Neural Network. Our task is to predict stock prices for a few days, which is a time series problem. The LSTM model is very popular in time-series forecasting, and this is the reason why this model is chosen in this task. 

## Implementation
These are the steps which I followed to make this project:
1. Import the required libraries
2. Fetch 5 years of historical data from 10-10-2016 to 10-10-2021 of BSE from yahoo finance 
3. Preprocess the data in order to prepare it for the LSTM model
4. Create data with timesteps
5. Build the LSTM model: In order to build the LSTM, we need to import couple of modules from Keras- **Sequential** for initializing the neural network; **Dense** for adding a densely connected neural network layer; **LSTM** for adding the Long Short-Term Memory layer
6. We add the LSTM layer with the following arguments: **50 units** which is the dimensionality of the output space; **return_sequences=True** which determines whether to return the last output in the output sequence, or the full sequence; **input_shape** as the shape of our training set.
7. We add the Dense layer that specifies the output of 1 unit. After this, we compile our model using the popular adam optimizer and set the loss as the mean_squarred_error. This will compute the mean of the squared errors. Next, we fit the model to run on 100 epochs with a batch size of 41.


Data source: [Yahoo Finance](https://finance.yahoo.com/quote/%5EBSESN/history?p=%5EBSESN)
