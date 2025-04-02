# TripleTen Sprint 2 Project / Zuber Database Analysis
This is the 2nd project I worked on in the TripleTen Business Intelligence Analyst program. This project was my introduction to working with SQL.

### Zuber Database Analysis

The goal of the project was to find patterns in the available information, understand passenger preferences, and the impact of external factors on rides.

#### The Data

The data was spread across four files:

- `neighborhoods.csv`: data on city neighborhoods 
    - `'name'`: name of the neighborhood  
    - `'neighborhood_id'`: neighborhood code  
- `cabs.csv`: data on taxis
    - `'cab_id'`: vehicle code  
    - `'vehicle_id'`: the vehicle's technical ID
    - `'company_name'`: the company that owns the vehicle
- `trips.csv`: data on rides  
    - `'trip_id'`: ride code 
    - `'cab_id'`: code of the vehicle operating the ride
    - `'start_ts'`: date and time of the beginning of the ride (time rounded to the hour)
    - `'end_ts'`: date and time of the end of the ride (time rounded to the hour)
    - `'duration_seconds'`: ride duration in seconds
    - `'distance_miles'`: ride distance in miles
    - `'pickup_location_id'`: pickup neighborhood code
    - `'dropoff_location_id'`: dropoff neighborhood code
- `weather_records.csv`: data on weather
    - `'record_id'`: weather record code
    - `'ts'`: record date and time (time rounded to the hour)
    - `'temperature'`: temperature when the record was taken
    - `'description'`: brief description of weather conditions, e.g. "light rain" or "scattered clouds" 

The data is provided by TripleTen, who took it from Kaggle and modified it.

#### The Process

To start the analysis, I analyzed data from competitors and tested a hypothesis about the impact of weather on ride frequency. I wanted to find the number of taxi rides for each taxi company for November 15-16, 2017 and sort the results by the amount of trips in descending order (doc 'Zuber_Database_Analysis(1)'). I then proceeded to find the number of rides for every taxi company whose name contains the words "Yellow" or "Blue" for November 1-7, 2017 and grouped them by the company name (doc 'Zuber_Database_Analysis(2)'). After finding that Flash Cab and Taxi Affiliation Services were the most popular taxi companies in November 2017, I wanted to know the number of rides for these two companies and group the data by the taxi company names (doc 'Zuber_Database_Analysis(3)'). 
I then had to determine if and how the duration of rides from the Loop to O'Hare International Airport changes on rainy Saturdays compared to other days of the week and other weather conditions. To do so, I retrieved the weather condition records from the `weather_records` table and split all hours into two groups: "Bad" if the description field contains the words "rain" or "storm," and "Good" for others (doc 'Zuber_Database_Analysis(4)' and doc 'Zuber_Database_Analysis(5)'. 
And finally, I retrieved the data from the `trips` table that had rides that started in the Loop (neighborhood_id: 50) and ended at O'Hare (neighborhood_id: 63) on a Saturday and retrieved the weather conditions for each ride, along with the duration (doc 'Zuber_Database_Analysis(6)'). 

### Conclusion

After the analysis was complete, 
