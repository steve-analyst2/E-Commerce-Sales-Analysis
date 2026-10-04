# Business Findings

## Executive Summary

This analysis examined **5,000 e-commerce transaction records** to understand sales performance, product performance, geographic performance, and order delivery outcomes.

After data cleaning and validation, the analysis produced **KES 1,243,391.60 in Clean Total Sales** and **4,960 valid orders**.

Five business questions guided the analysis:

1. How has sales performance changed over time?
2. Which product categories generate the highest sales?
3. Which products are the top performers by sales?
4. Which countries generate the highest sales?
5. What is the distribution of orders by delivery status?

The analysis found that sales were highly concentrated among a small number of products, particularly within Electronics, while geographic sales were more widely distributed across countries.

Returned and Cancelled orders also represented a substantial share of valid orders, highlighting an area requiring further operational investigation.

---

# 1. How Has Sales Performance Changed Over Time?

## Analysis

Monthly sales were analyzed using `Clean Total Sales` grouped by Order Date across 2025 and 2026.

Total sales across the analyzed dataset amounted to **KES 1,243,391.60**, consisting of:

- **2025:** KES 798,049.35
- **2026:** KES 445,342.25

## Key Results

Sales fluctuated considerably from month to month rather than following a consistent upward or downward pattern.

The highest monthly sales value was recorded in **July 2026 at KES 82,459.55**.

Other strong months included:

- April 2025: KES 81,791.30
- June 2025: KES 81,475.25
- August 2025: KES 79,064.70
- January 2025: KES 78,207.90

Sales declined sharply after August 2026.

Only **KES 44.00** was recorded in September 2026, while October and November contained no recorded sales. December recorded only **KES 51.20**.

## Finding

Monthly sales performance was volatile, with repeated peaks and declines throughout the analysis period.

Although 2025 generated substantially more recorded sales than 2026, the sharp decline toward the end of 2026 appears to be associated with very limited or missing transaction data.

The annual totals should therefore not be treated as a direct like-for-like comparison of two complete years without first confirming the completeness of the late-2026 records.

## Business Interpretation

The monthly fluctuations indicate that sales were not evenly distributed throughout the period.

Understanding what drove stronger months could help determine whether the peaks were associated with particular products, product categories, countries, promotions, or other factors.

The late-2026 pattern also demonstrates the importance of checking data completeness before interpreting a decline as actual business deterioration.

## Recommendation

Investigate the factors associated with the strongest sales months and determine whether successful product, market, pricing, or promotional patterns can be replicated.

Before drawing conclusions about declining performance in late 2026 or comparing annual performance between 2025 and 2026, verify whether all transactions for the final months of 2026 were captured completely.

---

# 2. Which Product Categories Generate the Highest Sales?

## Analysis

Sales performance was compared across product categories using `Clean Total Sales`.

Total sales across all categories amounted to **KES 1,243,391.60**.

## Key Results

- **Electronics:** KES 798,709.75
- **Home Appliances:** KES 241,877.55
- **Fashion:** KES 112,582.35
- **Beauty:** KES 86,102.50
- **Unknown:** KES 4,119.45

Electronics generated approximately **64.2% of total sales**.

Home Appliances ranked second with approximately **19.5%**.

Together, Electronics and Home Appliances generated approximately **83.7% of total sales**.

## Finding

Sales were heavily concentrated in the **Electronics** category.

Electronics generated more than three times the sales value of Home Appliances and substantially more than Fashion and Beauty.

The category's dominance is particularly notable because transaction volumes across the four main product categories were relatively similar:

- Electronics: 1,245
- Fashion: 1,240
- Beauty: 1,239
- Home Appliances: 1,228

This indicates that Electronics' higher sales value was not simply caused by having substantially more transactions.

## Business Interpretation

The results suggest that higher-value Electronics products are important drivers of overall sales.

However, heavy dependence on one category also creates concentration risk. A significant change in demand, pricing, availability, or supply conditions affecting Electronics could materially affect overall sales.

## Recommendation

Prioritize inventory availability, pricing analysis, and promotional activity around strong-performing Electronics products.

At the same time, investigate opportunities to increase the sales contribution of lower-performing categories to create a more balanced product portfolio.

