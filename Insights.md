# E-Commerce Exploratory Data Analysis - Business Insights

## Project Overview

This document summarizes the findings obtained from Exploratory Data Analysis performed on the cleaned e-commerce order dataset.

The analysis focuses on:

- Sales performance
- Product contribution
- Customer behaviour
- Order performance
- Discount impact
- Revenue drivers

Dataset Size:

- Records: 1200 orders
- Columns: 16
- Primary Key: OrderID


---

# 1. Dataset Quality Insights

## Data Validation

Checks performed:

- Missing value analysis
- Duplicate OrderID check
- Data type validation


Findings:

- No duplicate OrderID records were found.
- Missing values were handled during preprocessing.
- CouponCode missing values were converted into "None".
- Dataset was ready for analysis.


---

# 2. Overall Sales Performance

## Average Order Value (AOV)

Average order value:

₹1053.97


Interpretation:

The average customer transaction value is approximately ₹1054.

This metric can be used as a baseline for improving customer spending.


---

# 3. Product Performance Analysis


## Quantity Sold by Product

Product-wise quantity sold:

|Product|Units Sold|
|-|-:|
|Chair|562|
|Printer|542|
|Laptop|535|
|Desk|508|
|Tablet|497|
|Monitor|480|
|Phone|411|


Insights:

- Chair generated the highest sales volume.
- Phone had the lowest quantity sold among products.


Business Action:

High-volume products should maintain sufficient inventory availability.


---

# 4. Revenue Contribution by Product


Revenue generated:

|Product|Revenue|
|-|-:|
|Chair|₹195,620|
|Printer|₹195,613|
|Laptop|₹192,127|
|Tablet|₹186,569|
|Monitor|₹175,651|
|Desk|₹167,460|
|Phone|₹151,722|


Insights:

- Chair and Printer are the highest revenue-generating products.
- Revenue distribution is relatively balanced across products.

Business Action:

Focus promotional strategies on high-revenue products.


---

# 5. Category Analysis


Category Revenue:

|Category|Revenue|Contribution|
|-|-:|-:|
|Electronics|₹901,682|71.29%|
|Furniture|₹363,080|28.71%|


Insights:

- Electronics contributes around 71% of total revenue.
- Furniture contributes around 29%.


Business Action:

Electronics inventory and marketing should receive higher priority.


---

# 6. Time Trend Analysis


Analysis performed:

- Yearly revenue trend
- Monthly revenue trend


Findings:

- Revenue fluctuates across months.
- Monthly trend analysis helps identify periods of higher sales activity.


Business Action:

Use historical patterns for:

- Inventory planning
- Seasonal campaigns
- Resource allocation


---

# 7. Payment Behaviour Analysis


Payment distribution:

|Payment Method|Orders|
|-|-:|
|Online|258|
|Cash|246|
|Credit Card|234|
|Debit Card|232|
|Gift Card|230|


Revenue contribution:

|Payment Method|Revenue Share|
|-|-:|
|Credit Card|20.86%|
|Online|20.75%|
|Cash|20.54%|
|Gift Card|19.48%|
|Debit Card|18.37%|


Insights:

- Payment preference is evenly distributed.
- Credit Card generated the highest revenue contribution.


Business Action:

Maintain support for all payment methods.


---

# 8. Discount Analysis


Discount usage:

Discount Applied Orders:

891

No Discount Orders:

309


Revenue:

|Type|Revenue|AOV|
|-|-:|-:|
|Discount Applied|₹942,361|₹1057.64|
|No Discount|₹322,401|₹1043.37|


Insights:

- Discounted orders generated significantly higher total revenue.
- Average order value is slightly higher for discounted orders.


Business Action:

Discount campaigns should be optimized based on revenue impact.


---

# 9. Order Status Analysis


Order distribution:

|Status|Orders|
|-|-:|
|Cancelled|250|
|Returned|247|
|Pending|237|
|Shipped|235|
|Delivered|231|


Order Outcome:

Successful Orders:

58.58%

Unsuccessful Orders:

41.42%


Insights:

A significant percentage of orders do not successfully complete.


Business Action:

Investigate reasons behind:

- Cancellations
- Returns
- Pending orders


---

# 10. Customer Analysis


Customer level metrics calculated:

- Total Orders
- Revenue Generated
- Average Order Value


Insights:

- Customer revenue contribution is not evenly distributed.
- Some customers generate higher revenue with fewer but larger purchases.


Business Action:

Create customer segments using:

- Spending behaviour
- Purchase frequency
- Recency


---

# 11. Referral Source Analysis


Customer acquisition sources:

|Source|Contribution|
|-|-:|
|Instagram|21.58%|
|Email|20.83%|
|Google|20.08%|
|Facebook|19.00%|
|Referral|18.50%|


Insights:

- Instagram is the highest contributing referral channel.
- Marketing channels have relatively similar performance.


Business Action:

Continue investing across multiple channels.


---

# 12. Outlier Analysis


Outliers detected using IQR method.


Findings:

High-value transactions were identified.

Top outlier products:

- Printer
- Laptop
- Tablet
- Chair
- Monitor


Interpretation:

These transactions represent:

- Premium customers
- High-value orders


Business Action:

Investigate before removing because they represent valuable customers.


---

# 13. Correlation Analysis


Variables analyzed:

- Quantity
- UnitPrice
- ItemsInCart
- TotalPrice


Key findings:

- UnitPrice has the strongest relationship with TotalPrice (0.72),
  indicating premium products contribute significantly to revenue.

- Quantity has a moderate positive relationship with revenue (0.62),
  showing larger purchases generally increase order value.

- ItemsInCart has a weaker relationship with revenue (0.39),
  suggesting cart size alone is not a strong revenue predictor.

- Quantity and UnitPrice are almost independent (0.015),
  meaning expensive products are not necessarily purchased in larger quantities.


Business Meaning:

Revenue increases mainly due to:

- Higher priced products
- Larger purchase quantities


---

# Final Business Recommendations


1. Prioritize high revenue products like Chair, Printer and Laptop.

2. Focus inventory management on Electronics category.

3. Improve order completion rate by reducing cancellations and returns.

4. Optimize discount strategies using revenue impact.

5. Develop customer segmentation for retention campaigns.

6. Monitor high-value transactions for VIP customer identification.


---

# Conclusion

EDA transformed raw transactional data into meaningful business insights.

The analysis provides a foundation for:

- SQL business queries
- Power BI dashboard creation
- Customer segmentation
- Advanced analytics

