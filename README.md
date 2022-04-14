# Python-API-Challenge

## Part I - WeatherPy
A Python script was created to visualise the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, the Python library, the OpenWeatherMap API, was utilised to create a representative model of weather across world cities.
A series of scatter plots were created to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

Then linear regression was run on each relationship. The plots were separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

## Part II - VacationPy

A heat map was created that displays the humidity for every city from Part I.
The DataFrame was narrowed down to find the ideal weather condition. For example:
- A max temperature lower than 80 degrees but higher than 70.
- Wind speed less than 10 mph.
- Zero cloudiness.
(Any rows that did not contain all three conditions were dropped.)

Finally, Google Places API was used to find the first hotel for each city located within 5000 meters of the coordinates and the hotels were plotted on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