Transactions classified as `Unknown` should continue to be monitored and reduced through improved product-category data capture.

---

# 3. Which Products Are the Top Performers by Sales?

## Analysis

Individual products were ranked using `Clean Total Sales` to identify the five products generating the highest sales value.

## Key Results

The Top 5 products were:

1. **Laptop Pro 14: KES 463,852.50**
2. **Smartphone X12: KES 229,971.00**
3. **Microwave Oven: KES 72,684.00**
4. **Vacuum Cleaner: KES 59,247.00**
5. **Smart Watch: KES 51,204.00**

Together, these five products generated **KES 876,958.50**, representing approximately **70.5% of total sales**.

Laptop Pro 14 alone contributed approximately **37.3% of total sales**.

Smartphone X12 contributed approximately **18.5%**.

Combined, Laptop Pro 14 and Smartphone X12 generated **KES 693,823.50**, or approximately **55.8% of total sales**.

## Finding

Sales performance was highly concentrated among a small number of products.

**Laptop Pro 14 was the strongest-performing product by a substantial margin**, generating more than twice the sales of Smartphone X12.

The Top 5 products accounted for approximately 70.5% of total sales.

There is also a strong connection with the product-category analysis. Laptop Pro 14, Smartphone X12, and Smart Watch belong to Electronics, helping explain why Electronics dominated category sales.

## Business Interpretation

Overall sales performance is strongly dependent on a small number of high-value products, particularly Laptop Pro 14 and Smartphone X12.

These products represent important sales drivers, but this concentration creates potential risk if their demand, pricing, availability, or supply conditions change.

The results also demonstrate why category-level analysis should be supported by product-level analysis. The strong performance of Electronics is influenced substantially by a small number of leading products.

## Recommendation

Maintain adequate inventory availability for the strongest-performing products, particularly Laptop Pro 14 and Smartphone X12.

Investigate the factors driving their strong performance, including demand, pricing, customer preferences, and promotional activity.

Where appropriate, apply successful strategies to other products while developing additional strong-performing products to reduce dependence on a small number of sales drivers.

---

# 4. Which Countries Generate the Highest Sales?

## Analysis

Sales were compared across countries using `Clean Total Sales` to identify the geographic markets generating the highest sales value.

## Key Results

Sales by country were:

1. **Uganda: KES 178,995.00**
2. **South Africa: KES 142,285.20**
3. **United Kingdom: KES 135,738.10**
4. **India: KES 126,291.15**
5. **Ghana: KES 115,359.60**
6. **Rwanda: KES 112,379.10**
7. **Tanzania: KES 109,939.80**
8. **Kenya: KES 108,389.05**
9. **Nigeria: KES 105,366.85**
10. **United States: KES 105,352.15**
11. **Unknown: KES 3,295.60**

Uganda generated approximately **14.4% of total sales**.

The top three markets: Uganda, South Africa, and the United Kingdom, generated approximately **36.7% of total sales**.

## Finding

Uganda was the highest-performing country, generating **KES 178,995.00**.

However, unlike product performance, sales were relatively distributed across geographic markets.

No single country accounted for an overwhelming share of total sales, and most identified countries generated more than KES 100,000.

This suggests that sales were geographically more diversified than they were by product.

## Business Interpretation

The geographic distribution reduces dependence on a single market compared with the much stronger concentration observed among products and product categories.

Uganda represents the strongest market, but several other countries also make meaningful contributions to overall sales.

Understanding the characteristics of Uganda's performance could help identify opportunities that may be transferable to other markets.

## Recommendation

Investigate the factors contributing to Uganda's leading performance, including:

- Product mix
- Average order value
- Transaction volume
- Customer purchasing patterns

The business should also assess growth opportunities in other strong markets such as South Africa, the United Kingdom, and India rather than concentrating expansion efforts exclusively on Uganda.

Country information should continue to be validated to reduce transactions classified as `Unknown`.

---

# 5. What Is the Distribution of Orders by Delivery Status?

## Analysis

Valid orders were grouped by Delivery Status and counted using `Order ID`.

The analysis included **4,960 valid orders**.

## Key Results

The distribution was:

