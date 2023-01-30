## Commmon calculation fourmulas

| --- |
| **Spread sheet** |
| --- |

### SUM - calculate the total between cells

### Percentage change - N / B - 1

### AVERAGE - calculate the average between cells

### Conditional formatting with color scale display the range of specific color range

### MIN - Find the minimum, or the smallest, between cells

### MAX - Find the maximum, or the largest, between cells

### COUNTIF - Counting the total when the IF condition is met

- Syntax: =COUNTIF(range, criteria/condition)

```
=COUNTIF(B2:B20, ">1")
```

- `B2:B20` is the specific range of cells
- `">1"` is the condition, which in this case greater than 1

### COUNTIFS - Similar to COUNTIF but can include multiple conditions

- Syntax: =COUNTIFS(criteria_range1, criterion1, [critria_range2, citeria_range2, ...])

```
=COUNTIFS(A1:A9, "Coffee", C1:C9, "12/15/2020")
```

- `A1:A9` is the specific range or cells for the counting to happen in
- `"Coffee"` is the first condition to be meet or criterion1, where the string is Coffee
- `C1:C9` is the specific range or cells for the second condition to consider
- `"12/15/2020"` is the second condition to be meet or criterion2, where the date is 12/15/2020

### SUMIF - A function that adds numberic data based on one condition

- Syntax: =SUMIF(range, criteria/condition,[sum_range])

```
=SUMIF(B2:B20, "=1", C3:C20)
```

- `B2:B20` is the specific range for the condition
- `"=1"` is the condition
- `C3:C20` is the specific range or cells to perfrom the sum function for

### SUMIFS - Similar to SUMIF but can include multiple conditions

- Syntax: =SUMIFS(sum_range, criteria_range1, criterion1, [criteria_range1, criterion2, ...])

```
=SUMIFS(B1:B9, A1:A9, "Fuel", C1:C9, "12/15/2020")
```

- `B1:B9` is the specific range or cells to perform the sum function for
- `A1:A9` is criteria_range1
- `"Fuel"` is the first condition to be meet or criterion1 where string is equal to Fuel
- `C1:C9` is criteria_range2
- `12/15/2020` is the second condition to be meet or criterion2 where the date is 12/15/2020

### Array - A collection of Values in cells

### SUMPRODUCT - A function that multiplies arrays and returns the sum of those products

- Syntax: =SUMPRODUCT(array1, [array2]...)

```
=SUMPRODUCT(B2:B5, C2:C5)
```

- `B2:B5` is the first array
- `C2:C5` is the second array

The SUMPRODUCT function would multiply the each row of the arrays, then calculate the SUM or total of the product.

### Profit margin - A percentage that indicates how many cents of profit has been generated for each dollar of sale

| --- |
| Pivot Tables |
| --- |

### Calculated field - A new field within a pivot table carries out certain calculations based on the values of other fields

---

### Check and recheck - Helps ensure the data is complete, accurate, secure, and consistent

### Validating process:

- **Data type** means checking that the data matches the data type defined for the field
- **Data range** means checking that the data falls within an acceptable range of values defined for the field
- **Data constraints** means checking that the data meets certain conditions or criteria, such as type of characters
- **Data consistency** means checking that the data makes sense in the context of other related data
- **Data structure** means checking that the data follows or conforms to a set structure, such as MP3 files or HTML code
- **Code validataion** means checking that the application code systematically performs any of the previously mentionad validations during user data input

---

### Operator - A symbol that names the type of operation or calculation to be performed in a formula

### Modulo (%) - A operator that returns the remainder when one number is divided by another

### Underscores - Lines used to underline words and connect text characters

### GROUP BY - A SQL command that groups rows that have the same values from a table into summary rows

### EXTRACT - A SQL command that extract any part from date/time value

### Temporaty table - A database table that is created and exists temporarily on a database server

### WITH - clause is a type of temporary table that you can query from multiple times
