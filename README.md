# Pizza Sales Analysis – SQL & Power BI Project

## Objective
To analyze the performance of a pizza business using SQL by extracting key insights on revenue, customer behavior, and product performance from historical sales data.

## Dataset
Pizza Sales-<a href="">Dataset</a>

## 📊 KPI Requirements
The following key performance indicators (KPIs) were identified to evaluate business performance:

- Total Revenue : Total income generated from all pizza sales.
- Average Order Value (AOV) : Revenue divided by the number of distinct orders.
- Total Pizzas Sold : Total quantity of pizzas sold over the period.
- Total Orders : The count of distinct orders placed.
- Average Pizzas per Order : Average number of pizzas included in a single order.

## 📈 Chart Requirements
The following visualizations are recommended to support insights:

- Daily Order Trend : Bar chart of total orders by day of the week.
- Monthly Order Trend : Line or bar chart showing how orders vary each month.
- Sales by Category : Pie chart or bar chart showing % sales contribution by pizza category.
- Sales by Size : Pie or bar chart showing % revenue by pizza size.
- Top/Bottom 5 Pizzas (Revenue, Quantity, Orders) : Horizontal bar charts for comparison.

## Process
- Data Source : Used the pizza_data table which includes columns like order_id, order_date, pizza_name, pizza_category, pizza_size, quantity, and total_price.

- SQL Queries:
  - Aggregate functions like SUM(), COUNT(), AVG() were used for KPIs.
  - TO_CHAR(order_date, 'Day/Month') used to extract time-based trends.
  - Subqueries and CAST() applied for percentage calculations.
  - Data grouped by pizza_name, pizza_category, and pizza_size for detailed analysis.

- Tools : Queries were executed in pgAdmin (PostgreSQL).

## Project Insights
- Fridays and weekends showed higher order volumes.
- February had noticeable pizza category trends (e.g., higher quantity sold in specific categories).
- Medium-sized pizzas dominated the sales by revenue.
- Classic and Supreme categories performed better than others.
- Top 5 pizzas generated significantly more revenue than the rest, showing a clear customer preference.
- Bottom 5 pizzas had very low orders, suggesting potential items to discontinue or revamp.

## Conclusion
This analysis provided valuable insights into which pizza types, sizes, and categories perform best, as well as customer ordering patterns by day and month. The business can use these insights to:

- Optimize the menu.
- Run promotions on underperforming items.
- Adjust inventory and staffing based on peak days.