1. **Returned: 1,045 orders (21.1%)**
2. **Cancelled: 1,016 orders (20.5%)**
3. **Processing: 996 orders (20.1%)**
4. **Delivered: 968 orders (19.5%)**
5. **Shipped: 929 orders (18.7%)**
6. **Unknown: 6 orders (0.1%)**

Returned and Cancelled orders combined accounted for **2,061 orders**, or approximately **41.6% of valid orders**.

## Finding

Order volumes were relatively evenly distributed across the five main delivery statuses, with each representing approximately 19%–21% of valid orders.

However, **Returned was the largest individual status**, followed closely by Cancelled.

Together, Returned and Cancelled represented approximately **41.6% of valid orders**, identifying an important area for further operational investigation.

Only six orders were classified as `Unknown`, indicating that delivery-status information was available for almost all valid orders.

## Business Interpretation

The relatively high number of Returned and Cancelled orders could represent potential lost sales, additional handling costs, customer dissatisfaction, inventory disruption, or fulfillment inefficiencies.

However, the available dataset does not explain why individual orders were returned or cancelled.

The analysis therefore identifies an area requiring investigation but does not establish the underlying cause.

Processing and Shipped orders may also represent transactions that were still active when the dataset was captured and should not automatically be classified as unsuccessful orders.

## Recommendation

Investigate Returned and Cancelled orders using additional information such as:

- Return reason
- Cancellation reason
- Product
- Product category
- Customer location
- Payment method
- Shipping duration
- Fulfillment issues

Monitor return and cancellation rates over time and determine whether specific products, markets, or fulfillment patterns are associated with higher rates.

Future data collection should include standardized `Return Reason` and `Cancellation Reason` fields to support root-cause analysis.

---

# Overall Findings

The combined analysis produced several important observations.

## 1. Product Concentration Is High

Electronics generated approximately **64.2% of total sales**, while the Top 5 products generated approximately **70.5%**.

Laptop Pro 14 and Smartphone X12 alone contributed approximately **55.8% of total sales**.

This indicates substantial dependence on a relatively small number of high-value products.

## 2. Geographic Sales Are More Diversified

Uganda was the strongest country but generated only approximately **14.4% of total sales**.

The top three countries contributed approximately **36.7%**, indicating much lower geographic concentration than product concentration.

## 3. Transaction Volume Does Not Fully Explain Category Performance

Transaction volumes across Electronics, Fashion, Beauty, and Home Appliances were relatively similar.

However, Electronics generated substantially more sales.

This suggests that product value and product mix are major contributors to the category's performance.

## 4. Delivery Outcomes Require Further Investigation

Returned and Cancelled orders represented approximately **41.6% of valid orders**.

The dataset does not contain sufficient information to determine why these outcomes occurred, making this an important area for further data collection and operational analysis.

## 5. Data Completeness Affects Trend Interpretation

The apparent collapse in sales after August 2026 should not automatically be interpreted as a business-performance decline.

The extremely low or missing sales values in the final months indicate possible incomplete transaction coverage.

This limits direct full-year comparison between 2025 and 2026.

---

# Overall Recommendations

Based on the analysis:

1. **Protect the strongest sales drivers** by maintaining adequate availability of leading Electronics products, particularly Laptop Pro 14 and Smartphone X12.

2. **Reduce product concentration risk** by identifying opportunities to grow additional products and lower-performing categories.

3. **Investigate Uganda's strong performance** and determine whether successful product or customer patterns can be replicated in other markets.

4. **Investigate Returned and Cancelled orders** and introduce standardized reason fields to support root-cause analysis.

5. **Improve data completeness monitoring**, particularly for time-series reporting, so incomplete periods are identified before performance comparisons are made.

6. **Continue using validation rules** for critical analytical fields to prevent questionable values from silently influencing business metrics.

---

# Analysis Limitation

The findings are based on the information available in the dataset.

Some business outcomes particularly returns, cancellations, sales fluctuations, and differences between markets, cannot be fully explained because the dataset does not contain contextual variables such as promotional activity, inventory availability, product costs, return reasons, cancellation reasons, or detailed fulfillment information.

The findings should therefore be interpreted as evidence of patterns and areas requiring further investigation rather than proof of causation.
