# Machine_learning_trading_bot
Module 14 Challenge
### Executive Summary
  This report examines potential models for approaching algorithmic trading of emerging markets' OHLCV data. In the first section of the analysis, the provided notebook is opened in google colab, the kernel is restarted, and the cells corresponding to three steps are run: importing the OHLCV dataset into a Pandas DataFrame, generating trading signals using short- and long-window SMA values, and splitting the data into training and testing datasets. 
  The SVC model from the SKLearn support vector machine (SVM) learning method is then utilized to fit the training data and make predictions based on the testing data, which are reviewed. The subsequent step entails reviewing the classification report associated with the SVC model's predictions. A predictions DataFrame is then prepared, containing columns for "Predicted," "Actual Returns," and "Strategy Returns" for the DataFrame. The next step is creating a cumulative return plot depicting actual returns versus strategy returns, which serves as a baseline for comparing the effects of tuning the trading algorithm. After plotting the charts, they are exported as PNG files and saved in the Images directory.
  
## PLOTS:

Plot 1- Generate trading signals using short- and long-window SMA values

![Plot_Trading Signals using Short and long window](https://user-images.githubusercontent.com/118064873/228393403-177e95f1-f5ad-48a4-8c54-f43f9bbc0f0c.png)

PLOT 2- a cumulative return plot that shows the actual returns vs. the strategy returns

![Plot_Actual vs Startegy_Returns_Original](https://user-images.githubusercontent.com/118064873/228396475-bf5a84c4-02a7-44e1-8ebe-100e552744be.png)

PLOT 3- Tune the training algorithm by adjusting the size of the training dataset.

![Plot_Actual Vs Startegy Returns_6months_Training](https://user-images.githubusercontent.com/118064873/228396731-9df39c7c-90f1-467c-b928-c7364a29cb1f.png)

PLOT 4- Tune the trading algorithm by adjusting the SMA input features.

![Plot_Actual vs Strategy returns_SMA_40_200](https://user-images.githubusercontent.com/118064873/228396872-a12bbbdc-8c11-4b82-b0d8-e7f07afcb716.png)

# CONCLUSION: 
Plot 3-Generate trading signals using short- and long-window SMA values

![Plot_Actual Returns vs Strategy_returns](https://user-images.githubusercontent.com/118064873/228392388-0096b33b-9386-4022-8625-903bccc53623.png)

1. Did this new model perform better or worse than the provided baseline model? Answer: No. The reason for this is, according to the diagram 5, after changing the classification model, the new model worked well until mid of 2020. However, after that the return of the new algo with Decisiontree didn't work well.
2. Did this new model perform better or worse than your tuned trading algorithm? Answer: No, it worked better than the tuned trading algorithm until the mid of 2020. Nevertheless, it starts to decline after that. So, the tuned algorithm is better than the new algo based on Decisiontree.
