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

I started the analysis by building a conversion funnel of how users interacted with the website, to help the stakeholder better understand how well the website is converting product page views into purchases. I then built acquisition cohorts based on the month of a user’s first purchase, and tracked cohort metrics month by month. After isolating user purchase activity into it's own table, I then calculated the first purchase date for each user who made a purchase and broke down their purchase dates into 3 columns: `'event_month'`, `'first_purchase_month'`, and `'cohort_age'`. Finally, I was able to aggregate the purchase data into cohorts and then calculate retention rates for each cohort month by month.

### Conclusion

During the analysis, I discovered the following:
