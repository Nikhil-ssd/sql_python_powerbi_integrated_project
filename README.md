# sql_python_powerbi_integrated_project
An integrated sales &amp; revenue analysis project utilizing MySQL, Python &amp; Power BI.

Problem Statement :

1) Import data into MySQL database. 
2) Perform data cleaning and transformation using Python. 
3) Create a Power BI dashboard to visualize key insights. 

Load the datasets and clean them by using python: 
-  Clean and perform necessary operations on data.
-  Create a new column in the sales data to calculate total_sale_amount (quantity sold × price). 

Insert the cleaned data into mysql database/ Excel file. 

Power BI (Dashboard) 
Import the cleaned dataset into Power BI from mysql database/ Excel file. 
Create a dashboard that includes the following visuals: -  A bar chart showing revenue by product category. -  A map displaying revenue by region. -  A line chart showing monthly revenue trends for 2023. -  A table listing the top 5 products by revenue. - Include additional insights based on business requirements. 
Ensure the dashboard is interactive and user-friendly, with proper filters and labels.

Dataset Information

By using a SQL Script, data is stored in database named jforce by inserting it into three tables namely Customers, Sales and Products.

A) The Customers table contains 300 rows and 6 columns namely 1) customer_id 2) customer_name 3) gender 4) age 5) city 6) join_date

B) The Sales table contains 300 rows and 7 columns namely 1) sale_id 2) product_id 3) customer_id 4) quantity_sold 5) sale_amount 6) sale_date 7) region

C) The Products table contains 18 rows and 4 columns namely 1) product_id 2) product_name 3) category 4) price

# Steps followed to solve this problem
1) Created a database named "jforce" in MySQL
2) Created 3 tables named Customers, Sales, Products and inserted data into these tables by running a SQL Script.
3) Created a Python Jupyter notebook file, established connection with MySQL using MySQL-python connector.
4) Feteched data from the database tables using the cursor object and stored the data in their respective dataframes.
5) Closed the connection established
6) Performed data-cleaning, pre-processing and feature engineering using Python's pandas library
7) Exported the datasets to excel files.
8) Imported the cleaned and processed data sets in Power BI.
9) Performed additonal data-cleaning, processing and modelling.
10) Built various suitable and relevant visuals according to the problem statement.

# What does the Power BI Report contain
The Power BI Report contains 2 tabs namely 1) Revenue Dashboard and 2) Sales Dashboard

The Structure of the Revenue and Sales Dashboard is the same with both containing 6 visuals, 7 slicers and a title box.

The Revenue Dashboard shows
1) Total Revenue by Category Stacked Bar-chart
2) Total Revenue by Month Line-chart
3) Total Revenue by Region Map-chart
4) Total Revenue by Gender Bar-chart
5) Total Revenue by Age-group Histogram
6) Top 7 customers by revenue table
7) Top 7 products by revenue table

Similarly, 

The Sales Dashboard shows
1) Total Sales by Category Stacked Bar-chart
2) Total Sales by Month Line-chart
3) Total Sales by Region Map-chart
4) Total Sales by Gender Bar-chart
5) Total Sales by Age-group Histogram
6) Top 7 customers by Sales table
7) Top 7 products by Sales table

Data in both these tabs can be sliced and diced by 7 Slicers namely Product Name, City, Sales Date, Category, Price Range, Gender and Region to analyze data as required to gather valuable insights to make informed business decisions.

