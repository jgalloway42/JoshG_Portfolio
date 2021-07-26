# Josh Galloway Portfolio
Selected projects from my work in data science, statistics, and numerical analysis.

## RNN Application: Predicting VIX Ticker Volatility from Headlines

Working from publicly available data sources, the student trained a recursive neural network (RNN) implemented in Python (pandas, sklearn, keras) to predict the Chicago Board Options Exchange (CBOE) Volatility Index (VIX). An ad hoc method of sentiment quantification was applied to datasets containing Reddit and ABC headlines spanning several years. The result was a trained RNN that was able to predict the Delta VIX closing day over day based on the headlines from the previous 20 trading days.
<br>
Once  trained,  the  network  was  scored  against  a  test  set  to  root-mean-squared  error (RSME),  and  evaluated  again  by  graphing  the  results  of  the  prediction  against  the recorded  data  set.   The  RMSE  was  1.87  for  the  ABC  dataset  against  the  segregated test set, and 2.07 for the Reddit.  The predictions graphed against the ABC datase is shown below, and the full writeup pdf is available [here](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/Math_7243_Machine_Learning_Final_Project_r3.pdf).

![](/images/VIX%20Prediction%20ABC%20Headlines%20Results.png)
