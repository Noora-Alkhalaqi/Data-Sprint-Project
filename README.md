# Olist Shipping Company Evaluation

## Project Overview

This project evaluates the performance of the shipping company used by
Olist, a Brazilian e-commerce marketplace. The analysis focuses on
whether the shipping partner is performing effectively in terms of
delivery timeliness, freight cost, reliability, and service quality.

The project includes data cleaning, exploratory data analysis,
performance evaluation, and recommendations based on the Olist
e-commerce dataset.

## Project Objectives

The main objectives are to:

-   Evaluate on-time and delayed delivery performance.
-   Analyze freight costs and the freight-to-product-price ratio.
-   Examine whether product weight, size, category, and delivery
    distance affect shipping performance.
-   Compare delivery performance across Brazilian states.
-   Compare in-state and out-of-state deliveries.
-   Investigate the relationship between shipping performance and
    customer satisfaction.
-   Analyze cancellations, complaints, damaged deliveries, and repeated
    seller-related issues.
-   Identify opportunities for improving Olist's shipping operations.

## Key Performance Indicators

  KPI                          Result
  ------------------------ ----------
  On-time delivery rate        93.22%
  Delay rate                    6.78%
  Customer satisfaction      4.09 / 5
  Freight-to-price ratio          32%

Overall, the results indicate strong on-time delivery performance, while
freight cost, regional differences, delays, and customer experience
remain important areas to monitor.

## Analysis Questions

The project investigates questions including:

-   What percentage of orders are delivered late?
-   What is the average delay duration, and how does it vary by state
    and product category?
-   Do product weight and size influence delivery delays?
-   Are delays associated with particular months, weekends, or quarters?
-   Does lateness occur even when sellers and customers are in the same
    state?
-   What is the average freight value and freight-to-price ratio?
-   How does the freight-to-price ratio vary by product category and
    state?
-   Are lighter products being overcharged?
-   How does seller-customer distance affect freight value and delivery
    time?
-   How do states with no sellers perform?
-   How do in-state and out-of-state deliveries compare?
-   How does delivery performance affect customer reviews and
    satisfaction?
-   How many cancellations or complaints relate to late or damaged
    deliveries?
-   Are repeated delivery issues concentrated among specific sellers,
    products, or categories?
-   Are delivery delays more likely to be associated with seller
    handling or carrier delivery?

## Project Files

### Data Cleaning

**`Data_Cleaning_01.ipynb`**\
Cleans and prepares the customer, seller, and geolocation datasets,
including state information.

**`Data_Cleaning_02.ipynb`**\
Cleans the orders, order items, and payment datasets. It checks data
types, duplicates, missing values, and invalid or inconsistent records.

**`Data_Cleaning_03.ipynb`**\
Cleans product and order-review data, uses the product-category
translation data, and incorporates translated review text for later
analysis.

### Data Analysis

**`Data_Analysis_01.ipynb`**\
Analyzes shipping cost and freight behavior, including freight-to-price
ratios, product weight, product categories, states, seller-customer
distance, and delivery-time estimation.

**`Data_Analyzing_02.ipynb`**\
Focuses on delivery delays, including late-order percentage, time
patterns, same-state deliveries, product weight and size, and average
delay duration by state and product category.

**`Data_Analyzing_03.ipynb`**\
Examines geographic and service-quality performance. It analyzes states
without sellers, in-state versus out-of-state shipping, regional
performance, seller-customer distance, customer satisfaction,
cancellations, complaints, seller issues, damaged products, and
responsibility for delays.

**`Olist Shipping Company Evaluation.pptx`**\
Summarizes the project questions, analysis findings, KPIs, conclusions,
and recommendations.

## Data Preparation

The cleaning process includes:

1.  Loading the original Olist datasets.
2.  Checking and correcting data types.
3.  Checking duplicate records.
4.  Investigating missing values.
5.  Checking invalid or inconsistent records.
6.  Preparing state and geographic information.
7.  Cleaning product and review data.
8.  Incorporating English translations where required.
9.  Saving cleaned datasets for analysis.

## Analysis Approach

The notebooks use Python-based data analysis to combine information from
orders, customers, sellers, products, reviews, order items, and
geolocation data.

The analysis includes:

-   DataFrame filtering and aggregation
-   Dataset merging
-   Group-based comparisons
-   Delivery-delay calculations
-   Freight and price calculations
-   Geographic distance calculations
-   Product weight and size grouping
-   State and regional comparisons
-   Review-score analysis
-   Complaint and cancellation analysis
-   Seller-level delivery issue analysis
-   Data visualization

## Tools and Libraries

The project is implemented in Jupyter Notebook using Python. Libraries
used across the notebooks include:

-   `pandas`
-   `numpy`
-   `matplotlib`
-   `seaborn`
-   `geopy`

## Main Findings

The evaluation found that:

-   93.22% of orders were delivered on time.
-   6.78% of orders were delayed.
-   Average customer satisfaction was 4.09 out of 5.
-   The overall freight-to-price ratio was 32%.
-   Freight pricing generally increases with product weight and delivery
    distance.
-   Shipping performance differs across geographic areas and delivery
    types.
-   Delivery performance is connected to customer satisfaction and
    review outcomes.
-   Seller handling and carrier delivery stages can be examined
    separately to better identify responsibility for delivery problems.

## Recommendation

The project recommends that Olist continue working with its current
shipping partner while regularly monitoring delivery performance and
customer reviews.

As an improvement, Olist can develop a **machine-learning model that
predicts whether an order is likely to be delivered on time or
delayed**. This could help identify high-risk orders earlier and support
proactive delivery management.

## Suggested Repository Structure

``` text
olist-shipping-evaluation/
│
├── Data_Cleaning_01.ipynb
├── Data_Cleaning_02.ipynb
├── Data_Cleaning_03.ipynb
├── Data_Analysis_01.ipynb
├── Data_Analyzing_02.ipynb
├── Data_Analyzing_03.ipynb
├── Olist Shipping Company Evaluation.pptx
└── README.md
```

## Team

**Narrow Insights Analytics**

## Conclusion

The project provides a data-driven evaluation of Olist's shipping
performance by combining delivery, freight, geographic, seller, product,
and customer-review information. The findings support continued use of
the current shipping partner while emphasizing continuous performance
monitoring and predictive analytics to reduce future delivery risk.

## Resourses

https://olist.com/
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
https://www.bbc.com/news/business-48386415
https://www.lloydsbanktrade.com/en/market-potential/brazil/ecommerce
https://www.latintimes.com/brazil-correios-postal-service-strike-explained-whats-settled-whats-not-why-your-package-599440