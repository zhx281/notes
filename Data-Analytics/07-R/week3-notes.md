# Key Terms

### Data Frame - A collection of columns

- Columns should be named
- Data stored can be many different types, like numeric, factor or character
- Each column should contain the same number of data items

### Tibbles - like streamlined data frames

- Never change the data types of the inputs
- Never change the names of your variables
- Never create row names
- Make printing easier

### Tidy data (in R) - A way of standardizing the organization of data within R

- Variables are organized into columns
- Observations are organized into rows
- Each value must have its own cell

### The `head()`, `glimpse()` and `str()` summary functions allow you to preview data frames in R.

- `head()`: returns the columns and the first serveral rows of data
- `glimpse()` or `skim_without_charts()`: returns a summary of the data
- `mutate()`: lets you change the data frame, not preview it

### Cleaning data:

- `rename()`: renames the column name
- `clean_names()`: check column to make sure there is not duplicate
- `rename_with()`: can be used to reformat column names to be upper or lower case

### `arrange()`, `group_by()` and `filter()` functions can be use to help organize data

- `arrange()`: sorting the data
- `group_by()`: grouping the data
- `filter()`: filter results
- `drop_na()`: drops the missing values
- `summarize()`: help summary the data

### `separate()`, `unite()` and `mutate()` functions can be use to help transforming data

- `separate()`: separate data in column to new columns
- `unite()`: combine columns together to new column
- `mutate()`: change data and add to new column

### `sd()`, `cor()` and `mean()` functions can provide a statistical summary of the dataset

- `sd()`: calculates standard deviation
- `cor()`: calculates correlation
- `means()`: calcualtes mean

### Anscombe's quartet - Four datasets that have nearly identical summary statistics

### `bias()` function compares the actual outcome of the data with the predicted outcome to determine whether or not the model is biased. The value should be close to 0 to be unbias.
