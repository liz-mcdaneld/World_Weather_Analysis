# World Weather Analysis
## Overview and Objective of the Project
While working on the PlanMyTrip app, beta testers have requested additional features to enhance the app. Beta testers have recommended adding weather descriptions to the current weather data pop ups when selecting on a map marker. They have also requested to have input statements to filter the data based off user input and preference for weather temperatures. This data will then be used to find the users ideal travel destination based off the temperature preference and find nearby hotels. Beta testers will also be able to create a vacation itinerary with four cities. Using Google Maps Directions API, the app will then generate a travel route with the four cities and place markers on the map. 

## Task List
Below is a list of the task used to preform the objective of the project.

1.	Using Python and Pandas to preform analysis task.
2.	Enable and import gmaps to embed Google Maps in Jupyter Notebooks.
3.	Import requests, numpy, and citipy dependencies.
4.	Generate random latitudes and longitudes using numpy.random( ) function.
5.	Configure API keys and retrieve data from OpenWeatherMap API.
6.	Retrieve and store values from a JSON array.
7.	Resolve potential errors using try and except blocks of coding.
8.	Create and add info box and markers using the Google Maps API to show weather data and description.
9.	Store weather data into a newly created weather DataFrame and CSV files.
10.	Create input box for users to input ideal minimum and maximum temperature parameters for destination search.
11.	Clean data by dropping and null values from dataset.
12.	Using Google Nearby Search API to find hotels within set parameters and storing clean data in a new hotel DataFrame and CSV files.
13.	Add info boxes for hotel data on map with markers to show hotel and current weather data.
14.	Create a vacation itinerary route with four cities using gmaps.directions with different travel modes and display this information in a map. 
15.	Store the new data for the four cities in a new itinerary DataFrame.

## Course of Action
### Retrieve the Weather Data
An API key was established with OpenWeatherMap to retrieve latitude and longitude, maximum temperature, humidity, cloudiness, wind speed, and weather descriptions. This information was then added and stored into a new DataFrame then exported to a CSV file. 

### Create a Customer Travel Destinations Map
Input statements are added to ask beta testers for their minimum and maximum temperature preferences. This information is used to create a new DataFrame, which is cleaned from null entries and empty rows before exporting into a CSV file. Info boxes are added with pop-up markers to show hotel name, city, country, and a current weather description with the maximum temperature.
![WeatherPy_vacation_map](https://user-images.githubusercontent.com/103263248/174843280-2ca8f588-3007-4008-9f6c-350763e184de.png)


### Create an Itinerary Map
Based on each of the four cities on the itinerary, four DataFrames are created. Pairs of latitude and longitude are retrieved for each of the four cities and stored in this DataFrame.  A travel map is created with a directions layer map to show travel routes between the four cities. 
![WeatherPy_travel_map](https://user-images.githubusercontent.com/103263248/174843360-7629b628-8e69-4ad5-a697-045790898835.png)


A DataFrame containing just the four cities on the itinerary is created. Info boxes with pop-up markers for the four cities on the itinerary is generated that shows the hotel name, city, country, and current weather description with the maximum temperature. 
![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/103263248/174843415-ce6d3f49-a2e9-4878-a791-c48731e69705.png)

