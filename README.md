# Bangkit Capstone Project Summary
Our project was called "Agrarian". Agrarian is a web based application that provide information of today's weather parameters like temperature, precipitation, humidity, and able to predict the precipitation and temperature of several days ahead as an insight for farmers to determine best planting time for their plants seed.


## Research Steps
1. Machine Learning\
The machine learning main job role were model building, fine tuning model, and model deployment. the first step of our ML model building was searching for the suitable dataset. the dataset that we were using was Semarang Daily Weather Summary which recorded by Ahmad Yani International weather station, and provided by National Center for Environmental Information (NCEI) (https://www.ncei.noaa.gov/). The data contains precipitation(mm), maximum temperature(F), minimum temperature(F), and average temperature(F) of Semarang City since 19th August 1957 to 3rd June 2021.\
After we got the dataset, the next step that we did was data anlysis to cleanup the data, look at the statistics and the distribution of data. It was done to erase or fix some error datapoint. for this project, we make a model that can perform curve fitting of time series dataset, and forecast the next value. To measure the best result we use loss and MAE as our measurement. this way, we know how much our model fit the dataset how good its result when it is used for forecasting. For this model, we used several layers like convolutional, LSTM, and dense layers. For the fine tuning process, we did several searching in google and looking at several video material in time series forecasting course, then tweak several parameters like batch size, window size, learning rate, also change the slice of our dataset. In the end, for the final result, we were able to get satisfying result where we get 0.25 for our precipitation curve MAE, 1.50 for our maximum temperature curve MAE, and 1.24 for our minimum temperature curve MAE.\
The next step is to deploy our model. Because we used web application as our platform, then we need to use tensorflow.js as our deployment method.


