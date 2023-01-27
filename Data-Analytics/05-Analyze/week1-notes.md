# Key Terms

### Analysis - The process used to make sense of the data collected
 - The goal of analysis is to identify trends and relationships within data so you can accurately answer the question you're asking.
 - **The 4 phases of analysis**:
    1. Organize data - gahtering the data
    2. Format and adjust data - streamlines things and saves you time, sorting and filtering, eliminate irrelevant info from your data
    3. Get input from others - gives you a viewpoint you might not understand or have access to
    4. Transform data - identifying relationships and patterns, and making calculations based on data you have

----

### Most of the datasets will be organized as tables.

### Sorting and filtering are to ways to keep things organized when format and adjust data

### Sorting vs Filtering
  - **Sorting** - ranks your data based on a specific metric you choose to make it easier to understand analyze, and visualize
  - **Filtering** - really useful when you have lots of data and you are only interested in seeing data that meets a specific criteria, and hiding the rest
  - Use sort to quickly order the data 
  - Use filter to display only the data that meets the criteria
  - After you filter data, you can sort the filtered data

### Outliers - data points that are very different from similarly collected data and might not be reliable values.

---
## Sorting in Spreadsheet
---

### Sort sheet - All of the data in a spreadsheet is sorted by the ranking of a specific sorted column (data across rows is kept together).
  - In Google shreadsheet, first select the column to be sorted then click Data (in the top menu bar) > Sort Sheet > choose either the (A to Z) for ascending order or (Z to A) for descending order 

### Sort Range - Nothing else on the spreadsheet is rearranged besides the specified cells in a column
  - In Google shreadsheet, first select the column to be sorted then click Data (in the top menu bar) > Sort Range > choose either the (A to Z) for ascending order or (Z to A) for descending order 

### Customized sort order - When you sort data in a spreadsheet using multiple conditions
  - In Google shreadsheet, first select all columns and rows (including header row) then click Data (in top menu) > Sort range > Advanced range sorting options
    - check Data has header row
    - select the column to sort by and (A to Z) for ascending order or (Z to A) for descending order 
    - Add another sort column for additional options

### SORT Function - Change to effect the entire dataset
  - Range Field : Range of cells
  - Index of sort column: Integer
  - Ascending or descending : Bool
 ```
 =SORT(A2:B6, 2, True)
 ```
 
---
## Sorting in DQL
---

### ORDER BY - Sort dataset by specific column, default in ascending order
  - Make sure the ORDER By clause to the last line 
```sql
SELECT 
  * 
FROM 
  `movie_data.movies`
ORDER BY Release_Date
 
-- Add DESC clause for descending order
ORDER BY Release_Date DESC

-- Combine with filters
-- WHERE clause
SELECT 
  * 
FROM 
  `movie_data.movies`
WHERE 
  Genre = "Comedy"
ORDER BY Release_Date

-- WHERE and AND clause
SELECT 
  * 
FROM 
  `movie_data.movies`
WHERE 
  Genre = "Comedy"
AND
  Revenue > 300000000
ORDER BY Release_Date DESC
 
```

### IF - function for checking 
```sql
SELECT
  -- replace the 9999.9 values as NULL
  IF (
  temp=9999.9,
  NULL,
  temp) AS temperature
```
