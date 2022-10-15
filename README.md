# World_Weather_Analysis
## Module 6
### Deliverable 1: Retrieve Weather Data  
The following information was retrieved from the API call
- Latitude and longitude
- Maximum temperature
- Percent humidity
- Percent cloudiness
- Wind speed
- Weather description (for example, clouds, fog, light rain, clear sky)
I used the city_data variable is an emplty list the would hold the infomation. A For loop was use to retrived the weather information. This can be viewed in the file [Weather_Database.ipynb in 7 out 7](https://github.com/JaredTMurray/World_Weather_Analysis/blob/main/Weather_Database/Weather_Database.ipynb)
The columns were reorder to have country as the second colums.
This image 1 below shows the city_ data first 5 rows
![Image 1](https://github.com/JaredTMurray/World_Weather_Analysis/blob/main/weather_data/Deliverable%201%20cities.png)

### Deliverable 2: Create a Customer Travel Destinations Map 
In this deliverable I did the following
- Add the weather data to a DataFrame: I use the city_data list to create a new pandas DataFrame by passing city_data_df = pd.DataFrame(city_data). Image 1 above illustrates the dataset 
- Add the config.py file to the .gitignore file: This was done and imposted the from the config file
- Create input statements 
- Filter a DataFrame using the loc method
- Retrieve hotel data
- Add data to a pop-up marker
- Create a marker layer map

Please Click on [Vacaction_Search](https://github.com/JaredTMurray/World_Weather_Analysis/blob/main/Vacation_Search/Vacation_Search.ipynb) to view the code
I have used the date from WeatherPy_Database.csv to create city_data Dataframe. I then prompt the user to enter the minimum and maximum temperature criteria. This I enter -10 to 80. I then clean up the data by using dropna function to create clean_travel_cities.df dataframe. I added a new column for the Hotel name and also set up my G-Key to access map and locations for the hotels. To highlight the map I add makers and info box 

_heat_layer = gmaps.heatmap_layer(locations, weights=max_temp,dissipating=False, max_intensity=300, point_radius=4)_
_marker_layer = gmaps.marker_layer(locations, info_box_content=hotel_info)_

The following image genertated from the [Vacaction_Search](https://github.com/JaredTMurray/World_Weather_Analysis/blob/main/Vacation_Search/Vacation_Search.ipynb) illustrate the heat layer, the marker layer and the information content box for hotels located in US

![](https://github.com/JaredTMurray/World_Weather_Analysis/blob/main/weather_data/Deliverable%202.png)

### Deliverable 3: Create a Travel Itinerary Map 
To resolve and create the travel itinerary i imparted the config file through (Import API key, from config import g_key). I create a marker layer map with a pop-up marker for each city on the itinerary. The cities on the itinerary are 
- Start and End city are Broome
- 1st city is Palmer
- 2nd city is Bethel
- 3rd city is WestBury
