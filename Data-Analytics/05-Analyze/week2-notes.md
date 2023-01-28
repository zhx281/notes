# Key Terms

### Incorrectly formatted data can: Lead to mistakes, take time to fix, and Affect stakeholder's decision-making

---

## Spreadsheet Functions

---

### CONVERT - function for convert the cell's format to another format

- cell
- origninal format
- format to

```
=CONVERT(D2, "mph", "m/s")
```

### CONCAT - function for combinating 2 cells

### CONCATENATE - function for combination multiple cells or strings

```
=CONCAT(A2, B2)

=CONCATENATE(A2, " ", B2)
```

### Date validation - Allows you to control what can and can't be entered in your worksheet

- Add dropdown lists with predetermined options
  - Select the column or cells > click on Data (in the top menu) > Data validation > Add rules > choose Dropdown > enter the dropdown values
- Create custom checkboxes
  - Select the column or cells > click on Data (in the top menu) > Data validation > Add rules > choose Checkbox (optional check for custom values)
- Protect structured data and formulas
  - By select the Advanced options and select the Reject the input under the "If the data is invalid" with the Data validation rules

### Conditional formatting - A spreadsheet tool that changes how cells appear when values meet specific conditions

- click on Format (in the top menu) > Conditional format > select the range of cells > using Format rules to specific the condition for formatting style

### LEN - length of a string

### FIND - find first position of string, case-sensitive. ex: =FIND(" ", A2)

### LEFT or RIGHT - to select which part of the string to isolate. ex: =RIGHT(A2, 8)

---

### Best practices for searching online:

- Thinking skills
- Data analytics terms - using the right terms or keyword
- Basic knowledge of tools
- Understanding syntax - being able to modify existing code

### Mental model - Your thought process and the way you approach a problem

### R - A programming language frequently used for statistical analysis, visualization, and other data analysis

### When to use which tool:

- Pivot table - when there is small amount of data
- SQL - when there is huge amount of data, and/or spreadsheet keeps crashing
  - SQL is great for querying, updating, and optimizing data
  - Can get complicated when trying to analyze data with only SQL
