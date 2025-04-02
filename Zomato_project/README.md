# TripleTen Final Project / Zomato Customer Analysis
This is the 7th project I worked on in the TripleTen Business Intelligence Analyst program. This project was the largest & most independent project I have done.

#### Link to Tableau Page: https://public.tableau.com/app/profile/jett.gibson/viz/TripleTenFinalProject_17424952764840/TotalSalesbyYearOccupation

### Zomato Customer Analysis

The goal of the project was to analyze who Zomato's customers were and what were their spending habits.

#### The Data

The data was spread across two files:

- `users.csv`: each row corresponds to one customer  
    - `'F1'`: number of row  
    - `'user_id'`: ID number that uniquely identifies each user
    - `'name'`: name of customer 
    - `'age'`: age of customer  
    - `'gender'`: gender of customer  
    - `'marital_status'`: marital status of each customer  
    - `'occupation'`: occupation for each customer 
    - `'monthly_income'`: montly income for each customer 
    - `'education_qualifications'`: edcuation qualification for each customer
    - `'family_size'`: how many family members each customer has 
- `orders.csv`: each row corresponds to a unique order  
    - `'F1'`: number of row  
    - `'order_date'`: the date the order was placed
    - `'sales_qnt'`: amount of orders placed
    - `'sales_amount'`: amount of money made
    - `'user_id'`: the date the order was placed
    - `'order_date'`: ID number that uniquely identifies each user

The data is provided by TripleTen, who took it from Kaggle and modified it.

#### The Process

I first explored the dataset to see which two groups of data I could inner join to conduct the analysis. I then began segmenting the customers by their occupation, monthly income, and martial status to see if there was a certain type of customer that used Zomato's services more than any other. I ran these segments of customers against the amount of sales, to see who was spending the most money on Zomato's services. I then began analyzing each segment of customer by their spending habits over time. What particular days of the week they were most active, what particular months they most active, etc. 

### Conclusion

After my analysis, I found that Zomato's customers are primarily young, single students who use their services primarily during the week, Monday through Friday, most likely during the school/work week. In order to boost overall performance for Zomato, I made the following suggestions:
- Student discounts
- Study Hour Promotions
- Campus Sponsorships
- Delivery Bundles
