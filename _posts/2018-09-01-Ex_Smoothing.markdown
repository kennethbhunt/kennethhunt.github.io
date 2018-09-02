---
layout: post
title:  "Simple Exponential Smoothing"
date:   2018-09-02 15:33:51 -0600
author: "Kenneth Hunt, MBA"
image: me3.JPG
---

Exponential smoothing is one of the most popular methods of times series forcasting. Here I will perform
 a time series analysis on weekly sales of a cutting tool dataset(Montgomery & Johnson (1976))

 
![ep1]({{ "/assets/img/ep1.png" | absolute_url }})

I decided to begin with a simple exponential smoothing model. There is no evendence of seasonality in the 
data set. Although there is a bit of an increase of the latter part of this graph, there is not very much 
evidence of a trend. 

![ep2]({{ "/assets/img/ep2.png" | absolute_url }})

I have done 2 simple benchmarking methods with the average method, and the seasonal Naive method. 

To evaluate the model accuracy, I used time series cross validation. I compared the root mean squared error, 
with the residual root mean squared error, respectively.

14.87963 <--RMSE

14.65432 <--Residual(RMSE)

The residual root mean squared error is slightly smaller. 

I will model the data here with simple exponential smoothing, and forecast the data.

![ep3]({{ "/assets/img/ep3.png" | absolute_url }})

The black line plots the data and shows changes in the data over time. The red line represents the "fitted"
values along side the data, which is the predicted value of the simple exponential smoothing model. 

Accuracy For Simple Exponential Smoothing 


                

Training set RMSE 3.26 MAPE 2.21 MASE 0.11 





References:
Hyndman, Rob J. and George Athanasopoulos (2018) 
Forecasting: Principles and Practice. https://otexts.org/fpp2/




 





