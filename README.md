# Machine_learning_trading_bot
Module 14 Challenge
### Executive Summary
  This report examines potential models for approaching algorithmic trading of emerging markets' OHLCV data. In the first section of the analysis, the provided notebook is opened in google colab, the kernel is restarted, and the cells corresponding to three steps are run: importing the OHLCV dataset into a Pandas DataFrame, generating trading signals using short- and long-window SMA values, and splitting the data into training and testing datasets. 
  The SVC model from the SKLearn support vector machine (SVM) learning method is then utilized to fit the training data and make predictions based on the testing data, which are reviewed. The subsequent step entails reviewing the classification report associated with the SVC model's predictions. A predictions DataFrame is then prepared, containing columns for "Predicted," "Actual Returns," and "Strategy Returns" for the DataFrame. The next step is creating a cumulative return plot depicting actual returns versus strategy returns, which serves as a baseline for comparing the effects of tuning the trading algorithm. After plotting the charts, they are exported as PNG files and saved in the Images directory.
  
## PLOTS:

Plot 1- Generate trading signals using short- and long-window SMA values

![Plot_Trading Signals using Short and long window](https://user-images.githubusercontent.com/118064873/228393403-177e95f1-f5ad-48a4-8c54-f43f9bbc0f0c.png)

PLOT 2- a cumulative return plot that shows the actual returns vs. the strategy returns
The below Plot reflects the stratgeic returns are higher than the actual returns.

![Plot_Actual vs Startegy_Returns_Original](https://user-images.githubusercontent.com/118064873/228396475-bf5a84c4-02a7-44e1-8ebe-100e552744be.png)

PLOT 3- Tune the training algorithm by adjusting the size of the training dataset.
The below Plot reflects whe the training data is increased to 6 months can improve the performance of algo. 
![Actual_vs_Startegy_6months_training](https://user-images.githubusercontent.com/118064873/228398150-d5acdadc-bfcf-4d6c-a126-25a77b19a8b5.png)

PLOT 4- Tune the trading algorithm by adjusting the SMA input features.
In the below plot, SMA short wndows has been assigned to 40 and long windows assigned to 100.
![Actual_Vs _Startegy_40_200](https://user-images.githubusercontent.com/118064873/228397935-4492e9eb-75a9-4dbb-b5a8-e7e9b7aaca81.png)

Plot 5-Backtest the new model to evaluate its performance

![Plot_Actual Returns vs Strategy_returns](https://user-images.githubusercontent.com/118064873/228392388-0096b33b-9386-4022-8625-903bccc53623.png)


