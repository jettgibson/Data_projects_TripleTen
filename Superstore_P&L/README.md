# TripleTen Sprint 4 Project / Superstore Profit & Loss

This is the 4th project I worked on in the TripleTen Business Intelligence Analyst program. This project was an introduction to Tableau.

#### Link to Tableau Page: https://public.tableau.com/app/profile/jett.gibson/viz/Sprint4Project_17405932009990/Returns2

### Superstore Profit & Loss

The goal of the project was to analyze Superstore's operation and increase it's profitability.

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

I first identified the important centers of profit and loss by segmenting pairs of dimensions together, to find which pairs would be the most profitable and which pairs would be the biggest losses. I then identified which products Superstore should stop selling, due to lack of performance. Along with indentifying which 3 subcategory items Superstore should focus on and which 3 they should stop selling. 

I then analyzed the 3 best combinations of states and months to advertise in, in order to determine which states/months would have the highest rate of return on investment in advertising. To do so, I made a visualization for the 3 states with the highest average profit for each month in the calendar year. Which helped determine exactly how much Superstore should be willing to spend on advertising in these states, and when to do so.

Finally, we evaluated the data to see if there were any products that had abnormal rates of returns. To do so, I created a calculated field where the null values are 0 and the Yes values are 1. I then used this calculated field to build a visualization for products with the highest return rate and also which customers were more prone to return items. I then built a visualization that ran the average profit against the average return rate for products by category and state. 

### Conclusion

After the analysis, I recommended that Superstore stop selling products such as Bookcases, Supplies, & Tables. And to focu on selling Copiers, Phones, & Accessories.
For Advertising, I recommended that Superstore focus Advertising in Indiana in the month of October, Vermont in the month of November, Washington in the month of March.
Lastly, for the products that had abnormal rates of returns, I found that Binders, Paper, and Accessories were the products that were the most prone to being returned by consumers and made suggestions to Superstore to help reduce the amount of returns. Along with making suggestions to help reduce the amount of returns in states such as Colorado, Oregon, Ohio, & Texas.
