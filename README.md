Business Problem

The retail leadership team wants to understand which business factors influence monthly store sales. Regression analysis is used to identify important variables associated with sales performance and provide evidence-based recommendations.

Dataset Description

The dataset contains monthly performance information for 80 stores across 4 months.

Dependent Variable
monthly_sales
Independent Variables
marketing_spend
footfall
avg_discount_pct
staff_count
inventory_availability_pct
competitor_distance_km
holiday_flag
customer_rating
region
store_type
Numerical Variables
marketing_spend
footfall
avg_discount_pct
staff_count
inventory_availability_pct
competitor_distance_km
customer_rating
monthly_sales
monthly_profit
Categorical Variables
region
store_type
Variables Requiring Cleaning
customer_rating
competitor_distance_km

Missing values were replaced using median values.

Variables Not Used
store_id
month
monthly_profit

Reason:

store_id is an identifier
month is not meaningful for this regression
monthly_profit is another outcome variable rather than a predictor
