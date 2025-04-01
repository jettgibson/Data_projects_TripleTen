# TripleTen Sprint 5 Project / SuperStore Returns

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

I first joined the two groups of data, Returns & Orders. Followed by creating a calculated field where null values are 0, and Yes values are 1. I then began analyzing the data to find the root clauses for returned orders by building the following:
- a scatterplot showing the correlation between total sales and total returns
- a bar chart showing the return rate by product category
- the return rate by customer. To find customers who are more prone to making returns
- a map showing the return rate by some geographic measure (state, city, etc.) to see if there is a geographic concentration to returned orders
- the return rate by some measure of time (month, week, etc.) to see if there is a seasonal effect to returned orders
- a bar chart showing the return rate by segment of customer and product category

I then created a dashboard for all of the charts to be displayed on. Along with creating a story to show which states exactly had the highest rates of returns, and what product category they were more prone to return.  

### Conclusion

After the analysis, I recommended to Superstore that the returned orders could be due a variety of issues, including:
- Product Quality issues
- Shipment errors
- Customer Dissatisfaction

But to mainly focus on the Western Region of the country, where a majority of returns were taking place. With California, Oregon, & Utah being the top 3 states with the highest rate of return, across all catagories.
