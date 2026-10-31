1. Introduction to Power BI
Power BI is a Business Intelligence (BI) tool developed by Microsoft. It helps users transform raw data into meaningful insights through interactive reports and dashboards.

Main features:
Data visualization
Data cleaning and transformation
Data modelling
Interactive dashboards
Business reporting

2. Power BI Components
1. Power BI Desktop: Used to create reports and dashboards.
2. Power BI Service: Cloud platform to publish and share reports.
3. Power BI Mobile: Used to access reports on mobile devices.
4. Power BI Gateway: Connects on-premises data sources to Power BI Service.
5. Power BI Report Builder: Creates paginated reports.


3. Power BI Workflow
1. Connect to data sources.
2. Import data.
3. Clean and transform data using Power Query.
4. Create relationships between tables.
5. Create calculated columns and measures using DAX.
6. Build visualizations.
7. Design interactive reports.
8. Publish reports to Power BI Service.


4. Data Sources
Power BI supports different data sources:
Microsoft Excel
CSV files
SQL Server
MySQL
Web data
SharePoint
Azure databases

6. Power Query
Power Query is used for data cleaning and transformation before loading data into Power BI.

Important operations:
Remove duplicates
Remove null values
Change data types
Rename columns
Split columns
Merge columns
Replace values
Filter rows
Remove unnecessary columns

6. Data Modelling
Data modelling defines relationships between tables.
Types of relationships:
One-to-One (1:1)
One-to-Many (1:*)
Many-to-Many (:)
Important concepts:


Primary Key
Foreign Key
Fact Table
Dimension Table
Star Schema
Snowflake Schema
7. DAX (Data Analysis Expressions)


DAX is a formula language used in Power BI to perform calculations.


Important DAX functions:


Function| Purpose
SUM()| Adds values
AVERAGE()| Calculates average
COUNT()| Counts numeric values
COUNTROWS()| Counts table rows
DISTINCTCOUNT()| Counts unique values
CALCULATE()| Changes filter context
FILTER()| Filters a table
IF()| Conditional calculation
DIVIDE()| Safe division
RELATED()| Retrieves related values
SUMX()| Iterates and sums expressions
ALL()| Removes filters
SELECTEDVALUE()| Returns selected value


8. Important DAX Examples
Total Sales
Total Sales = SUM(Sales[Sales])
Total Profit
Total Profit = SUM(Sales[Profit])
Total Orders
Total Orders = DISTINCTCOUNT(Sales[Order ID])
Average Sales
Average Sales = AVERAGE(Sales[Sales])
Profit Margin
Profit Margin =
DIVIDE([Total Profit], [Total Sales], 0) * 100
Total Customers
Total Customers = DISTINCTCOUNT(Sales[Customer ID])
High Sales Category
Sales Status =
IF([Total Sales] > 10000, "High", "Low")


9. Calculated Columns vs Measures
Calculated Columns:
Calculated row by row.
Stored in the data model.
Useful for categories and classifications.

Measures:
Calculated dynamically.
Respond to filters and slicers.
Useful for KPIs and aggregations.

10. Power BI Visualizations
Important visual types:
1. Bar Chart
2. Column Chart
3. Line Chart
4. Pie Chart
5. Donut Chart
6. Area Chart
7. Scatter Chart
8. Table
9. Matrix
10. Card
11. KPI Visual
12. Map


11. Filters and Slicers
Filters:
Visual-level filters
Page-level filters
Report-level filters

Slicers:
Slicers allow users to interactively filter report data based on selected values such as region, date, and category.

12. Power BI Dashboard vs Report
Dashboard| Report
Single-page view| Can contain multiple pages
Created in Power BI Service| Created mainly in Desktop
Displays pinned visuals| Supports detailed analysis
Provides an overview| Allows deeper exploration


13. Important Power BI Concepts
Drill Down: Explore detailed levels of data.
Drill Through: Navigate to another report page with filtered context.
Tooltips: Display additional information when hovering over visuals.
Bookmarks: Save a particular report view.
Conditional Formatting: Highlight values based on conditions.
Row-Level Security (RLS): Restrict data access based on user roles.
Data Refresh: Update reports with the latest source data.

15. Power BI Keyboard Shortcuts
Ctrl + S: Save report.
Ctrl + Z: Undo.
Ctrl + Y: Redo.
Ctrl + C: Copy.
Ctrl + V: Paste.
Ctrl + A: Select all.

15. Common Interview Questions
1. What is Power BI?
Power BI is a Microsoft Business Intelligence tool used to analyse data and create interactive reports.

2. What is Power Query?
Power Query is used to clean, transform, and prepare data before loading it into Power BI.
3. What is DAX?
DAX is a formula language used to create calculations, measures, and calculated columns.

4. What is a slicer?
A slicer is an interactive visual that allows users to filter report data.

5. What is a relationship?
A relationship connects two tables using common columns.

6. What is a KPI?
A Key Performance Indicator measures progress towards a business objective.

7. What is a Star Schema?
A data modelling structure containing a central fact table connected to dimension tables.

8. What is the difference between a measure and a calculated column?
A calculated column is evaluated row by row and stored, whereas a measure is calculated dynamically based on the filter context.

16. Real-Time Project Ideas
1. Sales Performance Dashboard
2. HR Analytics Dashboard
3. E-commerce Sales Dashboard
4. Financial Performance Dashboard
5. Customer Retention Dashboard


Conclusion
Power BI is an important skill for Data Analysts. Understanding Power Query, DAX, data modelling, and visualization helps create meaningful business reports and support data-driven decision-making.
