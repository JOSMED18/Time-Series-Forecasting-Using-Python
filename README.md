# Forecast-with-time-series-using-Python 📉📈
Creating a forecast for a dataset from 2010 to 2012 of Walmart. In this repository two models are used. Holt Winters model (which uses trend, level and seasonality) and regression analysis (which depends on different independent variables). In this case we are not discussing whether one is better than another. Instead, it is an opportunity to evaluate cases from different statistical points of view. We will see that Holt Winters model, since it is an exponential smoothing analysis, will never catch up with the real sale, but is a really good approach since it takes into account new data. In the other hand, regression takes into account the change in an independent variable. So let's see.

Here is the tableau dashboard with the whole story. Just to summarize. ✨
https://public.tableau.com/app/profile/josu.medina/viz/TimeSeriesAnalysis_16750539246830/Forecast_Story

### Machine Learning
Every machine learning model is divided in two phases: training and testing. It means we are using part of the data (most of it) to train a model and help him recognize patterns. Then, we use testing data to determine if it is precise. So, in this case, we divided it by a date that would allow our training data set to have 2 cycles. In time series analysis we need at least 2 cycles to forecast our data. So, as you will see, the error (Root Mean Square Error) will be big.

![image](https://user-images.githubusercontent.com/101015892/215389075-9c3f6007-86d6-49b4-8b49-63e7e2dc1f0e.png)
_Graph of training and testing data_

## Regression model
Regression uses independent variables to predict dependent variables, in this case we will use two: week and a flag that show us wheter there is a holiday or not during the week. It also identifies patterns in dates, it's a mix with Linear regression and time series analysis.

## Holt Winter
This is time series, totally. It uses the data and assigns a higher value for new data, and a lower one for old data. It is useful when data is stationary and have a well defined pattern. 
