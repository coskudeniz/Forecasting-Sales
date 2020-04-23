# Forecasting-Sales
Using time-series and deep learning models to forecast sales.

## DATA
A timeseries dataset is given in the dataset folder, which consists of monthly sales. The sales information spans the duration of 8 years and 9 months. The dataset is composed of two fileds. The first field "Month" shows the dates in yyyy-mm format and the second field "Sales" shows the number of products sold in the corresponding year and month.  

## AIM 
The aim of the project is to train models using the sales information from the first 8 years and then using the trained models to predict the amount of sales for the last 9 months. Different models are compared with each other based on the RMSE (Root Mean Square Error) calculated on the last 9 months. Generalization error is not reported for this project. 

The models used for predition are:
* Ridge Regression
* Random Forests
* Exponential Smoothing
* SARIMA (Seasonal Autoregressive Integrated Moving Average)
* LSTM (Long Short-Term Memory) Networks

## RESULTS
/***
Model | RMSE
--- | --- 
Ridge Regression | 766.69 
Random Forest | 349.61
Exponential Smoothing | __275.58__
SARIMA | 310.46
LSTM | 627.10
***/
