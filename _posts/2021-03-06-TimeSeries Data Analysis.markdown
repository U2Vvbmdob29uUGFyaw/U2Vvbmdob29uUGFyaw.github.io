---
layout: post
title:  시계열 데이터 분석
date:   2021-03-06
use_math: true
description: 시계열 데이터에서의 비정상 탐지
---

<blockquote> 시계열 데이터 분석 </blockquote>
### 1. Naive Approach
### 2. Simple Average
### 3. [Moving Average](https://en.wikipedia.org/wiki/Moving_average)
In statistics, a moving average (rolling average or running average) is a calculation to analyze data points by creating a series of averages of different subsets of the full data set. It is also called a moving mean (MM) or rolling mean and is a type of finite impulse response filter. Variations include: simple, and cumulative, or weighted forms (described below).

Given a series of numbers and a fixed subset size, the first element of the moving average is obtained by taking the average of the initial fixed subset of the number series. Then the subset is modified by "shifting forward"; that is, excluding the first number of the series and including the next value in the subset.

A moving average is commonly used with time series data to smooth out short-term fluctuations and highlight longer-term trends or cycles. The threshold between short-term and long-term depends on the application, and the parameters of the moving average will be set accordingly. For example, it is often used in technical analysis of financial data, like stock prices, returns or trading volumes. It is also used in economics to examine gross domestic product, employment or other macroeconomic time series. Mathematically, a moving average is a type of convolution and so it can be viewed as an example of a low-pass filter used in signal processing. When used with non-time series data, a moving average filters higher frequency components without any specific connection to time, although typically some kind of ordering is implied. Viewed simplistically it can be regarded as smoothing the data.
### 4. [Exponential Smoothing](https://en.wikipedia.org/wiki/Exponential_smoothing)
Exponential smoothing is a rule of thumb technique for smoothing time series data using the exponential window function. Whereas in the simple moving average the past observations are weighted equally, exponential functions are used to assign exponentially decreasing weights over time. It is an easily learned and easily applied procedure for making some determination based on prior assumptions by the user, such as seasonality. Exponential smoothing is often used for analysis of time-series data.

Exponential smoothing is one of many window functions commonly applied to smooth data in signal processing, acting as low-pass filters to remove high-frequency noise. This method is preceded by Poisson's use of recursive exponential window functions in convolutions from the 19th century, as well as Kolmogorov and Zurbenko's use of recursive moving averages from their studies of turbulence in the 1940s.

The raw data sequence is often represented by ${x_{t}}$ beginning at time $t=0$, and the output of the exponential smoothing algorithm is commonly written as ${s_{t}}$, which may be regarded as a best estimate of what the next value of $x$ will be. When the sequence of observations begins at time $t=0$, the simplest form of exponential smoothing is given by the formulas

$s_{0} = x_{0}$  
$s_{t} = \alpha x_{t} + (1-\alpha)s_{t-1}, t>0$  
where $\alpha$ is the smoothing factor, and $0 < \alpha > 1$
### 5. Holt Winter's Seasonal
### 6. ARIMA
### 7. Deep Learning
