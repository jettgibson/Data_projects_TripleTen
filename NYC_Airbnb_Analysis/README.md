# TripleTen Sprint 1 Project / NYC Airbnb Analysis
This was the very first project I worked on in the TripleTen Business Intelligence Analyst program. This project introduced me to Advanced Spreadsheets and a little bit of data visualization.

#### Link to Page: https://docs.google.com/spreadsheets/d/1onIaA13q_bJOESTcrwANEDGfe0y1ANWXmY5m34IC2lE/edit?usp=sharing

### NYC Airbnb Analysis

The goal of this project was to analyze the Manhattan vacation rental market in order to help a client decide on what type of property they should purchase for an Airbnb.

#### The Data

The dataset has the following columns:

- `processed_listings.csv`: each row corresponds to one listing  
    - `'id'`: unique listing IDs
    - `'last_scraped'`: the date of which the listing information was pulled
    - `'source'`: where the listing was sourced from
    - `'neighborhood_clean'`: the name of the neighborhood the listing is located
    - `'top_listing'`: `1` if yes, the listing is regarded as a 'top listing', `0` if no, the listing is not regarded as a 'top listing'
    - `'property_type'`: what type of property the listing is
    - `'accomodates'`: how many guests the listing accomodates
    - `'bedrooms_clean'`: how many bedrooms the listing has
    - `'beds'`: the amount of beds the listing contains
    - `'bathrooms_text'`: how many bathrooms the listing has in text format
    - `'revenue_earned'`: how much revenue the listing generates on a monthly basis
    - `'annual_revenue'`: how much revenue the listing generates on a annual basis
    - `'price'`: how much the listing charges per night
    - `'minimum_nights'`: the minimum amount of nights a guest must rent out the listing
    - `'maximum_nights'`: the maximum amount of nights a guest must rent out the listing
    - `'number_of_reviews'`: amount of reviews the listing has
    - `'number_of_reviews_ltm'`: amount of reviews the listing has received over the last 12 months
  
The data is provided by TripleTen, who took it from Airbnb and modified it.

#### The Process

I started the analysis by first cleaning the raw data, removing any inconsistent capitalization, trailing spaces, and empty cells from the columns, as well as removing any columns that would not be useful to the analysis. I then built a pivot table to show the 10 most attractive neighborhoods for vacation rentals based on the number of reviews a listing had, I also added a bar chart for visual representation of the neighborhoods. I created another pivot table, this time displaying which property sizes (amount of bedrooms) were most popular for vacation rentals based on the number of reviews over the last 12 months. 
The client wanted to see if different neighborhoods had different preferences for property sizes, so I updated the pivot table to recommend specific property sizes for each of the top 10 neighborhoods. Lastly, I created another pivot table showing the top listings annual revenue so that the client could have an idea of potential revenue annually.

### Conclusion

Once the analysis was complete, I recommended to the client that properties located in Lower East Side, Hells Kitchen, & Harlem with 1 bedroom were the most attractive vacation rentals. With the highest rated listing having produced $359,280.00 for the year, at the time the data was pulled.
