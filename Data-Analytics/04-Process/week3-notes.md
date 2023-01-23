# Key Terms

### Relational database - A database that contains a series of tables that can be connected to form relationships

---

| Spreadsheets                 | SQL                                                         |
| ---------------------------- | ----------------------------------------------------------- |
| Generated with a program     | A language used to interact with database programs          |
| Access to the data you input | Can pull information from different sources in the database |
| Stored locally               | Stored across a database                                    |
| Small datasets               | Larger datasets                                             |
| Working independently        | Tracks changes across team                                  |
| Built-in functionalities     | Useful across multiple programs                             |

- Analysts can use SQL and spreadsheets to perform arithmetic, use formulas, and join data
- Standard SQL works with a majority of databases and requires a small number of syntax changes to adapt to other dialects

---

### Typecasting - Converting data from one type to another

---

## Syntax

### SELECT, FROM - Pull data from any table in a database

```SQL
SELECT
  column_name
FROM
  `database.table`
```

### SELECT, FROM, WHERE - Pull data from a specific place in a table, typically a table column

```SQL
SELECT
  column_name
FROM
  `database.table`
WHERE
  column_name = 'name'
```

### LENGTH() / LEN() - Return the length of a string of text by counting the number of characters it contains

```SQL
SELECT
  column_name
FROM
  `database.table`
WHERE
  LENGTH(column_name) > 1
```

### SUBSTR() - Return a limited number of characters to create substrings from longer strings of text

```SQL
SELECT
  SUBSTR(column_name, 1, 2) AS new_name
FROM
  `database.table`
WHERE
  LENGTH(column_name) > 1
```

### DISTINCT - remove duplicate entires

```SQL
SELECT
  DISTINCT column_name
FROM
  `database.table`
WHERE
  column_name = 'name'
```

### INSERT INTO - Add new data into a database

```SQL
INSERT INTO `database.table`
  (column_1, column_2)
VALUES
  (column_1_value, column_2_value)
```

### UPDATE - Change existing data in a database

```SQL
UPDATE `database.table`
SET column = 'value'
WHERE _id = id
```

### DELETE - REMOVE data from a database

```SQL
DELETE FROM `database.table`
WHERE column = 'column name'
```

### TRIM() - Remove leading, trailing, and repeated spaces in data

```SQL
SELECT
  TRIM(column_name) AS new_name
FROM
  `database.table`
WHERE
  LENGTH(column_name) > 1
```

### COALESCE() - Return non-null values in a list

```SQL
SELECT
  COALESCE(column_name, name) AS new_name
FROM
  `database.table`
ORDER BY
  column_name
```

### CAST() - Convert data from one datatype to another

```SQL
SELECT
  CAST(price AS FLOAT) AS new_price
FROM
  `database.table`
```

### CONCAT() - Add strings together to create new text strings that can be used as unique keys

```SQL
SELECT
  CONCAT(first_name, last_name) AS full_name
FROM
  `database.table`
```
