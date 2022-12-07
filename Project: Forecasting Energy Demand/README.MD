#	Project 'Forecasting Energy Demand'
Under the conditions of electricity and power market, the problem of short-term load  forecasting comes to the fore. Currently a huge number of algorithms for predicting the volumes of electricity consumption have been created. But none of them can be called universal. Any algorithm for the short-term load forecasting is very demanding for the preliminary processing of statistical data.   
The consumption of electricity by the population and industrial enterprises depends on many factors: temperature, time of day (light / dark), weather conditions (in cloudy weather, people are more likely to stay at home), etc.
## Goals and objectives of the project: 
- get as much information as possible from the available data and build the most accurate forecast possible
- analysis of the influence of meteorological factors on electricity demand
- developing an hourly electricity demand forecasting model for the Toronto IESO electrical zone
- Cleaning data and exploring using visualization tools
- Evaluating the influence of meteorological factors on electricity demand
- Building regression models using machine learning methods.

## Overview: 
The study was carried out using programming language Python in Google Collab, as well as its libraries: Numpy and Pandas are for data processing and manipulation; Matplotlib,plotly and seaborn are for data visualization, Scikitlearn, and CatBoost are for loading machine learning models and metrics. Google Collab (Jupyter notebook) was chosen as the working environment because these tools allow me to effectively develop and present its results in an interactive form. All initial data sets are a sufficiently large sample and correspond to some characteristics of the Big Data. 
Using Pandas_profiling  I have received a brief overview of my data.
## Data Description:
- date_time – The date and time measurement stamp
- reading – The measurement of average hourly electricity demand taken in the Toronto IESO electrical zone
- date_time – The date and time measurement stamp
- drybulb – a measure of dry-bulb temperature in degrees Celsius 
- dewpoint – a measure of dew point temperature in degrees Celsius 
- windspeed – a measure of wind speed in km/h
- winddirection – a measure in degrees ranging from 0 to 360
- illumination – measured in klux
- humidex and windchill – measures of apparent temperature in degrees Celsius 
## Conclusions:
Accurate predictive data were obtained in machine learning models by identifying factors such as temperature, humidex, hour of a day. I have buit various regression models of machine learning. The best ones for this task are RandomForest and Catboost.
the goal and objectives of the project were achieved: electricity consumption was predicted based on the data. Electricity consumption has a clear seasonal pattern. There is a trend increase in consumption associated with an increase in the average daily temperature. The most accurate prediction results were obtained using a machine learning model based on the CatBoostRegressor algorithm. It is important to note that in order to increase the reliability of the forecast, it is necessary to get more data, to try feature engineering to artificially expand the data, and also to look closer at the humidex.
