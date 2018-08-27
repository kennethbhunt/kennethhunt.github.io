---
layout: post
title:  "Data Science for Decision Making"
date:   2018-08-28 15:33:51 -0600
author: "Kenneth Hunt, MBA"
image: me3.JPG
---


Many types of companies today are generating large amounts of data. The data is very useful by business decision makers to draw 
inferences from and to help them make choices that will allow their companies to be as efficient and profitable and 
possible.

Time series data can be defined as a series of data points indexed in time order. Time series analysis comprises methods 
for analyzing in order to exact meaningful statistics and other characteristics of the data.

There are a number of ways that time series anaysis can be useful for businesses. For example, it may be necessary to 
forecast quantities of product items, and having a better understanding of historical time series patterns.
Forecasting time series data is key for any business to remain competitive and to operate at the most efficient manner
 possible. I’m going the explore 3 simple forcasting methods that may be used in forecasting time series data, and it may
 also be used as benchmarking more complex time series forcasting methods.

This is a look at the "Bike Sharing Dataset" from the UCI Machine Learning Repository. This dataset contains the daily 
count of rented bikes during 2011-2012. 

![cap]({{ "/assets/img/cap.jpg" | absolute_url }})

It is important to first visualize the data and examine it’s patterns and any irregularities in the data set.

![p1]({{ "/assets/img/p1.png" | absolute_url }})

The chart above shows seasonality, as the rise and fall of bike rentals occur in January, and July. There is no obvious trend,
 or cyclic pattern in this chart.

Next, I will clean any possible missing values and any outliers which may have a significant effect on the data.

![p2]({{ "/assets/img/p2.png" | absolute_url }})

I will now use 2 simple forecasting methods which are the average method, the naive method, and the seasonal naive method. 
The average method calculated the forecast as the average of the historical data. The naive method calucates the forecast 
based on the value of the last observation of the data.

![p3]({{ "/assets/img/p3.png" | absolute_url }})

In the chart above, we can see both the average method, and the naive, or the random walk method. These simple methods can 
perform quite well for forcasts, or they can be used as benchmarks for more complex time series forecasts. It is important
 that if more complex time series forcasting methods are used, they must have higher performance than simple methods or they 
should not be used in a forecast.




