# Target-Sales-Analysis-SQL-Case-Study

## About Business Case
Target is a globally renowned brand and a prominent retailer in the United States. Target makes itself a preferred shopping destination by offering outstanding value, inspiration, innovation and an exceptional guest experience that no other retailer can deliver.

This particular business case focuses on the operations of Target in Brazil and provides insightful information about 100,000 orders placed between 2016 and 2018. The dataset provides insights on:
- Order status, price, and payment methods
- Freight performance and delivery efficiency
- Customer locations and demographics
- Product attributes
- Customer reviews and satisfaction

By analyzing this extensive dataset, it becomes possible to gain valuable insights into Target's operations in Brazil. The information can shed light on various aspects of the business, such as order processing, pricing strategies, payment and shipping efficiency, customer demographics, product characteristics, and customer satisfaction levels.

## Tools 
Google BigQuery

## column description 
**Dataset:** https://drive.google.com/drive/folders/1TGEc66YKbD443nslRi1bWgVd238gJCnb
The data is available in 8 csv files:

1. customers.csv
2. sellers.csv
3. order_items.csv
4. geolocation.csv
5. payments.csv
6. reviews.csv
7. orders.csv
8. products.csv

### 1. customers.csv
| Feature | Description |
|---------|-------------|
| customer_id | ID of the consumer who made the purchase |
| customer_unique_id | Unique ID of the consumer |
| customer_zip_code_prefix | Zip code of consumer’s location |
| customer_city | City from where the order was made |
| customer_state | State code (e.g., São Paulo - SP) |

### 2. sellers.csv
| Feature | Description |
|---------|-------------|
| seller_id | Unique ID of the seller registered |
| seller_zip_code_prefix | Zip code of the seller’s location |
| seller_city | City of the seller |
| seller_state | State code (e.g., São Paulo - SP) |

### 3. order_items.csv
| Feature | Description |
|---------|-------------|
| order_id | Unique ID of the order made by the consumer |
| order_item_id | Unique ID given to each item in the order |
| product_id | Unique ID of the product |
| seller_id | Unique ID of the seller |
| shipping_limit_date | Deadline date for shipping the product |
| price | Actual price of the product |
| freight_value | Delivery cost for the product |

### 4. geolocations.csv
| Feature | Description |
|---------|-------------|
| geolocation_zip_code_prefix | First 5 digits of the Zip Code |
| geolocation_lat | Latitude |
| geolocation_lng | Longitude |
| geolocation_city | City |
| geolocation_state | State |

### 5. payments.csv
| Feature | Description |
|---------|-------------|
| order_id | Unique ID of the order |
| payment_sequential | Sequence number of the payment in EMI |
| payment_type | Mode of payment (e.g., Credit Card) |
| payment_installments | Number of installments |
| payment_value | Total amount paid |

### 6. orders.csv
| Feature | Description |
|---------|-------------|
| order_id | Unique ID of the order |
| customer_id | ID of the consumer |
| order_status | Status of the order (delivered, shipped, etc.) |
| order_purchase_timestamp | Timestamp of the purchase |
| order_delivered_carrier_date | Date carrier delivered the product |
| order_delivered_customer_date | Date customer received the product |
| order_estimated_delivery_date | Estimated delivery date |

### 7. reviews.csv
| Feature | Description |
|---------|-------------|
| review_id | ID of the review |
| order_id | Unique ID of the order |
| review_score | Score given by the customer (1–5) |
| review_comment_title | Review title |
| review_comment_message | Review message |
| review_creation_date | Timestamp of review creation |
| review_answer_timestamp | Timestamp when review was answered |

### 8. products.csv
| Feature | Description |
|---------|-------------|
| product_id | Unique identifier for the product |
| product_category_name | Product category |
| product_name_length | Length of product name |
| product_description_length | Length of product description |
| product_photos_qty | Number of product photos |
| product_weight_g | Product weight in grams |
| product_length_cm | Product length in cm |
| product_height_cm | Product height in cm |
| product_width_cm | Product width in cm |

### Dataset Schema
Please refer to the `schema.png` file in this repository to view the table relationships.

## Recommendations
● To increase orders during the low-demand months (September to December),
Target can introduce special shopping events or offer holiday deals around
Christmas and other local holidays.
● Afternoon and Night time experience the highest traffic. Target ensures that
their website runs smoothly during these peak hours. Additionally dispatch
teams are well-staffed during this period, and supported with automated alerts to
enable faster processing and timely deliveries.
● Target can reduce avg freight value and delivery time by partnering with local
vendors to enable faster delivery and lower shipping expenses. This approach
can help Boost order volume in the Northern regions like Paraiba (PB) by making
products more affordable and improving delivery speed.
● Since the mode of payment through credit card is very high Target should retain
this strategy to make the credit card payment process as smooth as possible.
● To increase debit card adoption, Target can collaborate with key banking partners
to introduce exclusive debit card deals.
● Since most customers choose one month installment or shorter plans, the
company should focus on promoting shorter installment options.
