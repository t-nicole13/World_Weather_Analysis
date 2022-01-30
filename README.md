# World_Weather_Analysis

## Original Objective
- Goal: PlanMyTrip will use weather data to recommend ideal hotels based on client's weather prefrences.
- Task: Create a Pandas DataFrame with 500+ of the world's unique cities and their weather data in real time.
- Analysis:
    1.  Collect the data: 
        - NumPy (To generate 1500+ random latitudes and longitudes.)
        - citipy (To list the nearest city to the latitudes and longitudes.)
        - OpenWeatherMap API (To Request the current weather data from each unique city in the list.)
        - JSON (To collect the data and add it to a DataFrame.)
    
    2. Exploratory Analysis with Visualization:
        - Scatter Plots (To show weather data.)
        - Linear Regression (Determine correlations for weather data.)
        - Google Maps & Places API (To create a series of heatmaps.)

    3. Visualize Travel Data:
        - Add pop-up markers to the heatmaps to display information on specific cities based on customer's travel preferences.
    
## New Objective
- Goal: Make a few changes to the PlanMyTrip app to take the app to the next level.
- Tasks: 
    - Add the weather description to the weather data I've already retrieved.
    - Have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. 
    - Use the Google Maps Directions API to create a travel route between the four cities as well as a marker layer map.

- Analysis:
    1. Deliverable 1: Retrieve Weather Data
        - Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap.
        - Retrieve the current weather description for each city.
        - Create a new DataFrame containing the updated weather data.
    2. Deliverable 2: Create a Customer Travel Destinations Map
        - Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby.
        - Show those destinations on a marker layer map with pop-up markers.
    3. Deliverable 3: Create a Travel Itinerary Map
        - Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations.
        - Create a marker layer map with a pop-up marker for each city on the itinerary.

## Resources
- Software: Python 3.7.11, Jupyter Notebook 6.4.5
- Libraries: Numpy 1.20.3, Pandas 1.3.4, Matplotlib 3.5.0, citipy 0.0.5, Requests 2.26.0, SciPy 



## Results
- City Latitude vs Maximum Temperature: The temperature decreases when the latitude increases.
    ![Fig1](https://user-images.githubusercontent.com/33010018/151690116-d608cc67-b019-4b29-939f-c6c77e3c6452.png)

- For City Latitude vs Humidity, City Latitude vs Cloudiness, and City Latitude vs Wind Speed, the markers are all over the place on each map.  I couldn't determine if the latitude affected the humidity, cloudiness, or wind speed.
    ![Fig2](https://user-images.githubusercontent.com/33010018/151690124-5d4dd4e2-3ed3-4c35-a8ca-20ec71972a3c.png)  
    ![Fig3](https://user-images.githubusercontent.com/33010018/151690130-eed50364-0eae-4c11-a283-6bad22c434d4.png) 
    ![Fig4](https://user-images.githubusercontent.com/33010018/151690135-2a81a9ff-1ad6-4c8a-a1fb-411d8aaf3263.png)
- Correlation
    - Latitude vs Max Temperature (Northern Hemisphere): The max temperature decreases when the latitude increases.
    - Latitude vs Max Temperature (Southern Hemisphere): Can't determine a strong correlation between the 2 values.

    - Latitude vs Percent Humidity (Northern Hemisphere): Can't determine a strong correlation between the 2 values.
    - Latitude vs Percent Humidity (Southern Hemisphere):  Can't determine a strong correlation between the 2 values.

    - Latitude vs Percent Cloudiness (Northern Hemisphere):  Can't determine a strong correlation between the 2 values.
    - Latitude vs Percent Cloudiness (Southern Hemisphere): Can't determine a strong correlation between the 2 values.

    - Latitude vs Wind Speed (Northern Hemisphere): Can't determine a strong correlation between the 2 values.
    - Latitude vs Wind Speed (Northern Hemisphere): Can't determine a strong correlation between the 2 values.

- Vacation Itinerary
    - Travel Map
    ![WeatherPy_travel_map](https://user-images.githubusercontent.com/33010018/151690195-fafff25d-329c-4c8a-a03b-d532aef92adc.png)
    
    - Travel Map Markers
    ![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/33010018/151690214-75213aae-fe7b-4fb8-a26c-4db0580e2282.png)

- Vacation Search
    - Weather Vacation Map
    ![ WeatherPy_vacation_map](https://user-images.githubusercontent.com/33010018/151690258-f65207e5-0f59-41d4-b3be-9d8df46a3f01.png)





