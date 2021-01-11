# ForecastingResearch  

Repository in which I put resources that have been helpful for me to learn/master forecasting

## Helpful Videos:  

 - [Dr. Franziska Bell's](https://www.youtube.com/watch?v=bn8rVBuIcFg) presentation on forecasting
     - Start by exploring your data, determine the trend and seasonality
     - Two classes of models:
         - Classical/Statistical
             - ARIMA
             - Exponential smoothing
         - Machine Learning
             - Quantile Regression Forest
             - Support Vector Regression
             - Recurrent Neural Networks
     - Deciding on which model depends on the amount of historical data available, the correlation 
     with explanatory variables, interpretability constrains and computational complexity. 
     - You evaluate using backtesting - training up to a timepoint, and then test what happens next. 
     (More details [here](https://eng.uber.com/omphalos/)) There are two methods:
         - Sliding window approach - you take a **fixed** window of raining data that you move 
         forward at every pass, and forecast the amount in front of it.
         - Expanding window approach - particularly useful with less data - you expand the training 
         data from pass to pass, and you test on the ending data.
     - There are several metrics one could use, but comparing your model to a naive forecast (assume 
     today's value will hold until tomorrow) is usually preferred.
     - You need to estimate the uncertainty (prediction intervals) 
     - Special events are frequent and heavily affect core metrics. Often with classical statistical 
     methods, adding exogenous variables is not possible. A more in-depth explanation of this can be 
     found [here](https://eng.uber.com/neural-networks-uncertainty-estimation/)

## Helpful Books:  

 - [Forecasting: Principles and Practice,](https://otexts.com/fpp2/) the classic, authoritative
 resource on forecasting.