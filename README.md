# Python API Homework - What's the Weather Like?

Created two notebooks in Jupyter by performing API calls to visualize weather information for cities across the globe using two URL. The list of city information was stored as Json and output into csv file, cities.csv, found in the starter_code folder. Using the data from the cities.csv I was able to create data frames related to weather attribute; such as max temp, humidity, cloudiness and wind speed for over 500 cities. Also, I installed citypy from citypy Python Library which let me incorporate ranges for latitude and longitude and find the city name closest to the specified coordinates. Importing citypy was critical for the analysis because it let me observe each city's weather attribute in relationship to their latitude and longitude and create scatter plots for each weather attribute. 

Other dependencies used at startup:

OpenWeatherMap API:

Base URL for API Call: "http://api.openweathermap.org/data/2.5/weather?q="

Google Places API:

Base URL for API Call: "https://maps.googleapis.com/maps/api/place/nearbysearch/json"

!pip install citypy - incorporate latitude and longitude

import pandas as pd - the main data frame used city_weather_df

import numpy as np

import requests - used to collect information from the base URL and API key by city_id;  {base_url + city + "&appid=" + weather_api_key}

import matplotlib - create scatter plots of data collected from API calls; latitude vs temperature, latitude vs humidity, latitude vs cloudiness; latitude vs wind speed

import time

import json - make data visible in Python

import csv - import data from cities.csv and created city_weather_df

import linregress - included regression line for each northern/southern hemisphere scatter plot

# WeatherPy Conclusion:

1. Humidity (%) had the highest correlation to Latitude amongst the other weather attributes. In general, as the latitude increased the Humidity (%) increased.

2. Separating the data into northern and southern hemispheres made it clearer and the scatter plots were easier to understand. The Northern Max Temp vs Latitude regression showed that by increasing the latitude from 0 degrees the temperature decreased. The Southern Max Temp vs Latitude regression showed that by increasing the latitude from -60 degrees the temperature increased. This holds true that as you get farther from 0 degrees latitude (equator) the temperature is lower and the closer you are to 0 degrees latitude the temperature is higher.

3. Comparing the Northern and Southern hemispheres for Cloudiness (%), the slope of the regressions looked very similar. Both regression lines show a positive slope and the statement holds true, as you increase the latitude the cloudiness (%) increases. The Northern Cloudiness vs Latitude plot has an r value of 0.112 and the Southern Cloudiness vs Latitude plot has an r value of 0.115. 

# VacationPy Conclusion:










