# World_Weather_Analysis
## Module 6
### Deliverable 1 
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
I have used the date from WeatherPy_Database.csv to create city_data Dataframe. I then prompt the user to enter the minimum and maximum temperature criteria. this I enter -10 tp 80. 
