# Portfolio Project Microsoft PowerBi  - Driving Sales Growth with Performance KPIs: The Power of a Sales Dashboard

In a competitive market, increasing sales requires more than just a skilled team—it demands precise, data-driven management. One of the most effective ways to boost sales performance is by equipping your sales team with a comprehensive dashboard that tracks key performance indicators (KPIs). By focusing on metrics like monthly incoming orders, growth rates, trends across quantity, sales volume, number of transactions, customer count, and profit margin, you can transform raw data into actionable insights.

A sales dashboard serves as a central hub for monitoring and analyzing these KPIs, providing a clear picture of your sales team's performance. By tracking monthly incoming orders and growth rates, you can quickly identify patterns and assess whether your strategies are driving the desired results. Trends in sales quantity and volume reveal shifts in customer behavior, helping you adapt to market changes. Monitoring the number of transactions and customers allows you to gauge engagement levels, while margin analysis ensures that growth is not just in sales but in profitability as well.

Implementing such a dashboard enables your sales team to focus on what matters most—meeting and exceeding targets. With real-time data at their fingertips, they can make informed decisions, prioritize high-impact activities, and respond swiftly to opportunities and challenges.

In conclusion, a sales performance dashboard is not just a tool; it's a strategic asset that can significantly enhance your team's effectiveness. By bringing key KPIs into focus, you'll empower your sales team to drive sustained growth, improve customer relationships, and maximize profitability.

View Sales

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_01.JPG?raw=true)

View Quantity

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_02.JPG?raw=true)

View Transactions

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_03.JPG?raw=true)

View Customers

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_04.JPG?raw=true)

View Margin

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_05.JPG?raw=true)

## General Layout
- using new slicer with reference labels and details
- creating summarized tables for years and months to use them as parametres in the project
- using bookmark navigator to show different selection of graphs depending on user interaction
- using custom color pallette
- using custom labels based on the month/year selection
- creating relationship between slicers years/months to change the number of displayed months depends on the year (dataset is up to april 2019)

## KPI's
The goal was to show KPI's for choosen current month/year
- calculating current month and previous months performance indicators
- calculating Month-Over-Month changes
- calculating Year-Over-Year changes
- calculating Delta to Budget 
- using FORMAT() function to differ positive and negative indicators
- using custom arrows to visually show the positive/negative changes
- using conditional formating based on the value


## Sales Tab
The goal was to show the data for choosen current year and all previous months in current year
- using RANK() function to rank sales based on the category in the choosen month
- using TREATAS() function to make the relationship between the budget dimension table and calendar table
- using titles and subtitles to help understanding the scope of graphs

## Quantity Tab
The goal was to show all the data up to choosen current year and month
- using bookmarks to change between total and cummulative graph
- using line graph with analytics tool to show average 
- using matrix with RANK() function and PARETO calculations on different levels - product category and product

## Transactions Tab
The goal was to show the monthly tranctions for choosen current year and all previous months in current year in relation to averages
- creating a unique order id by combining the date of transaction, store id, customer id, transaction id in PowerQuery using concatenation and Text functions including PadStart to have constant number of digits in each order id
- creating a horizontal bar chart with custom label placeholder and additional detail together with error bars
- creating additional kpi's for transactions

## Customers Tab
The goal was to show monthly proporition of customers among the shops
- creating a horizontal bar chart to show number and percentage of customers among 3 shops
- creating custom cards using new cards
- creating three seperate measueres with KEEPFILTERS() in the CALCULATE() function

## Margin
The goal was to show monthly profit margin with highliting products with negative margins
- updating the product lookup table with PANDAS (multiply cost by several factors to create more interesting graphs)
- creating a horizontal bar chart to show with dummy data to enable two rows of labelling
- creating a filter on the matrix to show only the products which have negative margin
