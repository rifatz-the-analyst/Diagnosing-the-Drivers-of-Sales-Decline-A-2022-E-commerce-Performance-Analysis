# Diagnosing the Drivers of Sales Decline: A 2022 E-commerce Performance Analysis

## Project Background

### Business Context

Vrinda Store is an Indian fashion retailer that sells apparel through multiple online marketplaces, including Amazon, Myntra, Ajio, Flipkart, and other e-commerce channels. Throughout 2022, the company experienced a noticeable decline in sales performance despite maintaining healthy operational performance.

As a Data Analyst, the objective of this project is to identify the key drivers behind the declining sales performance and provide data-driven recommendations to support future business decisions. The analysis focuses on understanding whether the decline was driven by products, sales channels, customer behavior, pricing, or geographic markets.

### Business Questions

This analysis aims to answer the following business questions:

1.	How did revenue and completed orders change throughout 2022? 
2.	Was the decline in revenue primarily driven by fewer transactions or changes in Average Order Value (AOV)? 
3.	Which product categories contributed most to revenue, and which had the greatest impact on the decline? 
4.	Which sales channels contributed most to business performance, and where did the largest declines occur? 
5.	Which geographic markets generated the highest revenue? 
6.	What business opportunities can be prioritized to recover lost revenue?

## Data Preparation & Data Structure

### Data Source

The dataset contains approximately 31,000 e-commerce transactions from Vrinda Store covering January–December 2022.
Each transaction includes:

- Order information
- Customer demographics
- Product information
- Sales channel
- Order status
- Pricing
- Geographic information

### Data Cleaning & Preparation

The following preparation steps were performed before analysis:

- Removed duplicate records.
- Standardized text fields (product category, state, sales channel).
- Converted the Date column into a proper date format.
- Created a Month column for monthly trend analysis.
- Filtered Delivered orders to calculate Net Sales and Completed Orders.
- Created calculated metrics
- Validated transaction values by confirming:

  Amount = Price × Quantity

### Key Metrics

The following business metrics were used throughout the analysis.

Metric	Description
Net Sales	Revenue from Delivered orders only
Completed Orders	Number of Delivered orders
Average Order Value (AOV)	Net Sales ÷ Completed Orders
Revenue Contribution	Percentage contribution to total revenue
Revenue Decline	January vs December revenue difference
Compound Monthly Growth Rate (CMGR)	Average monthly growth/decline rate
Correlation Coefficient	Relationship between revenue, orders, and AOV
Estimated Revenue Recovery	Estimated recoverable revenue based on identified opportunities

### Data Model

The analysis was performed using a single transaction table containing customer, product, sales, and geographic information.
Primary dimensions include:

- Date
- Product Category
- Sales Channel
- Customer Segment
- State 

Fact measures include:

- Revenue
- Orders
- Quantity
- Price
- Amount

## Executive Summary

1.	Vrinda Store experienced a 13.95% decline in revenue between January and December 2022, with an average monthly decline (CMGR) of -1.36%. Although monthly sales fluctuated, the overall trend remained downward throughout the year.

2.	Correlation analysis revealed that revenue had a very strong relationship with completed orders (r = 0.99) but only a weak relationship with Average Order Value (r = 0.30). This indicates that declining revenue was primarily associated with fewer completed transactions rather than lower customer spending per order.

3.	Further analysis identified the Set product category and the Amazon sales channel as the largest contributors to declining performance. The Set category generated over half of total revenue but also accounted for 76% of the overall revenue decline, while Amazon contributed 59% of the decline across all sales channels.

4.	Geographically, the company's five largest states generated 52% of total revenue but also accounted for one-third of the overall revenue decline. Despite having below-average selling prices, these markets generated strong revenue through high transaction volume, reinforcing that business performance was primarily volume-driven rather than price-driven.

5.	Overall, the findings suggest that future growth should focus on recovering transaction volume, particularly within the Set category on Amazon and in the company's highest-performing geographic markets.

## Analysis & Insights

### 1.	Revenue Declined Primarily Because Fewer Orders Were Completed

Revenue and completed orders both followed an overall downward trend throughout 2022, despite temporary increases in March and August. Net sales fell by 13.95% between January and December, representing a total decline of 240,533, with a Compound Monthly Growth Rate (CMGR) of -1.36%. The negative trendline slope further confirms the overall downward direction of sales throughout the year.
A correlation analysis showed a very strong relationship between revenue and completed orders (r = 0.99), while the relationship between revenue and Average Order Value (AOV) was much weaker (r = 0.30). This indicates that the decline in revenue was primarily associated with fewer completed transactions rather than lower spending per order.

### 2.	Heavy Dependence on the Set Category and Amazon Increased Business Risk

