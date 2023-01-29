# Key Terms

### Aggregation - Collection or gathering many separate pieces into a whole

### Data aggregation - The process of gathering data from multiple sources in order to combin it into a single summarized collection

- Data aggregation can help data analyst:

  - Identify trends
  - Make comparisons
  - Gain insights

- Data can also be aggregated over a given time period to provide statistics such as:

  - Averages
  - Minimums
  - Maximums
  - Sums

- Functions help make data aggregation possible

### Summarized collection or summary - Describes identifying the data you need and gathering it all together in one place

### Subquery - A query within another query

---

## VLOOKUP (Vertical Lookup)

A Spreadsheet function that vertically searches for a certain value in a column to return a corresponding piece of information

#### Two common reasons to use VLOOKUP:

1. Populating data in a spreadsheet
2. Merging data from one spreadsheet with data in another

#### Preparing for VLOOKUP:

1. Make sure data is in the right format
2. Clear or remove all extra and/or trailing spaces
3. Remove duplicates

#### Basic use

Syntax:

```java
=VLOOKUP(103, A2:B26, 2, FALSE)
```

Explanation:

- `103` is the value to look for
- `A2:B26` is the range to be search
- `2` indicates to search for a match in the second column, since VLOOKUP will not recognize column names such as A, B, or C.
- `FALSE` tells VLOOKUP to find an exact match. When is `TRUE`, returns only a close match

#### VLOOKUP can use between sheets

Syntax:

```java
=VLOOKUP(A2, 'Employee Rates'!$A$2:$B$5, 2, FALSE)
```

Explanation:

- `A2` is the value to look for
- `'Employee Rates!'` indicates look in another sheet
- `$A$2:$B$5` - the range, `$` locks the range
- `2` indicates to search for a match in the second column
- `FALSE` find an exact match

#### Recognize the limitations of VLOOKUP and fix some of the most common problems

- **Troubleshooting questions**:

  - How should I proiritize these issues?
  - In a single sentence, what's the issue I'm facing?
  - What resources can help me solve the problem?
  - How can I stop this problem from happening in the future?

- **Limitations and fixes**:
  - VLOOKUP only returns the first match it finds.
  - VLOOKUP only return a value from the data to the right. It can't look left. Simple solution: copy data to look at to the leftmost, then column containing the data to lookup at is to the right
  - When reference is not absolute reference results would be correct
  - Lock the spreadsheet to prevent others from making changes that can mess up your results. _In spreadsheet select Data (in the top menu) > then Protect sheets and ranges_

#### Exact and approximate matching:

- `TRUE` tells VLOOKUP to look for approximate matches
- `FALSE` tells VLOOKUP to look for exact matches

### VALUE - Spreadsheet function that converts a text string that represents a number to a numerical value

### Absolute reference - A reference that is locked so that rows and columns won't change when copied. _In spreadsheet using `$` to lock the reference_

### MATCH - Spreadsheet function used to locate the position of a specific lookup value

### IFNA - Spreadsheet function to replace the `#N/A` error with something more descriptive

---

## JOIN in SQL

A SQL clause that is used to combine rows from two or more tables based on a related column

**Four common JOINs**: inner, left, right, and full outer

### Primary keys - reference columns in which each value is unique

### Foreign keys - are primary keys in other tables

### INNER JOIN - A function that returns records with matching values in both tables, default

### LEFT JOIN - A function that will return all the records from the left table and only the matching records from the right table

**LEFT is column to the left of the JOIN statement**

**RIGHT is column to the right of the JOIN statement**

### RIGHT JOIN - A function that will return all records from the right table and only the matching records from the left

### OUTER JOIN - A function that combines RIGHT and LEFT JOIN to return all matching records in both tables

### Aliasing - When you temporarily name a table or column in your query to make it easier to read and write

### COUNT - A query that returns the number of rows in a specified range

### COUNT DISTINCT - A query that only returns the distinct values in a specified range

**You'll use COUNT and COUNT DISTINCT any time you want to answer questions about "how many"**

---

## Subquery in SQL

With subqueries you can combine different pieces of logic together.

#### The statement containing the subquery can also be called the outer query or the **outer select**.

#### The subquery is the inner query or **inner select**. The inner query executes first so that the results can be passed on to the outer query to use.

#### Subqueries usually nested in FROM or WHERE clauses.

### HAVING - Allows you to add a filter to your query instead of the underlying table that can only be used with aggregate functions

### CASE - Returns records with your conditions by allowing you to include if/then statements in your query

#### Clauses like HAVING and CASE, paired with subqueries, will help you build more and more complex queries
