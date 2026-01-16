
<a href="/vish7715.github.io"> Home </a>

# Starbucks Rewards – Loyalty program Analysis and Customer Segmentation

## 📌 Business Use Case

Starbucks was born as a whole coffee beans seller in Pike’s place market in Seattle, Washington in 1971 . It is now the biggest coffee chain in the world expanding globally with over 40,000 stores globally as of 2025. 

As part of their Loyalty program, Starbucks rewards , different offer types have been sent to customers over a month of time. The use case is to study customer behaviour towards each offer type and then to segment those customers based on their behaviours for Starbucks to come up with data driven strategies to enhance customer experience.

---

## 🎯 Project Objectives

For this project, a simulation of the Starbucks rewards program dataset containing customers information including thr demographic details and offer types (BOGO,Discount) and interactions (offers viewed vs offers completed)  has been collected from Kaggle. 

## 📊 Business Question

In this project , key business questions to be answered are -

1. What are the most popular offer types ?
2. What is the most viewed offers vs most completed offers ?
3. Based on customers interactions within the app, what segments they can be put into ?

## 🧱 Data Structure

Dataset contains mainly 3 tables - 

### 1️⃣ profile.csv

| Column | Data Type |
|------|---------|
| gender | object |
| age | number |
| became_member_on | int64 |
| income | float 

---

### 2️⃣ portfolio.csv
| Column | Data Type |
|------|-------------|
| id | object |
| rewards | int |
| channels | object |
| difficulty | int |
| duration | int |
| offer type | onject

---

### 3️⃣ transcript.csv

| Column | Data Type |
|------|---------|
| person | object |
| event | object |
| value | object |
| time | int |

## 🛠️ Tools & Technologies
-Python (Pandas , Numpy , json)
- ML (K means clustering )

## Data Cleaning 

Data cleaning and transformation has been done via Pandas , python library. 

Python script can be found here -

(https://github.com/vish7715/Customer-Segmentation--Starbucks-Dataset/blob/main/Starbucks_campaign_data_.ipynb)


## Key Metrics for segmentation

Below metrics were used for identifying customer segments -

1. ## Frequency
   The number of transactions a customer does over the month of offer validity.
3. ## Average purchase Value
   The amount of money spent by customer over that period.
5. ## Completion Rate
   How many offers were viewed and completed by customer in the campign window.

## Data Insights 

1. What are the most popular offer types ?

   Below are the findings-
   
<img width="452" height="237" alt="image" src="images/Discount%20vs%20BOGO.png"/>
   

3. What is the most viewed offers vs most completed offers ?

   Based on Data Analysis done, below are the findings -
 
<img width="452" height="237" alt="image" src="images/Image%2012-01-26%20at%2008.59.png"/>

3. Customer Segmentation

   Using Unsupervised machine learning algorithm, K-means clustering and based on data analysis from customers and events table, customer segmentation was performed and customers were put into below clusters -

Cluster 1 - Starbucks Favourites (Most Valuable) - Highest offer completion rate which implies that this customer cluster viewed and completed the most offers.Highly responsive to offers and also the highest Average purchase value(apv) spent the most amount of money.

Cluster 2 - Regular Customers - They have highest frequency making the most number of transactions during the campaign month . Although, they have offer completion rate at 0.52 which is the average . They have low APV dusring the campaign window, which means campaigns dont affect their buying behaviour , they are regularly buying.

## 📌Recommendations

For Cluster 1 - Management should keep them as they are driving the highest sales during campign.

For Cluster 2 - Company should expose high end products to them at low cost as they are regular customers or increase products baskets(if they are buying some product regularly , should give them related products too) with them to increase stickiness.





   







