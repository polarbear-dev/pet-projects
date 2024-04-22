# Dating App Project

Imagine you work for a large dating application.

In addition to basic functions, the application also offers a premium subscription that provides access to a range of important additional features. An A/B test was conducted, in which the cost of the premium subscription was changed for new users from several countries when purchased through two new payment systems. The cost of the trial period remained the same.

Check:

1. Was the experiment successful overall?
2. Analyse whether the innovation makes sense among any specific user groups..

*Subscription fees are charged monthly until the user cancels it.

## Data
There are three groups in total: *test*, *control_1* and *control_2*. For each of them:

users_*.csv –  user information:

* **uid** – user identifier
* **age** – age
* **attraction_coeff** – attractiveness coefficient
* **coins** – number of coins (internal currency)
* **country** – country  
* **visit_days** – days after registration when the user visited the application (e.g., 1, then 7)
* **gender** – gender
* **age_filter_start**  – search filter, min.value 
* **age_filter_end**  – search filter, max.value 
* **views_count** – number of ratings received 
* **was_premium** – whether the user was ever premium (either a trial period of premium status or purchased for money)
* **is_premium** –  whether the user is premium
* **total_revenue** – normalized revenue

transactions_*.csv – payment information of users:

* **uid** – user identifier
* **country** – country
* **joined_at** – registration date and time
* **paid_at** – purchase date and time
* **revenue** – normalized revenue
* **payment_id** – payment identifier
* **from_page** – where the user came from to the payment page
* **product_type** –  product type (trial_premium – trial premium subscription, premium_no_trial – premium subscription without trial, coins – subscription for internal currency, other_type – other)
