---
layout: post
title:  "List of SQL Commands"
date:   2017-04-15 22:42:40 -0700
categories: SQL
---
These are the basic SQL commands.

ALTER TABLE lets you add columns.
```SQL
ALTER TABLE table_name
ADD column_name datatype;
```

AND is an operator that combines two conditions
```SQL
SELECT column_name(s)
FROM table_name
WHERE column_1 = value_1
AND column_2 = value_2;
```

Rename a column with AS.
```SQL
SELECT column_name AS 'Alias'
FROM table_name;
```

Average a column with AVG.
```SQL
SELECT AVG(column_name)
FROM table_name;
```

Filter a result within a certain range with BETWEEN.
```SQL
SELECT column_name(s)
FROM table_name
WHERE column_name BETWEEN value_1 and value_2;
```

Use if, else, then logic with CASE.
```SQL
SELECT column_name,
  CASE
    WHEN condition THEN 'Result_1'
    WHEN condition THEN 'Result_2'
    ELSE 'Result_3'
  END
FROM table_name;
```

Count the number of rows that are not null with COUNT.
```SQL
SELECT COUNT(column_name)
FROM table_name;
```

Create a table with CREATE TABLE.
```SQL
CREATE TABLE table_name (
  column_1 datatype,
  column_2 datatype,
  column_3 datatype
);
```

Delete rows from a table with DELETE.
```SQL
DELETE FROM table_name
WHERE some_column = some_value;
```

GROUP BY arranges data into groups.
```SQL
SELECT column_name, COUNT(*)
FROM table_name
GROUP BY column_name;
```

Adding a conditional to a command with HAVING.
```SQL
SELECT column_name, COUNT(*)
FROM table_name
GROUP BY column_name
HAVING COUNT(*) > value;
```

Combine rows from different tables with JOIN.
```SQL
SELECT column_name(s)
FROM table_1
JOIN table_2
  ON table_1.column_name = table_2.column_name;
```

Insert data into a table with INSERT and VALUES.
```SQL
INSERT INTO table_name (column_1, column_2, column_3)
/* It's not specified on the Codecademy page, but I believe the quotes
are for test and no quotes are for numbers */
VALUES (Value_1, 'value_2', value_3);
```

NULL means no value is present.
```SQL
SELECT column_name(s)
FROM table_name
WHERE column_name IS NULL;
```

LIKE allows you to search for patterns.
```SQL
SELECT column_name(s)
FROM table_name
WHERE column_name LIKE pattern;
```

LIMIT specifies the number of rows returned
```SQL
SELECT column_name(s)
FROM table_name
LIMIT number;
```

MAX returns the largest value from a column.
```SQL
SELECT MAX(column_name)
FROM table_name;
```

MIN returns the smallest value from a column.
```SQL
SELECT MIN(column_name)
FROM table_name;
```

You can use OR if you'd like to make use of or logic (as opposed to and/else).
```SQL
SELECT column_name
FROM table_name
WHERE column_name = value_1
  OR column_name = value_2;
```

You can sort returned items alphabetically or numerically with ORDER BY.
```SQL
SELECT column_name
FROM table_name
/* I believe the pipe and two choices is just showing options */
ORDER BY column_name ASC | DESC;
```

A LEFT JOIN will combine rows from different tables *even* if the join condition is not met.
```SQL
SELECT column_name(s)
FROM table_1
LEFT JOIN table_2
  ON table_1.column_name = table_2.column_name;
```

You can use ROUND to round the values to specified # of decimal places.
```SQL
SELECT ROUND(column_name, integer)
FROM table_name;
```

Get data from a table with SELECT and FROM.
```SQL
SELECT column_name
FROM table_name;
```

You can grab unique values with UNIQUE.
```SQL
SELECT DISTINCT column_name
FROM table_name;
```

SUM will obtain the sum of the selected values.
```SQL
SELECT SUM(column_name)
FROM table_name;
```

UPDATE is used to edit the rows from a table. SET is what sets the new value. WHERE defines where values are set.
```SQL
UPDATE table_name
SET some_column = some_value
WHERE some_column = some_value;
```

WHERE can be used to filter results based on some requirement.
```SQL
SELECT column_name(s)
FROM table_name
WHERE column_name operator value;
```

WITH is used to create a temporary table.
```SQL
WITH temporary_name AS (
  SELECT *
  FROM table_name)
SELECT *
FROM temporary_name
WHERE column_name operator value;
```
