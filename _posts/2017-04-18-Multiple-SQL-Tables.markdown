---
layout: post
title:  "Multiple SQL Tables"
date:   2017-04-18 22:42:40 -0700
categories: SQL
---

I went through all of the Codecademy SQL exercises a while ago. In this article, I will be reviewing the SQL commands from the Multiple Tables exercise. I will discuss what each query does.

These three succssive commands look at three different tables: orders, subscriptions, and customers.
```SQL
SELECT *
FROM orders
LIMIT 5;

SELECT *
FROM subscriptions
LIMIT 5;

SELECT *
FROM customers
LIMIT 5;
```


This joins the orders table and the subscriptions table on locations where the orders table and the subscriptions tables have matching entries for the subscription_id variable.
```SQL
SELECT *
FROM orders
JOIN subscriptions
	ON orders.subscription_id =
  subscriptions.subscription_id;
```


This joins orders and subscriptions where the subscription ids match *and* only where the subscrition table's description variable is Fashion.
```SQL
SELECT *
FROM orders
JOIN subscriptions
	ON orders.subscription_id =
  subscriptions.subscription_id
WHERE subscriptions.description = 'Fashion Magazine';
```

This counts all of the rows from the newspaper table.
```SQL
SELECT COUNT(*)
FROM newspaper;
```


This counts the rows from the online newspaper.
```SQL
SELECT COUNT(*)
FROM online;
```

Sometimes you only want to look at a few rows from a table. The LIMIT command can reduce the output to a requested number of rows. In this case, LIMIT is used to reduce output to 10 rows.
```SQL
SELECT *
FROM newspaper
LIMIT 10;

SELECT *
FROM online
LIMIT 10;
```

A left join collects all of the values from the table on the left with only the matching values from the table on the right. In this case the newspaper table is on the left and the online table is on the right. The tables are joined on the id variable.
```SQL
SELECT *
FROM newspaper
LEFT JOIN online
	ON newspaper.id = online.id;
```



An inner join only pools values together when they match on both the left and right tables. In this case, the left table is classes and the right table is students.
```SQL
FROM classes
JOIN students
	ON classes.id = students.class_id;
```

COUNT(\*) can be used to get the number of rows from the given table. In this case, the SQL query requests the number of newspapers from March. WHERE is used to de-limit the month to March with the start and end month selections that you can see in this SQL query.

```SQL
SELECT COUNT(*)
FROM newspaper
WHERE start_month <= 3
  AND end_month >= 3;
```

A SQL cross join crosses *all* of the rows from the table on the left with *all* of the rows from the table on the right.
```SQL
SELECT *
FROM newspaper
CROSS JOIN months;
```

UNION combines the ouput from two different SQL queries. In this case, everything from the newspaper and online tables is being combined.
```SQL
SELECT *
FROM newspaper
UNION
SELECT *
FROM online;
```
