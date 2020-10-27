# What's the Weather Like? - Python API Homework <!-- omit in toc -->

For Findings, please click on the findings section of the table of contents

- [Background](#background)
  - [WeatherPy - An analysis of weather data as it related to latitude](#weatherpy---an-analysis-of-weather-data-as-it-related-to-latitude)
  - [VacationPy - Planning future vacations based off of the weather data.](#vacationpy---planning-future-vacations-based-off-of-the-weather-data)
- [Findings](#findings)
    - [Takeaways from Results of WeatherPy](#takeaways-from-results-of-weatherpy)
- [VacationPy Results](#vacationpy-results)
- [Here are the 9 Cities and the closet hotels:](#here-are-the-9-cities-and-the-closet-hotels)

## Background

### WeatherPy - An analysis of weather data as it related to latitude

In this assignment, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I used a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

1. The first objective was to build a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

2. The next objective was to run linear regression on each relationship. This time, I seperated each city into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

### VacationPy - Planning future vacations based off of the weather data.

In the next part of the assignment, I took the weather data from above and used jupyter-gmaps and the Google Places API to identify
cities with "perfect weather".

1.  I created a heat map that displayed the humidity for every city from part I of the assignment.

2.  I narrowed down the DataFrame to find my ideal weather conditions. These conditions were:

    - A maximum temperature lower than 80 degrees but higher than 70 degrees.
    - A wind speed less than 10 mph
    - Zero Cloudiness

3.  After dropping cities that didn't meet all three conditions, I used the Google Places API to find the first hotel within 5000 meters of the city coordinates. 
4.  Next, I plotted each hotel on top of the humidity heatmap and included a pin containing the following:

    - Hotel Name
    - City
    - Country

## Findings


#### Takeaways from Results of WeatherPy

Here are my three takeaways related to the analyzing of the meteorological data:

-As we move closer to the equator, the temperature increases.
-Cloudiness seems to be randonly dispersed across all latitidues.
-As we move closer to the equator, the humidity increases. 


