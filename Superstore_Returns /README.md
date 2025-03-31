# TripleTen Sprint 5 Project

This is the 5th project I worked on in the TripleTen Business Intelligence Analyst program. This project was the most extensive project I had worked on thus far.

### Superstore Returned Orders

The goal of the project was to analyze potential problems that could be causing the high influx of returned orders for Superstore, and use Data Visualization to help the stakeholders understand the data.

#### The Data

The data was spread across three files:

- `orders.csv`: each row corresponds to one order  
    - `'category'`: name of category  
    - `'city'`: name of city  
    - `'county_region'`: name of county/region  
    - `'customer_id'`: ID number that uniquely identifies each customer  
    - `'customer_name'`: name of customer  
    - `'order_date'`: the date the order was placed  
    - `'order_id'`: ID number that uniquely identifies each order  
    - `'product_id'`: ID number that uniquely identifies each product  
    - `'product_name'`: ID number that uniquely identifies each product  
    - `'region'`: name of region  
    - `'segment'`: name of customer segment  
    - `'ship_date'`: date the order was shipped  
    - `'ship_mode'`: type of shipping  
    - `'state'`: name of state  
    - `'sub-category'`: name of sub-category item  
    - `'postal_code`: postal code the order was sent to  
    - `'profit'`: how much profit was made off the order  
    - `'quantity'`: amount of the ordered items  
    - `'row_id`: ID number that uniquely identifies each row  
    - `'sales'`: total amount of the sale  
- `people.csv`: each row corresponds to a unique person  
    - `'region'`: name of region  
    - `'regional_manager'`: name of the regional manager  
- `returns.csv`: each row corresponds to one returned order  
    - `'order_id'`: ID number that uniquely identifies each order  
    - `'returned'`: indicates if the order was returned or not

The data is provided by TripleTen, who took it from Kaggle and modified it.

#### The Process

I first explored the dataset and merged DataFrames from different sources. Finally, I analyzed the data using visualizations.

### Conclusion

Come back and write this
