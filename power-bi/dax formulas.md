1. What is DAX?
DAX (Data Analysis Expressions) is a formula language used in Power BI to perform calculations and analyse data.

2. Basic Aggregation Functions
SUM – Calculates total
Total Sales = SUM(Sales[Sales])
AVERAGE – Calculates average
Average Sales = AVERAGE(Sales[Sales])
MIN – Finds minimum value
Minimum Sales = MIN(Sales[Sales])
MAX – Finds maximum value
Maximum Sales = MAX(Sales[Sales])
COUNT – Counts numeric values
Total Count = COUNT(Sales[Sales])
COUNTROWS – Counts table rows
Total Records = COUNTROWS(Sales)
DISTINCTCOUNT – Counts unique values
Unique Customers = DISTINCTCOUNT(Sales[Customer ID])

3. Logical Functions
IF
Sales Status =
IF([Total Sales] > 10000, "High", "Low")
AND
Sales Check =
IF(
    AND([Total Sales] > 10000, [Total Profit] > 1000),
    "Good",
    "Needs Improvement"
)
OR
Performance =
IF(
    OR([Total Sales] > 10000, [Total Profit] > 1000),
    "Achieved",
    "Not Achieved"
)
SWITCH
Sales Category =
SWITCH(
    TRUE(),
    [Total Sales] > 20000, "High",
    [Total Sales] > 10000, "Medium",
    "Low"
)


4. Filter Functions
CALCULATE
West Sales =
CALCULATE(
    [Total Sales],
    Sales[Region] = "West"
)
FILTER
High Value Sales =
CALCULATE(
    [Total Sales],
    FILTER(Sales, Sales[Sales] > 1000)
)
ALL
All Region Sales =
CALCULATE(
    [Total Sales],
    ALL(Sales[Region])
)


5. Mathematical Functions
DIVIDE
Profit Margin =
DIVIDE([Total Profit], [Total Sales], 0) * 100
ROUND
Rounded Sales =
ROUND([Total Sales], 2)
ABS
Absolute Profit =
ABS([Total Profit])


6. Text Functions
UPPER
Upper Name = UPPER(Sales[Product])
LOWER
Lower Name = LOWER(Sales[Product])
CONCATENATE
Product Name =
CONCATENATE(Sales[Category], Sales[Product])

7. Time Intelligence Functions
Assuming you have a properly configured and marked Date table:
TOTALYTD
YTD Sales =
TOTALYTD([Total Sales], 'Date'[Date])
SAMEPERIODLASTYEAR
Last Year Sales =
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR('Date'[Date])
)
DATEADD
Previous Month Sales =
CALCULATE(
    [Total Sales],
    DATEADD('Date'[Date], -1, MONTH)
)


8. Iterator Functions
SUMX
Total Revenue =
SUMX(Sales, Sales[Quantity] * Sales[Unit Price])
AVERAGEX
Average Revenue =
AVERAGEX(Sales, Sales[Sales])


9. Important DAX Concepts
Row Context: Evaluates calculations for each individual row.
Filter Context: Determines which data is included in a calculation.
Measure: A dynamic calculation based on the current filter context.
Calculated Column: A column calculated row by row and stored in the model.
Context Transition: Converts row context into filter context, commonly through CALCULATE.

11. Practical Business KPIs
Total Sales = SUM(Sales[Sales])
Total Profit = SUM(Sales[Profit])
Total Quantity = SUM(Sales[Quantity])
Total Customers = DISTINCTCOUNT(Sales[Customer ID])
Total Orders = DISTINCTCOUNT(Sales[Order ID])
Profit Margin =
DIVIDE([Total Profit], [Total Sales], 0) * 100
Average Order Value =
DIVIDE([Total Sales], [Total Orders], 0)


11. Practice Questions
1. Calculate total sales.
2. Calculate total profit.
3. Find the average sales value.
4. Count unique customers.
5. Calculate profit margin.
6. Find sales for the West region.
7. Classify sales as High, Medium, or Low.
8. Calculate year-to-date sales.
9. Find previous year's sales.
10. Calculate average order value.
12. Important Interview Questions
Q1. What is CALCULATE?
CALCULATE evaluates an expression after modifying its filter context.
Q2. What is the difference between SUM and SUMX?
SUM adds values from a column. SUMX evaluates an expression row by row and then adds the results.
Q3. What is DISTINCTCOUNT?
It counts unique values in a column.
Q4. What is filter context?
It is the set of filters applied to a calculation.
Q5. Why is DIVIDE preferred over the division operator?
DIVIDE handles division by zero safely when an alternate result is provided.
Conclusion: DAX helps Data Analysts calculate business KPIs, compare performance, and create dynamic reports.
