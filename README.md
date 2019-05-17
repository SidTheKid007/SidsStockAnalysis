# SidsStockAnalysis
## Purpose
The basic purpose of this project was to experiment with different machine learning models used in the industry, and apply them to the real world example of stock forecasting. More specifically, this project looks at how well different models can predict what price a certain companies stock will close at tomorrow given what that companies stock closed at yesterday.

## Models Used
I set myself some benchmarks by using LinearRegression and a seasonal arima. I then proceeded to work with some more advanced regression models based off decision trees and neural nets. The decision tree based models that I looked at were ExtraTrees, RandomForrest, and XGBoost. The NeuralNet based models that I looked at were the classic Feed-Forward Neural Net and the LSTM Neural Net. I also explored TPOT which is an algorithm that searches for the best algorithm and the best parameters to properly fit the data.

## Results 
Adjusted R squared and Mean Squared Error were The primary metrics that were looked at to determine exactly how good the results were. Adjusted R squared has a range of -infinity to 1, and it is a measure of how closely the model's predictions matched the ground truth. MSE has a range of 0 to infinity, and this looks at how far away the model's predictions are from the ground truth. Better models will have a high adjusted test R^2 value, and a low test MSE.

Insert Charts here

## Conclusion

Linear Regression performed exceptionally well when recent historic data can be used in the prediction of future data. This is because there was a strong autocorrelation between a stock's price today, and a stock's price yesterday. Neural Net Based models tended to perform better than the tree based models because the trends and seasonalities typically weren't fully captured within the training set. Also, the LSTMs tended to outperform the Feed Forward NNs because of their inate nature to capture relevant historic data.

