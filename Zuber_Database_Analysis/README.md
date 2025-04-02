# TripleTen Sprint 2 Project / Zuber Database Analysis
This is the 2nd project I worked on in the TripleTen Business Intelligence Analyst program. This project was my introduction to working with SQL.

### Zuber Database Analysis

The goal of the project was to find patterns in the available information, understand passenger preferences, and the impact of external factors on rides.

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
