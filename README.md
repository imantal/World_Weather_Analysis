# World_Weather_Analysis

The objective of this project was to develop an app, PlanMyTrip, that uses the data to recommend ideal hotels based on clients' weather preferences. The first step was to collect and analyze weather data across cities worldwide. The second step was to find hotels based on the customer weather criteria (max and min temperatures) and the last step was to create a travel itinerary (map) based on the customer’s original and stop destinations.

## Collect the Data 

The NumPy module was used to generate more than 2,000 random latitudes and longitudes. The Citipy module was used to list the nearest city to the latitudes and longitudes. The OpenWeatherMap API was used to request the current weather data from each unique city in the list. Then, the JSON data from the API request was parsed and the following data were collected and added to a DataFrame: 

- City, country, and date
- Latitude and longitude
- Maximum temperature
- Humidity
- Cloudiness
- Wind speed
- Weather description (for example, clouds, fog, light rain, clear sky)

## Exploratory Analysis with Visualization
Scatter plots of the weather data were created for the following comparisons:
- Latitude versus temperature
- Latitude versus humidity
- Latitude versus cloudiness
- Latitude versus wind speed

The correlations for the following weather data were determined:
- Latitude and temperature
- Latitude and humidity
- Latitude and cloudiness
- Latitude and wind speed

A series of heatmaps were created using the Google Maps and Places API that showcased the following:
- Latitude and temperature
- Latitude and humidity
- Latitude and cloudiness
- Latitude and wind speed

## Visualize Travel Data

A heatmap with pop-up markers was created. It can display information on specific cities based on a customer's travel preferences: 

- The Pandas DataFrame was filtered based on user inputs for a minimum and maximum temperature.
- A heatmap created for the new DataFrame.
- Hotels were found from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
- The name of the first hotel in the DataFrame was stored.
- Pop-up markers were added to the heatmap to display information about the city, current maximum temperature, and a hotel in the city.

## Files
### Weather_Database.ipynb: to create a database of cities with their min and max temperature, current weather condition, cloudiness, etc.
### Vacation_Search.ipynb: to find hotels based on the customer weather criteria (max and min temperatures)
### Vacation_Itinerary.ipynb: to create a travel itinerary (map) based on the customer’s original and stop destinations
