# Stock Price Prediction Flipr Hackathon 5.0
Stock market prediction is the act of trying to determine the future value of a company stock
or other financial instrument traded on an exchange. The successful prediction of a stock's
future price could yield significant profit. The efficient-market hypothesis suggests that stock
prices reflect all currently available information and any price changes that are not based on
newly revealed information thus are inherently unpredictable. Others disagree and those
with this viewpoint possess myriad methods and technologies which purportedly allow them
to gain future price information.

Ever since COVID 19 strike, markets loom under fear as uncertainty prevails. lt has sent
markets around the world crashing to levels not witnessed since the Global Financial Crisis
of 2008. Following the strong correlation with the trends and indices of the global market as
BSE Sensex and Nifty 50 fell by 38 per cent.

The challenge of the stock price forecast is the most crucial component for companies and
equity traders to predict future revenues. A successful and accurate prediction to the future
stock prices ultimately results in profit maximization.

- Part-01:
The objective of the first part of the problem statement is to predict the Stock Price of a
Listed Stock on 10th August 2020. The output file 01 should contain only Stock Index and
the respective Stock Price for the test data.

- Part-02:
The Put-Call Ratio of a stock is a time-dependent parameter, for which you have to come up
with a Time-series prediction model. Using the Put-Call Ratio predicted by the model, you
need to calculate the Stock Price on 16th Aug 2020 for every Stock in the test data. . The
output file 02 should contain only Stock Index and the respective Stock Price on 16th August.

# Results
- Part-01:
ANN was used for training the data and predicitng the stock proce due to it having the best MAE and RMSE
  - MAE (Mean Absolute Error)
    - ANN - 0.02122319379167746
    - linear SVR - 0.059130836271092266
    - RBF SVR - 0.06315770319191907
  - RMSE (Root Mean Squared Error)
    - ANN - 0.05687169907013186
    - linear SVR - 0.08538380653520825
    - RBF SVR - 0.09271939343844929
The result was published in an excel file with stock indices and stock prices as its data.

- Part-02:
Here, for time series analysis, we used LSTM (RNN) for the prediction and it was favoured over ARIMA (Auto Regressive Integrated Moving Average) model, due to its performance. I used a Multiple Parallel LSTM, which uses a window based approach for prediction. The time series prediction was done for Put-Call Ratio. AFter the prediction of the ratio, these values were put in the train dataset in the attribute "Put-Call Ratio" and the prediction of the stock prices were done using ANN (which was used in part-1) and the result was published in an excel file with stock indices and stock prices as its data.
