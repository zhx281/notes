# Key Terms

### Verification - A process to confirm that a data-cleaning effort was well-executed and the resulting data is accurate and reliable, and also consider whether the data is credible and appropriate for the project

### When verifying data-cleaning:

1. Consider the business problem
2. Condider the goal
3. Consider the data

   Take a big picture, and ask "Do the numbers make sense?"

| Data-cleaning verification               |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Common problems                          | Corrections check                                                                                          |
| -----                                    | ----                                                                                                       |
| **Sources of errors**                    | Did you use the right tools and functions to find the source of the errors in your dataset?                |
| **Null data**                            | Did you search for NULLs using conditional formatting and filters?                                         |
| **Misspelled words**                     | Did you locate all misspellings?                                                                           |
| **Mistyped numbers**                     | Did you double-check that your numeric data has been entered correctly?                                    |
| **Extra spaces and characters**          | Did you remove any extra spaces or characters using the **TRIM** function?                                 |
| **Duplicates**                           | Did you remove duplicates in spreadsheets using the **Remove Duplicates** function or **DISTINCT** in SQL? |
| **Mismatched data types**                | Did you check that numeric, date, and string data are typecast correctly?                                  |
| **Messy (inconsistent) strings**         | Did you make sure that all of your strings are consistent and meaningful?                                  |
| **Messy (inconsistent) date formats**    | Did you format the dates consistently throughout you dataset?                                              |
| **Misleading variable labels (columns)** | Did you name your columns meaningfully?                                                                    |
| **Truncated data**                       | Did you check for truncated or missing data that needs correction?                                         |
| **Business Logic**                       | Did you check that the data makes sense given your knowledge of the business?                              |

---

### Documentation - The process of tracking changes, additions, deletions, and errors involved in your data-cleaning effort

    **Benefits of documentation:**

    - Recalling the errors that were cleaned
    - Inform other of the changes (assume that the data error aren't fixable or when data errors are fixable, how the data was fixed)
    - Determine quality of data

### Changelog - A file containing a chronologically ordered list of modifications made to a project

---

## Spreadsheet

---

### Pivot table - A data summarization tool that is used in data processing

### Find and replace - A tool that looks for a specified search term in a spreadsheet and allows you to replace it with something else

### COUNTA - A function that counts the total number of values within a specified range

---

## SQL

---

### CASE statement - The CASE statement goes through one or more conditions and returns a value as soon as a condition is met

```SQL
SELECT
  customer_id,
  CASE
    WHEN first_name = 'Tnoy' THEN 'Tony'
    ELSE first_name
    END AS cleaned_name
FROM
  customer_data.customer_name

-- for multiple CASEs

SELECT
  customer_id,
  CASE
    WHEN first_name = 'Tnoy' THEN 'Tony'
    WHEN first_name = 'Tmo' THEN 'Tom'
    WHEN first_name = 'Rachle' THEN 'Rachel'
    ELSE first_name
    END AS cleaned_name
FROM
  customer_data.customer_name
```
