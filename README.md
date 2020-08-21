# store-item-demand-forecasting-kaggle
we have given 5 years of store-item sales data, and asked to predict 3 months of sales for 50 different items at 10 different stores.  What's the best way to deal with seasonality? Should stores be modeled separately, or can you pool them together? Does deep learning work better than ARIMA? Can either beat xgboost?  This is a great competition to explore different models and improve your skills in forecasting.
Before we begin:
I would like to take the opportunity to appreciate the help of Corey Levinson,Kirill Tsyganov, Alexey Kozionov, Alexander Andreev, Jaroslav Bologov, Nurlan Shagadatov & Makarychev Sergey**.

If you liked my work, then please don't forget to upvote the Tutorial since it will keep me motivating to perform more in-depth reserach Forecasting Method.I hope you will enjoy our deep exploration into this dataset. Suggestions on improvements are welcome.

Let the Forecasting begin. :)

# Executive Summary:
This tutorial consists of comprehensive Exploratory Data Analysis with Prophet and MLP Neural Network Forecast Modeling for Store Item Demand Forecasting Challenge competition. The objective of the problem is to forecast 3 months of sales for 50 different items at 10 different stores using the 5 years history of sales.

The data contains the following files:

train.csv : the training data witht the history of sales.

test.csv: the test data to predict the sales.

Sample submission.csv: Sample submission file

# Data fields

date - Date of the sale data. There are no holiday effects or store closures.

store - Store ID

item - Item ID

sales - Number of items sold at a particular store on a particular date.

# Introduction:
Time series forecasting is a skill that few people claim to know. Machine learning is cool. And there are a lot of people interested in becoming a machine learning expert. But forecasting is something that is a little domain specific.

Retailers like Walmart, Target use forecasting systems and tools to replenish their products in the stores. An excellent forecast system helps in winning the other pipelines of the supply chain. If you are good at predicting the sale of items in the store, you can plan your inventory count well. You can plan your assortment well.

A good forecast leads to a series of wins in the other pipelines in the supply chain.

What is time series?
A time series is a sequence of observations collected at some time intervals. Time plays an important role here. The observations collected are dependent on the time at which it is collected.

The sale of an item say bread in a retail store like Walmart will be a time series. The sale could be at daily level or hourly level. The number of people flying from NewYork to Spain on daily basis is a time series. Time is important here. During Christmas holidays, this number would be humongous compared to the other days. This is know as seasonality.

What is the difference between a time series and a normal series?
Time component is important here. The time series is dependent on the time. However a normal series say 1, 2, 3...100 has no time component to it. When the value that a series will take depends on the time it was recorded, it is a time series.
