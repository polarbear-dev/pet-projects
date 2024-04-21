# Project e-commerce

Product manager asked you to analyze completed purchases and answer the following questions:

1. How many users have made a purchase only once? 

2. How many orders per month on average are not delivered for various reasons (provide a breakdown by reasons)?

3. For each product, determine which day of the week the product is most frequently purchased.

4. How many purchases per week, on average, does each user make (per month)?

5. Conduct a cohort analysis of users. From January to December, identify the cohort with the highest retention in the 3rd month.

6. Perform RFM segmentation of users to qualitatively assess your audience. In the clustering, you can select the following metrics: R - time from the user's last purchase to the current date, F - total number of purchases by the user over time, M - total purchase amount over time. Describe in detail how you created the clusters. For each RFM segment, establish the boundaries of the recency, frequency, and monetary metrics for interpreting these clusters. An example of such a description: RFM segment 132 (recency=1, frequency=3, monetary=2) has boundaries of recency from 130 to 500 days, frequency from 2 to 5 orders per week, monetary from 1780 to 3560 dollars per week.

**To solve the problem, conduct preliminary data analysis and formulate what should be considered a purchase. Justify your choice using payment facts, order statuses, and other available data.**

Files:

* **olist_customers_datase.csv — table with unique user identifiers**

*customer_id* — post-order user identifier

*customer_unique_id* — unique user identifier (analogous to a passport number)

*customer_zip_code_prefix* — user postal code

*customer_city* — user delivery city

*customer_state* — user delivery state

* **olist_orders_dataset.csv — orders table**

*order_id* — unique order identifier (receipt number)

*customer_id* — post-order user identifier

*order_status* — order status

*order_purchase_timestamp* — order creation time

*order_approved_at* — order payment approval time

*order_delivered_carrier_date* —  order delivery carrier time

*order_delivered_customer_date* — order delivery time to the customer

*order_estimated_delivery_date* — estimated delivery date

* **olist_order_items_dataset.csv —  items included in orders**

*order_id* — unique order identifier (receipt number)

*order_item_id* — product identifier within one order

*product_id* — product identifier (barcode analog)

*seller_id* — manufacturer's product identifier

*shipping_limit_date* — maximum seller delivery date for handing over the order to a logistics partner

*price* —  price per unit of product

*freight_value* —  product weight

— The example data structure can be visualized by order_id == 00143d0f86d6fbd9f9b38ab440ac16f5

Unique order statuses in the **olist_orders_dataset table**:

* created, 
* approved, 
* invoiced, 
* processing, 
* shipped, 
* delivered, 
* unavailable, 
* canceled.