Step 1 : Download this project repository as a zip file. 
Step 2 : Unzip the folder to your desired location 
Step 3 : If you don't have MySQL & MySQL Workbench Installed, go to https://dev.mysql.com/downloads/ and download the MySQL installer along with the MySQL Workbench for your operating system (Windows, macOS, or Linux) & launch it. 
Step 4 : Establish a connection with the MySQL Server on your local instance. 
Step 5 : Create a database with a suitable name on MySQL.
Step 6 : Open the script named "sample_data_all_quoted.sql" and run it to insert data into their respective tables.
Step 7 : Check if the 3 tables were created and data was inserted into them. 
Step 8 : If you don't have Anaconda installed, go to the Anaconda website and download the installer for your operating system (Windows, macOS, or Linux) and launch it. 
Step 9 : Launch Jupyter Notebook Interface from Anaconda Navigator after which opens in your default browser. 
Step 10 : Navigate to this project folder. 
Step 11 : When inside navigate to JForce > Updated Sloution.ipynb 
Step 12 : Open and Run the Updated Sloution.ipynb file cell by cell while analyzing the ouput.
Step 13 : Check the output excel files generated.
Step 14: If you don't have Microsoft Power BI Desktop Installed , go to https://www.microsoft.com/en-in/download/details.aspx?id=58494&msockid=39cd1c66ce6867ae13a2094ecfc066fd, download the suitable installer, install Microsoft Power BI Desktop and launch it. 
Step 15 : Navigate to the Sales & Revenue Dashboard.pbix file in the project folder.
Step 16 : Open the Sales & Revenue Dashboard.pbix using Microsoft Power BI Desktop. 
Step 17 : Go through the Power BI tasks mentioned above and compare the visuals in the Power BI File accordingly.

Why Use Power BI?
Power BI is ideal for analyzing HR data because of its:

Interactive Dashboards: Create dynamic dashboards for real-time monitoring of sales performance. Data Integration: Combine data from CRM systems, ERP platforms, and third-party sources for comprehensive analysis. Advanced Analytics: Leverage built-in AI features to uncover hidden patterns or anomalies. User-Friendly Interface: Enable non-technical users, such as sales teams, to explore data independently. Custom Reporting: Generate role-specific reports for stakeholders like sales managers, regional heads, or marketing teams.

Purpose of Solving this problem
Analyzing the sales data of a store like Superstore using Python & Power BI can provide valuable insights for decision-making across various operational, marketing, and strategic areas. Power BI's powerful visualization capabilities make it easier to identify trends, patterns, and actionable insights. Here's a breakdown of the key purposes:

1. Monitor and Improve Sales Performance
Revenue Trends: Track total sales, profit margins, and revenue growth over time. Category Insights: Identify top-performing product categories and subcategories. Seasonal Analysis: Discover seasonality patterns and high-demand periods. Regional Performance: Analyze sales performance by region, state, or city to identify strong and weak markets.

2. Understand Customer Behavior
Purchase Patterns: Identify which products are purchased frequently or together. Customer Segmentation: Group customers by buying habits, spending levels, or location. Loyalty Analysis: Determine the lifetime value of customers and their retention patterns.

3. Optimize Inventory Management
Stock Levels: Highlight overstocked or understocked items. Turnover Rates: Understand how quickly products are sold. Demand Forecasting: Use historical sales data to predict future demand and optimize inventory.

4. Identify Profitability Drivers
Profit Margins: Pinpoint which products, categories, or regions yield the highest profits. Cost vs. Revenue: Compare operational costs with revenue generation. Discount Analysis: Assess the impact of discounts on sales and profitability.

5. Evaluate Marketing Effectiveness
Campaign Impact: Measure how promotions and campaigns affect sales. Product Popularity: Identify which promotions drive the most traffic and conversions. Cross-Selling Opportunities: Analyze product combinations to target upselling or bundling strategies.

6. Enhance Operational Efficiency
Shipping and Delivery: Examine delivery times and costs to optimize logistics. Order Patterns: Identify peak order times to allocate resources effectively. Returns Analysis: Understand reasons for product returns to reduce future occurrences.

7. Drive Strategic Decision-Making
Market Expansion: Use regional sales data to identify opportunities for opening new stores. Pricing Strategies: Evaluate pricing trends to remain competitive. Customer Demographics: Target specific segments more effectively based on their preferences and buying behaviors.

8. Detect Anomalies and Address Issues
Low Performance Areas: Quickly identify products or regions with declining sales. Fraud Detection: Spot unusual patterns that could indicate fraud or errors. Customer Complaints: Analyze feedback data tied to sales trends.
