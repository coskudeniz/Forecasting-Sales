# Forecasting-Sales
Using time-series and deep learning models to forecast sales.

## DATA
A timeseries dataset is given in the dataset folder, which consists of monthly sales. The sales information spans the duration of 8 years and 9 months. The dataset is composed of two fileds. The first field "Month" shows the dates in yyyy-mm format and the second field "Sales" shows the number of products sold in the corresponding year and month.  

The time period spans the months from 1984-01 to 1992-09. The minimum amount of sales achieved is 1413 in 1992-08 and the maximum amount of sales achieved is 13916 in 1989-12. 

## AIM 
The aim of the project is to train models using the sales information from the first 8 years and then using the trained models to predict the amount of sales for the last 9 months. Different models are compared with each other based on the RMSE (Root Mean Square Error) calculated on the last 9 months. Generalization error is not reported for this project. 

The models used for predition are:
* Ridge Regression
* Random Forests
* Exponential Smoothing
* SARIMA (Seasonal Autoregressive Integrated Moving Average)
* LSTM (Long Short-Term Memory) Networks

## RESULTS
The mean of number of sales during the first 8 years rounded to the nearest integer is 4803. If this value will be predicted for each month for the following 9 months, the RMSE will be 1290.45 and the R2 score also known as the coefficient of determination will be -0.17. The R2 score measures the proportion of the variation in the dependent variable explained by the regression model. The RMSE and R2 Score results calculated using the last 9 months are shown in the table below. Hyperparameter tuning and model selection is performed trying to optimize RMSE, not the coefficient of determination.   

Model | RMSE | R2 Score
--- | --- | ---
Ridge Regression | 766.69 | 0.59 
Random Forest | 349.61 | 0.90
Exponential Smoothing | __275.58__ | 0.89
SARIMA | 310.46 | __0.93__
LSTM | 689.28 | 0.67 
