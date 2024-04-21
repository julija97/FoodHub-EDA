# FoodHub-EDA
### Context

The number of restaurants in New York is increasing day by day. Lots of students and busy professionals rely on those restaurants due to their hectic lifestyles. Online food delivery service is a great option for them. It provides them with good food from their favorite restaurants. A food aggregator company FoodHub offers access to multiple restaurants through a single smartphone app.

The app allows the restaurants to receive a direct online order from a customer. The app assigns a delivery person from the company to pick up the order after it is confirmed by the restaurant. The delivery person then uses the map to reach the restaurant and waits for the food package. Once the food package is handed over to the delivery person, he/she confirms the pick-up in the app and travels to the customer's location to deliver the food. The delivery person confirms the drop-off in the app after delivering the food package to the customer. The customer can rate the order in the app. The food aggregator earns money by collecting a fixed margin of the delivery order from the restaurants.

### Objective

The food aggregator company has stored the data of the different orders made by the registered customers in their online portal. They want to analyze the data to get a fair idea about the demand of different restaurants which will help them in enhancing their customer experience. Suppose you are hired as a Data Scientist in this company and the Data Science team has shared some of the key questions that need to be answered. Perform the data analysis to find answers to these questions that will help the company to improve the business.

### Data Description

The data contains the different data related to a food order. The detailed data dictionary is given below.

### Data Dictionary

* order_id: Unique ID of the order
* customer_id: ID of the customer who ordered the food
* restaurant_name: Name of the restaurant
* cuisine_type: Cuisine ordered by the customer
* cost: Cost of the order
* day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
* rating: Rating given by the customer out of 5
* food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
* delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information

### Conclusions:
* American, Japanese and Italian cuisines are the most popular based on the orders placed.
*  Thai and French cusine type restaurants generate the most revenue on average due to the highest cost of orders.
* Korean restaurants show to have the lowest food preparation and food delivery time on average (although this should be verified with more datapoints).
*  There are a lot of orders without a rating, which causes gaps in the data.
*  Weekends receive ~60% more orders than weekdays, however, it takes ~5.8 minutes longer on average to deliver food on the weekday than a weekend, which may be due to multiple reasons such as  as higher traffic volumes, scarcity of drivers.
* American and Japanese (the top cusine types by orders placed) have a smaller variability of delivery times than Thai and French cusines which generate more profit.This is, however, likely due to a smaller number of datapoints available and is not a correct representation of real life patterns.


### Recommendations:


* Conduct thorough research on the customer demographics that prefer Thai and French cuisine restaurants, and provide personlised, geo-targeted ads, aiming to boost orders and revenue in these high-revenue generating restaurant categories. In addition, these types of restaurants shuold be targeted as partners too.

* As FoodHub earns a fixed margin per order, it would improve its net profits by increasing the number of orders delivered. By minimizing delivery time, delivery personnel can accommodate more orders efficiently. Targeting Korean restaurants would be beneficial as it has a significatly lower both food preparation and delivery time.

* As a lot of ratings are missing, it is worth to encourage customers provide ratings which would allow FoodHub to collect more data. This can be done via incentives, discounts and improving the in app experience.

* FoodHub could benefit from optimizing delivery routes better to avoid congested routes on the weekdays which would allow drivers to cut on delivery time and satisfy more orders. In addition, worth evaluating the resources allocated to satisfy the demand on the weekdays.
