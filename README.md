# WeatherPy and VacationPy
# Overview
This Project consists of applying OpenWeatherMap API which studies the weather patterns relative to the latitude with the aim of gathering real-time weather data. In order to perform the relation between several weather variables such as temperature, humidity, cloudiness, and wind speed and the latitude, a scatter plot and linear regression analyses is conducted. As for VacationPy is when we perceive a standard vacation spots based on weather conditions while using the Geoapify API to discover nearby hotels.

# Weather Data Analysis
I collect weather data of over 500 cities worldwide by using the OpenWeatherMap API. According to the dataset, I was able to determine the difference in the change of the weather conditions with the latitude across the globe. The analysis was divided into two parts, one is the scatter plots of weather variables vs. latitude, and the other is the linear regression analyses on these relationships by hemisphere.

# Plots Created
 - Latitude vs. Temperature
     - Generated scatter plots to showcase the relationship between latitude and temperature (both hemispheres).
       ![image](https://github.com/user-attachments/assets/3e9dec9a-a298-45bd-8b30-c1fc025f3c13 width="400" height="300")

 - Latitude vs. Humidity
  - Created scatter plots to display the relationship between latitude and humidity.
 - Latitude vs. Cloudiness
   -  Scatter plots demonstrated the relationship between latitude and cloud cover.
- Latitude vs. Wind Speed
  - Plotted the relationship between latitude and wind speed.
# Linear Regression
I applied linear regression to each weather variable against latitude for northern and southern hemispheres:
- Northern Hemisphere:
  - Temperature (°C) vs. Latitude
  - Humidity (%) vs. Latitude
  - Cloudiness (%) vs. Latitude
  - Wind Speed (m/s) vs. Latitude
- Southern Hemisphere:
  - Temperature (°C) vs. Latitude
  - Humidity (%) vs. Latitude
  - Cloudiness (%) vs. Latitude
  - Wind Speed (m/s) vs. Latitude
    
# Insights from the Linear Regressions:
- Temperature: Clear negative correlation with latitude in the Northern Hemisphere, and positive in the Southern Hemisphere.
- Humidity, Cloudiness, and Wind Speed: The R² values indicated weaker relationships, suggesting more variability across latitudes for these variables.

# VacationPy
This dataset was focused on finding vacation spots of cities with the perfect weather condition. I aimed on offering a city with comfortable temperatures, low wind speeds, clear skies, and low humidity.
# Steps:
- Map Visualization: I displayed each city on a map with the Geoapify API while using the city coordinates from the dataset.
- Ideal Weather Condition Filter: I clarified cities based on my desired weather conditions (e.g., temperature between 21°C and 27°C, low wind speed, and zero cloudiness).
- Hotel Location: I used the Geoapify API to attain the closest hotel within a 10,000-meter radius, for each of the chosen cities.
- Interactive Map: I added the hotel name and country as hover information on the map.

# Conclusion
Overall, the project instructed the relationship between weather variables and latitude, with linear regression analysis providing a better understanding into these patterns by hemisphere. Moreover, VacationPy presented a realistic method on locating vacation destinations based on desired weather conditions and nearby hotels.


# How to Run
   1. Clone the repository:
       1. Open your terminal (Git Bash, Command Prompt, or any Git client).
       2. Use the cd command to navigate to the directory where you want to clone the repository.
       3. Run the following command to clone the repository: git clone link_provided
  2. Ensure Pandas, Geoviews, Hvplot, and Census is installed on your machine.
     - Install Pandas using pip if it's not already installed (pip install pandas).
     - Install Geoviews using pip if it's not already installed (pip install geoviews).
     - Install Hvplot using pip if it's not already installed (pip install hvplot).
     - Install Census using pip if it's not already installed (pip install census).
  3. Open the cloned file in the Visual Studio Code:
       1. Go to file > Open Folder and navigate to the folder where you cloned the repository.
       2. Select the folder to open in VS code.
  4. Run the Jupyter Notebook
     1. WeatherPy.ipynb: For weather analysis.
     2. VacationPy.ipynb: For vacation spot search and hotel location mapping.