The Set category generated 50.69% of total revenue, making it the business's primary revenue driver. However, it also accounted for approximately 76% of the overall revenue decline, highlighting a strong dependence on a single product category.
Similarly, Amazon contributed 35% of all completed orders but accounted for approximately 59% of the total revenue decline. Further analysis shows that 49% of the Set category's revenue decline occurred through the Amazon channel. Combined, the decline in the Set category and the Amazon channel explains approximately 37% of the total revenue decline, making them the largest contributors to the business's declining performance.

### 3.	Revenue Was Driven More by Transaction Volume Than Product Pricing

Although total revenue declined, Average Order Value (AOV) remained relatively stable throughout the year. This suggests that customer purchasing behavior per transaction changed very little, while the number of completed purchases declined substantially.
Interestingly, the Set category had the lowest average selling price on Amazon (₹842) but still generated the highest revenue (₹3.55 million) on the platform. This indicates that the category's strong sales performance was driven by high transaction volume rather than premium pricing, reinforcing the importance of maintaining demand for this product line.

## 4.	Revenue Declined in the Company's Largest Markets

The top five states, which contributed 52% of total revenue, experienced a combined sales decline of 79,160, accounting for approximately 33% of the overall revenue decline. This suggests that the downturn affected the company's core markets rather than only smaller regions.
Within these key markets, the Set category declined by 51,620, with 65% of that decline coming from Amazon. This reinforces the conclusion that reduced demand for the Set category on Amazon was one of the primary factors behind the overall decline in business performance.

Furthermore, the top five states have an average selling price (₹673.70) that was lower than the overall average (₹710.20). Combined with the strong correlation between revenue and completed orders (r = 0.99) and the relatively weak relationship between revenue and AOV (r = 0.30), this suggests that revenue in the company's core markets is primarily driven by transaction volume rather than higher-priced purchases.

## Recommendations

### 1.	Increase Transaction Volume by Optimizing the Sales Funnel

**Finding**

Correlation analysis showed a very strong relationship between revenue and completed orders (r = 0.99), while the relationship between revenue and Average Order Value (AOV) was much weaker (r = 0.30). This indicates that the decline in revenue was primarily associated with fewer completed transactions rather than lower spending per order.

**Recommendation**

Conduct a deeper analysis of the customer acquisition and sales funnel to identify where transaction volume is declining for specific product categories and sales channels. Focus on determining whether the decline is caused by reduced customer traffic, lower conversion rates, or both.

Understanding where customers drop off in the purchasing journey will help the business prioritize improvements with the greatest potential to increase completed orders.

**Expected Impact**

- Identify opportunities to increase customer traffic and conversion rates.
- Determine whether traffic is primarily generated through paid or organic channels.
- Identify bottlenecks in the sales funnel and prioritize improvements that can increase completed transactions.

### 2.	Prioritize the Set Category on Amazon

**Finding**

The Set category and the Amazon channel were the largest contributors to declining business performance. The Set category accounted for approximately 76% of the total revenue decline, while Amazon accounted for 59%. Combined, they explained approximately 37% of the overall revenue decline.

Estimated revenue decline:

- Set category: ₹182,805
- Amazon channel: ₹141,915
- Set category on Amazon: ₹88,997 

**Recommendation**

Prioritize improving the performance of the Set category on Amazon by increasing product visibility, optimizing product listings, evaluating product quality, reviewing customer feedback, and benchmarking against competitors. At the same time, strengthen the performance of other product categories to reduce dependence on a single revenue source.

Because the largest revenue decline occurred within the Set category on Amazon, improving performance in this area provides the greatest opportunity to recover lost revenue while reducing future business risk through product diversification.

**Expected Impact**

If the business recovers at least 25% of the lost revenue:

- Recover approximately ₹45,701 in Set category revenue.
- Recover approximately ₹35,479 in Amazon revenue.
- Recover approximately ₹22,249 from Set sales on Amazon. 

In addition, improving the performance of other product categories can help diversify revenue and reduce reliance on a single product line.

### 3.	Strengthen Performance in Core Markets

**Finding**

The top five states generated 52% of total revenue despite having an average selling price (₹673.70) below the overall average (₹710.20). Combined with the strong relationship between revenue and completed orders, this suggests that these markets generate revenue primarily through high transaction volume rather than higher-priced purchases.

The top five states also accounted for approximately ₹79,375, or 33%, of the overall revenue decline.

**Recommendation**

Prioritize marketing campaigns and customer retention initiatives in the top five revenue-generating states to increase transaction volume. At the same time, analyse lower-performing states to identify regions with strong market potential for future expansion.

Since the company's largest markets depend on transaction volume, increasing completed orders in these regions is likely to have the greatest impact on overall revenue recovery while creating opportunities for sustainable long-term growth.

**Expected Impact**

If sales performance in the top five states improves by 25%, the business could potentially recover approximately ₹19,844 in revenue.
In addition, identifying promising lower-performing markets may help expand the customer base and reduce dependence on the current core regions.
