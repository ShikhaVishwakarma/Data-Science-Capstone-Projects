Collected Bombay Stock Exchange stock price data of five years using yfinance. Normalized the data using
MinMaxScalerto scale the value of the data between 0 and 1. Created a stacked LSTM model having two
hidden layers. Mean squared erroris used as the loss function and adam is used as an optimizer. Trained the
model to forecast the stock price of next 10 days in future.

Data source: [Yahoo Finance](https://finance.yahoo.com/quote/%5EBSESN/history?p=%5EBSESN)
