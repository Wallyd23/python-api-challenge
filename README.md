# python-api-challenge
Description:

This Python project collects weather data for randomly selected cities worldwide using the OpenWeatherMap API. It then analyzes and visualizes the collected data to provide insights into how various weather parameters (e.g., temperature, humidity, cloudiness, wind speed) vary with latitude. Additionally, the script identifies ideal vacation spots based on specified weather conditions and finds nearby hotels using the Geoapify Places API.

Dependencies:

pandas: Used for data manipulation and analysis.
matplotlib: Employed for creating visualizations.
numpy: Utilized for numerical computing.
requests: Used for making HTTP requests to APIs.
scipy: Utilized for statistical analysis.
citipy: Utilized for determining the nearest city based on latitude and longitude.
hvplot: Used for interactive plotting.
geoviews: Employed for geographical data visualization.

APIs:

OpenWeatherMap API: Used to fetch current weather data for cities.
Geoapify Places API: Utilized to find nearby hotels based on geographical coordinates.

Usage:

Ensure that the required dependencies are installed in the Python environment.
Obtain an API key for the OpenWeatherMap API and Geoapify Places API. Replace the placeholder weather_api_key in the script with your OpenWeatherMap API key.
Run the Python script in a Python environment.

Functions:

1. Data Collection:
Generates random latitude and longitude coordinates.
Uses citipy to find the nearest city for each coordinate pair.
Makes API requests to OpenWeatherMap to retrieve weather data for each city.

2. Data Processing:
Cleans the collected data and stores it in a pandas DataFrame.
Saves the DataFrame to a CSV file for further analysis.

3. Data Visualization:
Creates scatter plots to visualize the relationship between latitude and various weather parameters (e.g., temperature, humidity, cloudiness, wind speed).
Generates linear regression plots to analyze the correlation between weather parameters and latitude in both the Northern and Southern Hemispheres.

4. Hotel Search:
Filters cities based on specified weather conditions to find ideal vacation spots.
Uses Geoapify Places API to search for nearby hotels for each selected city.
Stores the hotel information in a pandas DataFrame and displays it on an interactive map.