# vinodrajput_2511895_part4_tableau_dashboard-Public
Executive Retail Performance Dashboard
Student Information
Name: Vinod Rajput
Student ID: 2511895
Repository: vinodrajput_2511895_part4_tableau_dashboard
Business Problem Summary
A retail leadership team requires an executive dashboard to monitor sales performance, profitability, customer behavior, category performance, shipping efficiency, discount impact, and return patterns. The objective is to identify business opportunities, operational risks, and support data-driven decision making through interactive visual analytics.

Dataset Description
The dataset contains retail sales transaction data including:

Order ID
Order Date
Customer Information
Customer Segment
Region and State
Product Category and Sub-Category
Sales
Profit
Discount
Shipping Mode
Delivery Days
Return Information
The dataset was connected to Tableau and validated before dashboard development.

Tableau Workbook Description
File: tableau/executive_dashboard.twbx

The Tableau workbook contains multiple analytical views and one executive dashboard designed for leadership reporting. Interactive filters and dashboard actions allow users to explore data across regions, categories, customer segments, shipping performance, and return trends.

Calculated Fields Created
1. Profit Margin
[Profit]/[Sales]
Purpose: Measures profitability generated per unit of sales.

2. Cost
[Sales]-[Profit]
Purpose: Estimates cost incurred for generating sales.

3. Average Order Value
[Sales]/COUNTD([Order Id])
Purpose: Measures average revenue generated per order.

4. Return Rate
SUM([Return Flag])/COUNTD([Order Id])
Purpose: Measures percentage of returned orders.

5. Shipping Delay Bucket
IF [Delivery Days] <= 3 THEN "Fast Delivery"
ELSEIF [Delivery Days] <= 7 THEN "Normal Delivery"
ELSE "Delayed"
END


Purpose:
Categorizes delivery performance.



# Dashboard Components

The dashboard contains the following views:

1. Sales Trend View
2. Regional Performance View
3. Category Profitability View
4. Customer Segment View
5. Shipping Performance View
6. Discount vs Profit View
7. Return Analysis View

### KPI Cards

- Total Sales
- Total Profit
- Total Orders



# Filters and Interactions Used

### Dashboard Filters

- Region
- Category
- Customer Segment

### Dashboard Actions

A filter action was created on the Regional Performance View.

When a region is selected, all related dashboard views update automatically to display filtered results.


# Key Business Insights

1. Sales performance varies across regions, indicating different market strengths.
2. Certain product categories generate significantly higher profits than others.
3. Customer segments contribute differently to overall sales performance.
4. High discount levels are associated with reduced profitability.
5. Shipping performance impacts customer experience and operational efficiency.
6. Return rates vary across customer segments and product categories.
7. Some sub-categories contribute strongly to revenue generation.
8. Regional analysis helps identify expansion opportunities and performance gaps.



# Dashboard Story Summary

The dashboard provides a consolidated view of retail business performance. Leadership can identify high-performing regions, profitable categories, customer purchasing patterns, discount impacts, shipping efficiency, and return behavior. Interactive filters support deeper analysis and facilitate data-driven decision-making.



# Assumptions

- Dataset values are assumed to be accurate and complete.
- Profit Margin calculation uses Sales and Profit fields provided.
- Return Rate is calculated using available return indicators.
- Delivery performance is categorized using delivery days.



# Limitations

- Dashboard analysis depends entirely on available dataset fields.
- External market conditions are not represented.
- Customer satisfaction and qualitative factors are not included.
- Forecasting and predictive analytics are outside the scope of this dashboard.



# Screenshots Included

- full_dashboard.png
- sales_trend_view.png
- regional_performance_view.png
- category_profitability_view.png
- filter_interaction_view.png



# Conclusion

The Executive Retail Performance Dashboard successfully provides leadership with a centralized view of sales, profitability, customer behavior, category performance, shipping efficiency, discount impact, and return trends. Interactive filters and dashboard actions enhance exploration and support informed business decisions.
