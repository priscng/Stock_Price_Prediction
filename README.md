# Stock Price Prediction


## Objective
Stock price forecasting is a challenging topic in the finance industry as the stock market is very volatile and there are many factors that can affect the stock price. The aim for this project is to use neural network to develop a model that can accurately predict the prices.

For this project, we will focus on Google stock price and will explore to develop a model using Long Short Term Memory (LSTM).


## Methodology
- Extract stock price using Alpha Vantage API and pandas datareader.
- Explore the data and create visualization.
- Perform modeling using LSTM.
- Perform prediction on test dataset.


## Dataset
The Google stock price data is extracted from Yahoo Finance using pandas datareader. A total of 2721 stock prices is extracted with no missing data.

For price prediction, we will be using the adjusted close price to remove any artificial price turbulences due to stock splits and dividend payout events.


## Modeling Result
The predicted stock prices follow the trend of the real stock prices quite closely. The RSME of 3.4986 is relatively low also. This shows LSTM is an effective method to work with time series data like the stock prices.


## Conclusions
In this project, we used LSTM to predict the Google stock price. LSTM has proven to be an effective method to work with time series data like the stock prices and a low RSME score of 3.4986 is obtained. We have also compared the model performance between a 30-days vs. a 60-days window period of historical prices and the results are comparable.


## Limitations and Future Plans
The price prediction model uses historical prices to make predictions. Stock prices, however, may also be affected by other factors, such as the economy and other unforeseen circumstances, which are not taken into account by the machine learning algorithm. So, a model for predicting stock prices cannot be used as the sole basis for determining an investment decision. To make a sound investment decision, more market analysis is required.

Moving forward, we can explore sentiment analysis using social media platforms and analyze whether the stock is of interest to the public, which might increase the price so that the data can be used for investment decisions.
