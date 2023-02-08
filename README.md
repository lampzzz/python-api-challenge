# python-api-challenge

In this repository there are two python notebooks included. The first, WeatherPy, does an API call on openweathermap.org to generate a list of cities around the world with their weather for the day and creates a DataFrame from this information (saved as cities.csv in the output_data folder). This DataFrame is then split across the northern and southern hemispheres (Latitude > 0 or Latitude < 0, respectively) and used generate some scatter plots (saved as fig1-4 in the output_data folder) and linear regressions comparing different weather recordings (Max Temp, Humidity, Cloudiness, and Wind Speed) against the Latitudes of our cities. A discussion of the linear relationships is included for each regression generated.

Next, in VacationPy, our program uses our previously stored cities.csv to map out all of our stored cities according to their Latitude and Longitude on a world map. We then spend some time filtering our DataFrame to only include cities fitting a desired weather criteria for our "vacation" (in this case we have criteria: Max Temp between 21 and 27 C, Wind Speed less than 4.5 m/s, and Cloudiness = 0%). After filtering our data, we use another API call to geoapify.com to find the closest hotel to each of our matching cities and map our new selection of cities together with the Country and name of the hotel we found in our API call for easy referencing in the future.
