# Stock-prediction
Apple and google stock prediction using recurrent networks

Every stock data has 4 important data:

Open: the price at the beginning of the sale that day
Close: the last price that it was closed for sale that day
Low: the lowest price it has reached that day
High:the highest price it has reached that day


Here I used the 'Close' price to predict the price for the other days. Another more accurate way is to use the average of the Low and High price.

This is what happened in this code:

1. making a time-series of data. Every day data is made by the last 3 days data.

2. split it in Train, Validation and Test sets by Fold-sampling

3. The model details
   tested with three recurrent cells : RNN , LSTM, GRU
   tested with 3 optimizers: Adam, RMSprob, AdaDelta
   tested with learning-rate of 0.001
   250 epochs
   
the models reached 99% accuracy
