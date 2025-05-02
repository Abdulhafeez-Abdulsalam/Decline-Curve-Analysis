# Decline-Curve-Analysis

This is the code repository of Arps decline curve analysis which was used for forecasting production rate

DATA DESCRIPTION

​The analysis utilized publicly accessible production data provided by the Oil and Gas Division of the North Dakota Industrial Commission (NDIC). Specifically, the study employed time-series data comprising monthly production figures from mid-2015 through 2018 for history matching purposes, while data from 2019 were used for forecasting. This dataset, offering detailed monthly insights into oil, gas, and water production per well, is instrumental in evaluating production trends and reservoir performance over time. 

To model and forecast production decline, the conventional Arps decline curve models—exponential, hyperbolic, and harmonic—were applied, providing a framework to characterize different decline behaviors observed in the dataset. Although the dataset encompasses approximately 17,756 wells, the analysis focused on two wells to facilitate a detailed evaluation. Given the time-series nature of the data, the Root Mean Square Error (RMSE) metric was employed to assess model accuracy. RMSE quantifies the average magnitude of prediction errors by measuring the square root of the mean squared differences between predicted and actual values, making it particularly useful for evaluating time series forecasting models.

Arps DECLINE CURVE ANALYSIS

Arps decline curve analysis is a foundational method in reservoir engineering for forecasting production rates and estimating reserves of oil and gas wells. Introduced by J.J. Arps in 1945, this empirical approach models the decline in production over time using mathematical equations, aiding in economic evaluations and strategic planning.

EXPONENTIAL DECLINE MODEL

The exponential decline model assumes a constant percentage decrease in production rate over time. It's characterized by a straight-line trend on a semi-log plot, making it suitable for wells in stable reservoirs without significant pressure changes. The model is defined by:​

q(t) = qᵢ * e^(–D * t)​

Where:

q(t) is the production rate at time t

qᵢ is the initial production rate

D is the constant decline rate

HYPERBOLIC DECLINE MODEL

The hyperbolic decline model accounts for a decreasing decline rate over time, offering flexibility for wells experiencing variable reservoir conditions. It's represented by:​

q(t) = qᵢ / (1 + b * D * t)^(1/b)​

Where:

b is the decline exponent (0 < b < 1)​

This model is particularly useful for unconventional reservoirs where production decline doesn't follow a constant rate.​


HARMONIC DECLINE MODEL

The harmonic decline model is a special case of the hyperbolic model with a decline exponent b equal to 1. It describes a scenario where the decline rate decreases more gradually over time:​

q(t) = qᵢ / (1 + D * t)​

This model is applicable to wells with long-term production data showing a slow and steady decline.
