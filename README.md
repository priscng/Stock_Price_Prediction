# Stock Price Prediction


## Objective
Stock price forecasting is a challenging topic in the finance industry as the stock market is very volatile and there are many factors that can affect the stock price. The aim for this project is to use neural network to develop a model that can accurately predict the prices.

For this project, we will focus on Google stock price and will explore to develop a model using Long Short Term Memory (LSTM).


## Methodology
- Extract stock price using Alpha Vantage API and pandas datareader.
- Explore the data and create visualization.
- Perform modeling using LSTM.
- Improve model performance.
- Perform prediction on test dataset.


## Dataset
The Google stock price data is extracted from Yahoo Finance using pandas datareader. A total of 2721 stock prices is extracted with no missing data.

For price prediction, we will be using the adjusted close price to remove any artificial price turbulences due to stock splits and dividend payout events.


## Modeling Results
The predicted stock prices follow the trend of the real stock prices quite closely which shows LSTM is an effective method to work with time series data like the stock prices. From the experiment, the model with 100 nodes and 0.005 learning rate obtained the lowest RSME score.

|Model   | Nodes No. | Learning Rate  | RSME |
|:-------|:----------|:---------------|:-----|
|1       |50         |0.001           |4.6982
|2       |100        |0.001           |2.9253
|3       |100        |0.0001          |5.153
|4       |100        |0.01            |19.4969
|5       |100        |0.005           |2.0803


## Conclusions
In this project, we used LSTM to predict the Google stock price. LSTM has proven to be an effective method to work with time series data like the stock prices. We have also improved the model performance by increasing the number of nodes to 100 and learning rate to 0.005.


## Limitations and Future Plans
The price prediction model uses historical prices to make predictions. Stock prices, however, may also be affected by other factors, such as the economy and other unforeseen circumstances, which are not taken into account by the machine learning algorithm. So, a model for predicting stock prices cannot be used as the sole basis for determining an investment decision. To make a sound investment decision, more market analysis is required.

Moving forward, we can explore sentiment analysis using social media platforms and analyze whether the stock is of interest to the public, which might increase the price and this data can be used for investment decisions. We can also try to vary the different number of layers with different nodes and use other optimizers (e.g. SGD) to check if the model performance can be further improved.
