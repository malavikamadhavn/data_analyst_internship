Excel Formulas – Data Analyst Notes
1. SUM()
Purpose: Adds numbers in a selected range.
Syntax:
=SUM(A2:A10)
Example: Calculates total sales.

2. AVERAGE()
Purpose: Calculates the average of numbers.
=AVERAGE(B2:B10)

3. MIN() and MAX()
Purpose: Finds the smallest and largest values.
=MIN(B2:B10)
=MAX(B2:B10)

4. IF()
Purpose: Checks a condition and returns one result if TRUE and another if FALSE.
=IF(C2>=50,"Pass","Fail")

5. SUMIF()
Purpose: Adds values that meet one condition.
=SUMIF(A2:A10,"South",B2:B10)

6. SUMIFS()
Purpose: Adds values based on multiple conditions.
=SUMIFS(C2:C10,A2:A10,"South",B2:B10,"Laptop")

7. COUNTIF()
Purpose: Counts cells that meet one condition.
=COUNTIF(A2:A10,"Completed")

8. COUNTIFS()
Purpose: Counts cells based on multiple conditions.
=COUNTIFS(A2:A10,"South",B2:B10,"Completed")

9. VLOOKUP()
Purpose: Searches for a value in the first column of a table and returns a matching value from another column.
=VLOOKUP(E2,A2:C10,3,FALSE)

10. XLOOKUP()
Purpose: Searches for a value and returns a corresponding result from another range.
=XLOOKUP(E2,A2:A10,C2:C10,"Not Found")

11. INDEX() and MATCH()
Purpose: Finds a value using a flexible lookup combination.
=INDEX(C2:C10,MATCH(E2,A2:A10,0))

12. IFERROR()
Purpose: Displays a custom result when a formula produces an error.
=IFERROR(A2/B2,0)

13. LEFT(), RIGHT() and MID()
Purpose: Extracts characters from text.
=LEFT(A2,3)
=RIGHT(A2,4)
=MID(A2,2,5)

14. CONCAT() and TEXTJOIN()
Purpose: Combines text from multiple cells.
=CONCAT(A2,B2)
=TEXTJOIN(" ",TRUE,A2:C2)

15. TRIM() and LEN()
Purpose: Removes extra spaces and counts characters.
=TRIM(A2)
=LEN(A2)

16. Absolute and Relative References
Relative reference: "A1"
Absolute reference: "$A$1"
Mixed reference: "$A1" or "A$1"
Purpose: Controls how cell references change when formulas are copied.


---Important Data Analyst Tip
Excel formulas are useful for:
Sales analysis
Customer segmentation
Data cleaning
Finding duplicate records
Monthly reporting
Business performance analysis
