# crash_dummies
Project 5 for DSI-824

Team - Crash Dummies - Reggie DePiero, Apratim Biswas, and Christopher Villafuerte

## Goal:
In 2018 alone, there were 228,047 car accidents in New York City [[1]]("https://www.autoinsurancecenter.com/traffic-accidents-in-new-york-city.html"). The goal of the project is to identify high risk factors within NYC traffic. The final deliverable is a report that:
1. Studies the contributing factors and pre-condition.
2. Examines vehicular collisions data as a time series and build a model to predict number of crashes, and 
3. Create a map of risks, both: spatial and temporal. 

The motivating factors for creating such a map are:
1. first responders can use it to navigate the city during motor Vehicle crashes, natural disaster, and emergencies; and,
2. it be used by city planers to improve traffic performance and make the roads safer.

In our time-series model, we focused on Lincoln tunnel and its surrounding areas. This is because the tunnel serves as one of the major arteries that feeds traffic from New jersey. 

## Data
We accuirred data from NYC cityofnewyork.us
* Motor-Vehicle-Collisions-Crashes & ____
* 1.7 million entries since 2017
* Speed sensor data ~ 17 gb data from speed sensors

## Process
We inspected the crash data and saw that it listed all the crashes for each day for the last 3 years.
We examined the crash data and saw that ['CONTRIBUTING FACTOR VEHICLE 1'] & ['Pre-Conditions'] where interesting data to examine.
We applied pythons datetime method to examine the crash information as a time series data and organized it by crashed per day.
We examined the number or crashes that happened per day, per hours, number of crashes per Contributing factor and pre-condition.
We plotted the contributing factors via their gps location on a scatter to see if there was a particular accumulation of crashes in a particular area.


We saw that the number of crashes in nyc as a whole was overwhelming therefore we created an geoSpatial polygon to focus our attention to a give area.
We created a polygon to encapsulate the Lincoln tunnel and its surrounding area. We choose this area because the Lincoln tunnel is one of the major arteries that feeds car traffic from New jersey. This polygon was also chosen because it sits within the inner grid system of Manhattan island.
32 Million cares pass through the Lincoln Tunnel a year.
We created interactive clustering Maps using folium. These maps allowed us to visually see in what intersection and what streets there was a high accumulation of crashes.
Within this map we also color coded the top 3 causes of crashes within out polygon of NYC
## Model

We attempted to predict the number or crashes that would take place within our preset polygon for the month of September.
We used Sarima model and Ses model. 


## Conclusions
* There is a diurnal pattern to when crashes occur. Most occur in late afternoon.
* Most crashes involve cars going straight forward and are caused by inattentive drivers.
* Time-series models were able to predict the average number of crashes going forward, but was not able capture the complexity of the data.
###  Future Work
* Include additional factors in the model with better chance of capturing complexity.
* Create a spatio-temporal showing risk of vehicular crashes in New York City