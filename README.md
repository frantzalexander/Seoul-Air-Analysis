# Seoul Air Pollution Analysis

## Project Overview
The case study is a time series analysis of the air pollution in Gangnam, Seoul, South Korea. 

## Objectives
- Data Exploration

- Trend Analysis

- Identify Seasonal Patterns
  
- Anomaly Detection

- Create Benchmark Analysis

- Short-term Forecasting

- Identify Correlations

- Visualize the Underlying Data Structure 


## Results
![image](https://github.com/frantzalexander/Seoul-Air-Analysis/assets/128331579/89a15c32-e230-49d2-87ce-baea95619971)

As shown in the time series visualization, there were significant changes in air quality levels throughout the time period of the analysis.

This suggests a govenment policy change. 

The Training set for the ARIMA Model was the data from the Month of October 2019.

The Target prediction was November 1st, 2019.

The Baseline Mean Absolute Error of the model was 8.08.

The Mean Absolute Error from the Test Data with walk-forward validation was 8.76.

## Process
```mermaid
flowchart TD
start(((START)))
import[Import Dataset]
resample[Resample & Forward Fill Missing Values]
explore[Explore Dataset]
rolling[Create Weekly Rolling Average Visualization]
acf[Create ACF Visualization]
pacf[Create PACF Visualization]
split[Split Dataset: Training & Test]
model[Model Building]
baseline[Create Baseline Model]
iterate[Iterate]
hyper[Hyperparameter Tuning]
eval[Evaluate]
walk[Walk-Forward Validation]
communicate[Communicate Results]
finish(((END)))
start --> import
import --> resample
resample --> explore
explore --> rolling
rolling --> acf
acf --> pacf
pacf --> split
split --> model
model --> baseline
baseline --> iterate
iterate --> hyper
hyper --> eval
eval --> walk
walk --> communicate
communicate --> finish



