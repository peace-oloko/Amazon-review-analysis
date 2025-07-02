# Amazon-review-analysis
Exploratory data analysis of Amazon product reviews

## Overview
This case study involved analyzing product and customer review data from Amazon to extract actionable insights that can guide product improvement, marketing, and customer engagement strategies.

## Tools Used
- Microsoft Excel
  - Pivot Tables
  - Helper columns (e.g., Discount %, Price Bucket)
  - Filters and formulas
  - Charts (bar, scatter,)

## Key Insights
- About 3 categories share/offer the highest average discounts.
- The highest-rated products were identified based on both review count and star rating.
- Potential revenue calculations revealed that Electronics|Mobiles&Accessories|Smartphones&BasicMobiles|Smartphones has the strongest earning potential.
- A significant number of products have fewer than 1,000 reviews, showing opportunities for increased engagement.

## Deliverables
- Excel workbook containing:
  - Pivot table answers to all 14 analysis questions
  - Helper columns for Discount %, Price Bucket, and Potential Revenue
  - A combined score metric for rating × review strength
  - Visuals like rating distribution and discount vs rating scatter plot
- Summary dashboard showing key charts and slicers

## Notes
- Data cleaning included converting percentage values, price calculations, and rating formatting.
- All calculations were performed directly within Excel without external tools.

## Data Analysis

The analysis was conducted in Excel using helper columns, pivot tables, and formulas to extract insights from Amazon product review data.

### Helper Columns Created

#### Price Bucket 
  `=IF(actual price<200,"<₹200",IF(actual price<=500,"₹200–₹500",">₹500"))`

#### Potential Revenue 
  `=Actual Price * Rating Count`

#### Combined Score
-  = (Rating * 0.6) + (Rating Count / [Max Rating Count]) * 0.4


### Pivot Table Questions & Measures

#### Q1: Average Discount % by Category  
- Rows: Category  
- Values: Average of Discount %

#### Q2: Product Count by Category  
- Rows: Category  
- Values: Count of Product Name

#### Q3: Total Reviews per Category  
- Rows: Category  
- Values: Sum of Rating Count

#### Q4 & Q6: was achieved by sorting original table by Rating and Rating Count in descending order and top 5 was picked

#### Q5: Average Actual vs Discounted Price  
- Rows: Category  
- Values: Avg of Actual Price, Avg of Discounted Price

#### Q7: Products with Discount ≥ 50%  
- Filter Discount % column → `>=50`  

#### Q8: Rating Distribution  
- Pivot: Rows: Rating  
- Values: Count of Product Name

#### Q9: Total Potential Revenue by Category  
- Rows: Category  
- Values: Sum of Potential Revenue

#### Q10: Product Count per Price Bucket  
- Rows: Price Bucket  
- Values: Count of Product Name

#### Q11: Rating vs Discount  
- Scatter Chart was inserted  with X: Discount %, Y: Rating

#### Q12: Products with <1,000 Reviews  
- Filter Rating Count `< 1000`

#### Q13: Max Discount % by Category  
- Rows: Category  
- Values: Max of Discount %

#### Q14: Top 5 Products by Combined Score  
- Sorted Combined Score in descending order and picked top 5 rows




