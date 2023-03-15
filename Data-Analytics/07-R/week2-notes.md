# Key Terms

## The basic concepts of R:

- **Function**: A body of reusable code used to perform specific tasks in R
- **Argument**: Information that a function in R needs in order to run
- **Variable**: A representation of a value in R that can be stored for use later during programming
  - A variable name should start with a letter and can also contain numbers and underscores
  - `#` : comment operator
  - `<-` : assignment operator
- **Datatype**: An attribute that describes a piece of data based on its values, its programming language, or the operations it can perform
- **Vector**: A group of data elements of the same type stored in a sequence in R
  - ex: `vec_1 <- c(0, 1, 2, 3, 4)`
- **Pipe**: A tool in R for expressing a sequence of multiple operations, represented with `%>%`

  **When using pipes**:

  - Add the pipe operator at the end of each line of the piped operation except the last one
  - Check your code after you've programmed your pipe
  - Revisit piped operations to check for parts of your code to fix

- **Packages**: Units of reproducible R code

  **Packages offer a helpfull combination of code, reusable R functions, descriptive documentation, tests for checking operability, and sample data sets**

  Packages include:

  - Reusable R functions
  - Documentation about the functions
  - Sample datasets
  - Tests for checking your code

  Priority:

  - "base" - means installed and loaded
  - "recommended - means installed but not loaded
  - `library()` : function to install package

### Operator - A symbol that names the type of operation or calculation to be performed in a formula

### Assignment operators - Used to assign values to variables and vectors

### Arithmetic operators - used to complete math calculations

### Logical operators - returns a logical data type such as TRUE or FALSE.

- **There are three primary types of logical operators**:

  - AND (sometimes represented as & or &&)
  - OR (sometimes represented as | or ||)
  - NOT (!)

### Nested - In programming, describes code that performs a particular function and is contained within code that performs a broader function

### Nested function - A function contained within code that performs a broader function. The nested function performs its own specific function within the code.

### CRAN (Comprehensive R Archive Network) - An online archive with R packages, source code, manuals, and documentation

### Tidyverse - A system of packages in R with a common design philosophy for data manipulation, exploration, and visualization

- 8 core tidyverse packages: ggplot2, tibble, tidyr, readr, purrr, dplyr, stringr, and forcats
- `tidyverse_update()`: function for checking for and updating tidyverse
- Four packages that are an essential part of the workflow for data analysts:

  - **ggplot2**: Create a variety of data viz by applying different visual properties to the data variables in R
  - **tidyr**: A package used for data cleaning to make tidy data
  - **readr**: Used for importing data
  - **dplyr**: Offers a consistent set of functions that help you complete some common data manipulation tasks

### Factors - Store categorical data in R where the data values are limited and usually based on a finite group like country or year

### Conflicts happen when packages have functions with the same names as other functions

### `install.packages("package_name")` - function for install package or to just update the installed package

### `installed.packages()` - function shows a list of packages currently installed in an RStudio session. You can then locate the names of the packages and what's needed to use functions from the package.

### `update.packages()` - functin for updating all packages

### Vignette - documentation that acts as a guide to an R package, it shares details about the problem that the package is designed to solve and how the included functions can help you solve it.

### `browserVignettes("package_name")` - function allow you to read through vignettes of a loaded package.
