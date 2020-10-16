# Python API Homework - What's the Weather Like?

Created two notebooks in Jupyter by performing API calls to visualize weather information for cities across the globe using two URL. The list of city information was stored as Json and output into csv file, cities.csv, found in the starter folder. Using the data from the cities.csv I was able to create data frames related to weather attribute; such as max temp, humidity, cloudiness and wind speed for over 500 cities. Also, I installed citypy from citypy Python Library which let me incorporate ranges for latitude and longitude and find the city name closest to the specified coordinates. Importing citypy was critical for the analysis because it let me observe each city's weather attribute in relationship to their latitude and longitude and create scatter plots for each weather attribute. 

Other dependencies used at startup:

OpenWeatherMap API

Base URL for API Call: "http://api.openweathermap.org/data/2.5/weather?q="

Google Places API

Base URL for API Call: "https://maps.googleapis.com/maps/api/place/nearbysearch/json"

!pip install citypy - incorporate latitude and longitude

import pandas as pd - the main data frame used city_weather_df

import numpy as np

import requests - used to collect information from the base URL and API key by city_id;  {base_url + city + "&appid=" + weather_api_key}

import matplotlib - create scatter plots of data collected from API calls; latitude vs temperature, latitude vs humidity, latitude vs cloudiness; latitude vs wind speed

import time

import json - make data visible in Python

import csv - import data from cities.csv and created data frame


Utilized Panda functions recently learned in class:


# WeatherPy Conclusion:

1. Of the total 576 Heroes of Pymoli players, 84.03% were male players and 14.06% were female players. This is a large reason there is a higher Total Purchase Value from Male players over Female players.

2. The item name 'Final Critic' was the most popular item and the most profitable item in Heroes of Pymoli. It has a purchase count of 13 and has the highest Average Purchase Price among the other items.

3. According to Age Demographics, age group from 20 to 24 had the highest count and percentage of players at 44.79%. The second highest age group was 15 to 19 with percentage of players at 18.57%. The positive relationship between number of players and Total Purchase Value is also evident in Purchasing Analysis (Age) data frame. Players in the 20 to 24 age group had the highest Total Purchase Value among the other groups but the highest Average Purchase Price was for age group 35 to 39.












