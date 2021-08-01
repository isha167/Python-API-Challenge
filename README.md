# Python-API-Challenge
-----------------------
## ANALYSIS
------------
Three analysis that can be concluded on the basis of data analysis in weatherpy.ipynb file are:
1.Through the scatterplot of Latitude vs. Temperature Plot we can see that there is relationship between the temperature and latitude 
the temprature tends to reduce or get colder as we move towards the poles and is significantlly higher for the cities 
closer to the equator(0 degree latitude) and nearby latitudes

2.

## Part I - WeatherPy

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I used [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

The first requirement was to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The second requirement is to run linear regression on each relationship. This time,the plots were seperated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

My final notebook has:

* Randomly selected **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* A weather check on each of the cities using a series of successive API calls.
* Includes a print log of each city as it's being processed with the city number and city name.
* A CSV of all retrieved data and a PNG image for each scatter plot.

-----------------------------------------------------------------------------------------------------------------------------------------

### Part II - VacationPy

For this part of assignment,I did the following:

* Created a heat map that displays the humidity for every city from Part I.

 
* Narrowed down the DataFrame to find ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Dropped any rows that don't contain all three conditions. You want to be sure the weather is ideal.

  * **Note:** Adjusted the number to 9 for API calls and dataframe

* Used Google Places API to find the first hotel for each city located within 5000 meters of coordinates.

* Plotted the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.
------------------------------------------------------------------------------------------------------------------------------
### Techonolgy Used:
Python
Python Libraries
Google APIs
OpenWeatherMap APIs
Jupyter Notebook



