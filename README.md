Excited to share my third internship task where I worked with SQLite to analyze e-commerce data! Here's a quick overview of what I accomplished:

🔹 Average Items per Order: Calculated the average number of items in each order (1.14 items/order)
🔹 Customer Order Analysis: Identified top customers by order volume and their locations (mostly São Paulo)
🔹 Payment Insights: Analyzed payment types and values, filtering orders above average payment value
🔹 Geographic Trends: Discovered order distribution by state (SP leads with 41,746 orders)

This task helped me strengthen my SQL skills in:
✅ Writing complex queries with JOINs and subqueries
✅ Using aggregate functions (COUNT, AVG)
✅ Analyzing real-world e-commerce datasets

Special thanks to elevate labs for this valuable learning opportunity!

 Order Item Analysis
- Calculated average items per order (1.14)
```sql
SELECT AVG(item_count) AS avg_items
FROM (
    SELECT order_id, COUNT(*) AS item_count 
    FROM order_item 
    GROUP BY order_id
)
2. Customer Insights
Identified top customers by order volume

Geographic distribution of orders (SP state dominates with 41,746 orders)

3. Payment Analysis
Filtered orders with above-average payment values

Examined payment type distribution

Skills Demonstrated
SQL query writing
Data aggregation
JOIN operations
Subqueries
Data interpretation
Tools Used
DB Browser for SQLite
SQLite database
Results
The analysis revealed:
Most customers are concentrated in São Paulo (SP)

Average order contains 1-2 items


