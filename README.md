# Amazon-Product-Review-Analysis
Designed during my time at DSA Incubator Hub. An Excel-based analytics project on Amazon product reviews, discounts, and pricing, this project uses pivot tables, slicers, calculated columns, and interactive dashboards to extract actionable insights on product performance, category trends, customer engagement, and revenue opportunities.

## Project Overview

+ Topic: Amazon Product Review Analysis

+ Client Name: RetailTech Insights

+ Industry: E-commerce Analytics

+ Role: Junior Data Analyst

+ Tools Used: Microsoft Excel (Pivot Tables, Charts, Conditional Formatting, Slicers, Cards)

  + For Data Cleaning (corrected inconsistent format and removed duplicates)

  + For Data Manipulation (Used formulas for Calculated column)

  + For Data Summarization (Used Pivot tables for summarisation and aggregation)

  + For Visualization (Used charts, pie to build visuals for analysis result)

  + For Data Analysis Filtering & KPI Display (Used cards and slicers)
 
## Dataset Representation

The raw dataset contains information scraped from Amazon product pages, including:

+ Total Records: 1,465

+ Columns: 16

+ Source: Web-scraped Amazon product review data

+ Each row represents: A unique product

+ Data Fields Includes:

  + Product name

  + Product Category

  + Product Price

  + Product Discount

  + Product Ratings

  + User Reviews

  + Review Content

  + Review Title

## Data Analysis Tasks and Answers

This involves the exploring of the given dataset to answer some questions about the DATA;

1. **What is the average discount by percentage by product category?**
    + Used pivot table and sumarised value as average and formated the final output to percentage. Visualised by Horizontal Barchart.

2. **How many products are listed under each category?**
    + Used pivot table and summarised value as distinct count. Visualised by Horizontal Barchart

3. **What is the total number of reviews per category?**
    + Used Pivot table: Sum of rating_count column by category. I also used Card to visualise it.

4. **Which products have the highest average ratings?**
    + Used pivot table: Values as rating summarised to Average. Sort output in a descending order and filtered to show top 10.

5. **What is the average actual price vs the discounted price by category?**
    + Used Pivot table: Summarised values as average. Visualised using clustered column chart.

6. **Which products have the highest number of reviews?**
    + Used Pivot table: summarised values to sum. Sort output in a descending order and filtered to show top 10.

7. **How many products have a discount of 50% or more?**
     + Used pivot table: Summarised value as count. Visualised using card/shape as KPI.

8. **What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?**
    + Used Pivot table: Product name in the value box, summarised as count. Visualised with a chart.

9. **What is the total potential revenue (actual_price × rating_count) by category?**
    + Used pivot table: Newly derived calculated column and the sum of values in the pivot row. Visualised with Card/shape.

10. **What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?**
    + Used pivot table: Another newly calculated column(price range bucket), with values set to distinct count. Visualised with Pie chart.

11. **How does the rating relate to the level of discount?**
    + Used pivot table: new column(discounts bucket), with values as rating, set to average. Visualised with clustered barchart.

12. **How many products have fewer than 1,000 reviews?**
    + Used pivot table: main category and summarised values as count. None of the product have more than a thousand reviews.

13. **Which categories have products with the highest discounts?**
    + Used pivot table: discount percentage as value and sorted in descending order.

14. **Identify the top 5 products in terms of rating and number of reviews combined.**
    + Used Pivot table: Rating count(same as number of reviews) plus the rating in values box in the pivot. Then sort to the top 5 using value filter. Visualised with Pivot table in the dashboard created.
   
## Analysed Dataset - [Amazon Analysed data](https://docs.google.com/spreadsheets/d/1O0VSJC_x-WFm7TXO4x77A2BRae0eptgqLyOp4yrIPIU/edit?gid=278939281#gid=278939281)

## Summary(Insights From Analysis)

1. **Average Discount Percentage By Product Category**
    + Computers & Accessories: ~53.2%
    + Electronics: ~49.9%
    + Car & Motorbike: ~42.0%
**Implication:** Computers & Accessories have the highest average discount. Promotions in this category may be driving more price-sensitive consumer traffic.

2. **Product Count by Category**
    + Electronics: 476 products
    + Computers & Accessories: 375 products
    + Car & Motorbike: 1 product
**Implication:** Electronics dominate in variety. Investing more in this category's optimization and bundling offers could enhance conversions.

3. **Total Reviews Per Category**
    + Electronics: 14.2 million+
    + Computers & Accessories: 6.3 million+
    + Car & Motorbike: ~1,118
**Implication:** High review volume indicates strong engagement in Electronics and Computers & Accessories. Consider highlighting social proof and review summaries on product pages

4. **Top-Rated Products Across Categories**
    + Every category listed has products with 5-star average ratings. ***Examples include:***
        + Electronics: Amazon Basics Wireless Mouse
        + Computers: REDTECH USB-C to Lightning Cable

**Implication:** These can be featured in marketing campaigns and recommended listings. Also study these products to replicate their success factors.

## Recommendations

#### 1. **Product Improvement**

  + Focus on improving underperforming items in Electronics through review mining and sentiment analysis.
  + Use customer reviews to identify recurring complaints or praise.

#### 2. **Marketing Strategy**

  + Run discount campaigns centered on high-conversion categories like Computers & Accessories.
  + Leverage top-rated products in ad creatives and influencer collaborations.
  + Highlight star reviews and usage scenarios to boost trust.

#### 3. **Customer Engagement**

  + Request more reviews on products with fewer ratings via post-purchase emails.
  + Develop personalized upsell offers based on review sentiment and categories browsed.
  + Consider loyalty points or referral programs for reviewers in high-engagement categories.
