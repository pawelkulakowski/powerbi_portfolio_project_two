# Portfolio Project Microsoft PowerBi  

The goal was to create a project with a use of parameters year and month to show the general sales situation in each of choosen month/year.

The project is still in the development phase. Many of measueres were used only for testing and some of tabs (despite the ones which are below described) are still being in the process of developing.

View Sales

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_01.JPG?raw=true)

View Quantity

![alt text](https://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_02.JPG?raw=true)

View Transactions

![alt text](ttps://github.com/pawelkulakowski/powerbi_portfolio_project_two/blob/master/project_03.JPG?raw=true)

## General Layout
- using new slicer with reference labels and details
- creating summarized tables for years and months to use them as parametres in the project
- using bookmark navigator to show different selection of graphs depending on user interaction
- using custom color pallette
- using custom labels based on the month/year selection

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