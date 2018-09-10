---
layout: post
title:  "SQL Aggregate Functions"
date:   2018-04-15 22:42:40 -0700
categories: SQL
---

SQL calculations performed on multiple rows are called aggregate functions.

You should be used to this starting command by now! It prints out all of the values from the fake_apps table.
```SQL
SELECT * FROM fake_apps;
```

This command counts all of the rows that are in the fake_apps table.
```SQL
SELECT COUNT(*)
FROM fake_apps;
```

It's possible to count all of the free apps with a WHERE clause that sets price equal to 0.
```SQL
SELECT COUNT(*)
FROM fake_apps
WHERE price = 0;
```

Here, SUM is used to get the grand total of all the downloads from fake_apps.
```SQL
SELECT SUM (downloads)
FROM fake_apps;
```

The MIN command can be used to obtain the minimum # of downloads from the fake_apps table.
```SQL
SELECT MIN(downloads)
FROM fake_apps;
```

MAX is the opposite of MIN. Here, MAX gets the biggest price from the fake_apps table.
```SQL
SELECT MAX(price)
FROM fake_apps;
```

Here, the average # of downloads is obtained with the AVG SQL command.
```SQL
SELECT AVG (downloads)
FROM fake_apps;
```

This is a very similar command. It gets the average price from the apps.
```SQL
SELECT AVG (price)
FROM fake_apps;
```

ROUND will round the input value to the selected number of decimal places.
```SQL
SELECT name, ROUND(price, 0)
FROM fake_apps;
```

ROUND can have any # of decimal places selected. Here, round is used to select 2 decimal places.
```SQL
SELECT ROUND(AVG(price), 2)
FROM fake_apps;
```

This selects the prices, counts them and arranges them by price.
```SQL
SELECT price, COUNT(*)
FROM fake_apps
GROUP BY price;
```

This command is very similar to the last command. It selects prices, counts them, and arranges by price, *specifically* where the downloads are greater than 20,000.
```SQL
SELECT price, COUNT(*)
FROM fake_apps
WHERE downloads > 20000
GROUP BY price;
```

This calculates the total number of downloads for each category separately.
```SQL
SELECT category, SUM(downloads)
FROM fake_apps
GROUP BY category;
```

This command collects movies with ratings rounded from 1-5. We're using a new table called imdb_rating. It counts the names of each movie and rounds the rating to 0 decimal places.
```SQL
SELECT ROUND(imdb_rating),
   COUNT(name)
FROM movies
GROUP BY ROUND(imdb_rating)
ORDER BY ROUND(imdb_rating);
```

You can save time in SQL by using the column # instead of the column name. This command is identical to the previous one, but it uses #s instead of columns. The 1 in "GROUP BY 1" represents the imdb_rating column.
```SQL
SELECT ROUND(imdb_rating),
   COUNT(name)
FROM movies
GROUP BY 1
ORDER BY 1;
```

This gets the price column from the fake_apps table. It rounds the downloads to 0 decimal places and counts each of their subsets.
```SQL
SELECT price,
   ROUND(AVG(downloads)),
   COUNT(*)
FROM fake_apps
GROUP BY price;
```

You don't necessarily want to review events that are so rare as to be uninteresting. This is the same as the previous query, *however* it will only present output when a count is greater than 10.
```SQL
SELECT price,
	ROUND(AVG(downloads)),
	COUNT(*)
FROM fake_apps
GROUP BY price
HAVING COUNT(*) > 10;
```
