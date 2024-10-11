# SQL E-commerce case study : Query writing

🎯 Objective

Analyzing the sales, product, and customer data for an e-commerce company. getting various insights and calculating various KPI and data with SQL in Big Query.
This project aims to leverage the power of e-commerce data (sales, product, and demographic) analyzed through SQL to unlock actionable insights driving profitable growth. By delving into 
customer behavior, product trends, and sales patterns, we will uncover hidden value that can inform key business decisions. You need to find these patterns and calculate various metrics and 
KPIs that suit the data and the goal.


## Dataset

Demographic table:

| **Variable**          | **Description**                                                            |
|-----------------------|----------------------------------------------------------------------------|
| **HOUSEHOLD_KEY**      | Uniquely identifies each household                                          |
| **AGE_DESC**           | Estimated age range                                                        |
| **MARITAL_STATUS_CODE**| Marital Status (A - Married, B - Single, U - Unknown)                      |
| **INCOME_DESC**        | Household income                                                           |
| **HOMEOWNER_DESC**     | Homeowner, renter, etc.                                                    |
| **HH_COMP_DESC**       | Household composition                                                      |
| **HOUSEHOLD_SIZE_DESC**| Size of household up to 5+                                                 |
| **KID_CATEGORY_DESC**  | Number of children present up to 3+                                        |

Transaction table:

| **Variable**           | **Description**                                                         |
|------------------------|-------------------------------------------------------------------------|
| **HOUSEHOLD_KEY**       | Uniquely identifies each household                                       |
| **BASKET_ID**           | Uniquely identifies a purchase occasion                                  |
| **DAY**                 | Day when transaction occurred                                            |
| **PRODUCT_ID**          | Uniquely identifies each product                                         |
| **QUANTITY**            | Number of products purchased during the trip                             |
| **SALES_VALUE**         | Amount of dollars retailer receives from sale                            |
| **STORE_ID**            | Identifies unique stores                                                 |
| **COUPON_MATCH_DISC**   | Discount applied due to retailer's match of manufacturer coupon           |
| **COUPON_DISC**         | Discount applied due to manufacturer coupon                              |
| **RETAIL_DISC**         | Discount applied due to retailer's loyalty card program                   |
| **TRANS_TIME**          | Time of day when the transaction occurred                                |
| **WEEK_NO**             | Week of the transaction. Ranges from 1 to 102                            |


Products Table:

| **Variable**              | **Description**                                                          |
|---------------------------|--------------------------------------------------------------------------|
| **PRODUCT_ID**            | Number that uniquely identifies each product                             |
| **DEPARTMENT**            | Groups similar products together                                          |
| **COMMODITY_DESC**        | Groups similar products together at a lower level                        |
| **SUB_COMMODITY_DESC**    | Groups similar products together at the lowest level                      |
| **MANUFACTURER**          | Code that links products with the same manufacturer together              |
| **BRAND**                 | Indicates Private or National label brand                                 |
| **CURR_SIZE_OF_PRODUCT**   | Indicates package size (not available for all products)                   |

    
# Business Recommendations/Insights

- **Discount Strategies for High-Value Customers**: Since households making larger purchases benefit more from discounts, customize promotions to encourage frequent purchases among these high-value customers. Targeted offers can further boost sales within this group.

- **Stocking Popular Products**: Products like 'Fluid milk white,' soft drinks, bananas, and shredded cheese have high purchase rates. Ensure these items are well-stocked and prominently displayed, alongside other fast-moving groceries. Consider bundling these popular items with less frequently purchased products to increase overall sales. Expand the variety of high-demand level-2 commodities to capture a larger market share.

- **Personalized Marketing Based on Household Size & Income**: Tailor marketing efforts based on household size and income. High-income households with smaller family sizes tend to have a higher Average Order Value (AOV), so premium and personalized product recommendations could be highly effective. Implement loyalty programs or exclusive offers to retain these high-value customers.

- **Optimizing Promotions for Peak Hours**: Since top-selling items are primarily purchased in the afternoon and evening, schedule promotions and stock replenishments accordingly. Consider extending store hours or increasing staff during peak times to better serve customers and capture additional sales.

- **Retention Strategies for High-Income Groups**: High-income households often have a high AOV but low purchase frequency, indicating a need to convert these premium, one-time buyers into repeat customers. Implement loyalty programs or subscription models to increase retention. Additionally, consider value-based offers or psychological pricing to increase AOV for lower-income households, which tend to make smaller but more frequent purchases.

- **Improve Underperforming Departments**: Analyze sales patterns and customer preferences within underperforming departments to identify areas for improvement. Use targeted marketing and promotions to enhance their performance. Simultaneously, continue to invest in top-performing departments, such as grocery and Drug GM, to maintain and grow their success.
