# TripleTen Sprint 3 Project / E-Commerce Company Analysis
This is the 3rd project I worked on in the TripleTen Business Intelligence Analyst program. This project was the most in depth and complex project we worked on with Advanced Spreadsheets.

### E-Commerce Company Analysis

The goal of the project was to analyze and understand how well the website is converting product page views into purchases.

#### The Data

The dataset has the following columns:

- `users.csv`: each row corresponds to one customer  
    - `'user_id'`: unique customer IDs
    - `'event_type'`: the type of activity by the user
    - `'category_code'`: category of the product being viewed or purchased
    - `'brand'`: company that makes the product
    - `'price'`: price of the product, in USD
    - `'event_date'`: date of the user activity, in YYYY-MM-DD format

The data is provided by TripleTen, who took it from Kaggle and modified it.

#### The Process

I started the analysis by building a conversion funnel of how users interacted with the website, to help the stakeholder better understand how well the website is converting product page views into purchases. I then built acquisition cohorts based on the month of a user’s first purchase, and tracked cohort metrics month by month. After isolating user purchase activity into it's own table, I then calculated the first purchase date for each user who made a purchase and broke down their purchase dates into 3 columns: `'event_month'`, `'first_purchase_month'`, and `'cohort_age'`. Finally, I was able to aggregate the purchase data into cohorts and then calculate retention rates for each cohort month by month.

### Conclusion

During the analysis, I discovered the following:
- Of all the users that visited the sites page, 29% of users would add an item to their shopping cart, and 36% of those users would make a purchase.
- Users that made a first time purchase on the website are not likely to return and make a second purchase.

I recommended to the E-Commerce Company afterwards that they may want to look at making changes/improving the websites design in order to increase the amount of users adding products to their shopping cart and make purchases. Along with sending reminders to users with items in their shopping cart but have not made a purchase yet. Website promotions may also give a boost to users adding items to their shopping cart, and subsequently making a purchase. With users that made a first purchase, the E-Commerce Company may want to look at sending followup's & promotions to boost sales & repeat users.
