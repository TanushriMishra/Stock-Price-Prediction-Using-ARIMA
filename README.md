# Stock-Price-Prediction-Using-ARIMA

An ARIMA is a class of statistical models for analyzing and forecasting time series data. ARIMA is an acronym that stands for AutoRegressive Integrated Moving Average. Briefly they are-
AR: Autoregression. A model that shows dependent relationship between an observation and some number of lagged observation 

I: Integrated. It uses of differencing of raw observations (e.g. subtracting an observation from an observation at the 

previous time step) in order to make the time series stationary.

MA: Moving Average. A model that uses the dependency between an observation and a residual error from a moving average model applied to lagged observations.

Each of these components are explicitly specified in the model as a parameter. A standard notation is used of ARIMA(p,d,q) where the parameters are substituted with integer values to quickly indicate the specific ARIMA model being used.
An ARIMA model consists of coordinates (p, d, q):

•	p stands for the number of autoregressive terms, i.e. the number of observations from past time values used to forecast future values. e.g. if the value of p is 4, then this means that four previous time observations in the series are being used to forecast the future trend.

•	d denotes the number of differences needed to make the time series stationary (i.e. one with a constant mean, variance, and autocorrelation). For instance, if d = 1, then it means that a first-difference of the series must be obtained to transform it into a stationary one.

•	q represents the moving average of the previous forecast errors in our model, or the lagged values of the error term. As an example, if q has a value of 1, then this means that we have one lagged value of the error term in the model.
Implementing ARIMA with statsmodels in Python
For this model we have to do as below

1. Load Libraries
Firstly, we load our libraries . 
import pandas
import matplotlib.mlab as mlab
import matplotlib.pyplot as plt
import numpy as np
import math
from statsmodels.tsa.stattools import acf, pacf
import statsmodels.tsa.stattools as ts
from statsmodels.tsa.arima_model import ARIMA

2. Import csv and define “Close” as closing price variable using pandas

3. Autocorrelation and Partial Autocorrelation Plots

4.ARIMA Model Generation

For Detailed description checkout the "An ARIMA " File above.


Thanks for reading.
