# London-Bike_Rides

# Bike Share Exploratory Analysis 
This repository contains an analysis and predictive model for bike shares based on weather, seasonal, and temporal data from London's bike-sharing system. The dataset spans from 01/01/2015 to 31/12/2016 and is derived from multiple sources.

## Purpose
The primary objective of this project is to analyze historical bike-share data and build predictive models to forecast future bike shares based on:
- Weather conditions
- Holidays
- Weekends
- Seasons
---
## Dataset Overview

The dataset combines data from:

1. [Transport for London Open Data](https://cycling.data.tfl.gov.uk/)  
   - **License**: Contains OS data © Crown copyright and database rights 2016 and Geomni UK Map data © database rights [2019]. Powered by TfL Open Data.
2. [Freemeteo.com](https://freemeteo.com/) (Weather Data)
3. [UK Government Bank Holidays](https://www.gov.uk/bank-holidays)

## Metadata

| **Column Name**    | **Description**                                                                                             |
|--------------------|-------------------------------------------------------------------------------------------------------------|
| `timestamp`        | Timestamp field for grouping the data                                                                      |
| `cnt`              | Count of new bike shares                                                                                   |
| `t1`               | Real temperature (°C)                                                                                       |
| `t2`               | "Feels like" temperature (°C)                                                                            |
| `hum`              | Humidity (%)                                                                                              |
| `wind_speed`       | Wind speed (km/h)                                                                                         |
| `weather_code`     | Category of the weather (see below for description)                                                       |
| `is_holiday`       | Boolean field (1 = holiday, 0 = non-holiday)                                                              |
| `is_weekend`       | Boolean field (1 = weekend, 0 = weekday)                                                                  |
| `season`           | Meteorological seasons (0 = Spring, 1 = Summer, 2 = Fall, 3 = Winter)                                     |

### Weather Code Categories

| Code | Description                                                                          |
|------|--------------------------------------------------------------------------------------|
| 1    | Clear / Mostly clear                              |
| 2    | Scattered clouds / Few clouds                                                       |
| 3    | Broken clouds                                                                       |
| 4    | Cloudy                                                                              |
| 7    | Rain / Light rain                                               |
| 10   | Rain with thunderstorm                                                              |
| 26   | Snowfall                                                                            |
| 94   | Freezing fog                                                                        |

---

### Target Variable:
- `bike_rides` (Count of new bike shares)

### ANALYSIS PROCESS

1. First the date downloaded from Kaggel.com and accessed using python for data wrangling and cleaning.
2. Data missing value and duplicates handling.
3. Data used for predictive modeling to find future expectations of bike shares
4. Data accessed using Tableau and created responsive dashboard for insights.


## INSIGHTS AND RECOMMENDATIONS 
1. Based on data it is observed that bike shares are not dependent on weekend or holidays means people actually<b>
using these services for their needs more than entertainment purposes. 
2. Bike shares are not favorable in too cloudy, rainy or days with snowfall.
3. Seasonality not much affect the bike shares bu it still understandably higher in warmer seasons than previous.
4. When looking at the bike shares hourly consumption, it is visible that throughout the day people use this services to reach work, school or after work to reach home or other destinations

### Recommendations
1. To increase bike shares for entertainment purposes marketing campagins, gamification or discounts can be applied so service providers can make more income during any time of the day<br>
as scooters bring happines, improve mood and allows you to enjoy the nature and eco-friendly life harmony. This way it may increase acquisition and conversion during weekends<br/>
or holidays.
2. As the weather temperature, cloudy days are usual weather conditions in UK it does not much affect the consumption and in this situations company has not much to do agains natural weather conditions to use these services unless we want to innovate the product<br/>
and create new products for those needs.
