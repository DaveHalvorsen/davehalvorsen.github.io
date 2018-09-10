---
layout: post
title:  "SQL Restaurant Queries"
date:   2018-04-18 22:42:40 -0700
categories: SQL
---
I have already completed all of the SQL exercises from Codecademy. This set of exercises surrounds a fictional restaurant database. I am reviewing the commands here to make sure that I understand them.

This is essential! Select \* returns all of the values from the table.
```SQL
SELECT * FROM nomnom;
```

DISTINCT will only return one for each time that an item is repeated. Here it is used to obtain a list of each neighborhood from the nomnom table.
```SQL
SELECT DISTINCT neighborhood FROM nomnom;
```

Here, the DISTINCT SQL command is again used. This time it gets each unique cuisine type.
```SQL
SELECT DISTINCT cuisine FROM nomnom;
```

Here, \* is used to get *all* of the values from nomnom WHERE the cuisine type is Chinese.
```SQL
SELECT * FROM nomnom
WHERE cuisine = "Chinese";
```

Here, \* is used to get *all* of the values from the nomnom table WHERE the review is greater than or equal to 4.
```SQL
SELECT * FROM nomnom
WHERE review >= 4;
```

The WHERE command isn't just used on numbers. It can match letters as well. Here, WHERE is used to find the cuisine of Italian and the price of $$$.
```SQL
SELECT * FROM nomnom
WHERE cuisine = "Italian"
AND price = "$$$";
```

I thought this was a great SQL command! Suppose you can't remember the name of one of the restaurants, but you *can* remember part of the name. The SQL command of LIKE is used here to match a name that has meatball in the center and an unknown number of characters to the left and right.
```SQL
SELECT * FROM nomnom
WHERE name LIKE "%meatball%";
```

What if you'd like to determine all of the nearby restaurants? This SQL query uses WHERE and OR to return restaurants near three neighborhoods.
```SQL
SELECT * FROM nomnom
WHERE neighborhood = 'Midtown' OR
neighborhood = 'Downtown' OR
neighborhood = 'Chinatown';
```

You'd obviously like to avoid restaurants that haven't received a health code rating yet! This SQL query uses IS NULL to find all of the restaurants that haven't received a health code rating yet.
```SQL
SELECT * FROM nomnom
WHERE health IS NULL;
```

Here's how to create a top ten ranking of all the local restaurants. LIMIT is used to only allow 10 rows. ORDER BY is applied to review with the DESC (descending) selection.
```SQL
SELECT * FROM nomnom
ORDER BY review DESC
LIMIT 10;
```

CASE is SQL's way of using if, then, else logic. This SQL statement returns a Review column with Excellent, Good, Fair or Poor. Those values are assigned based on the review being above the threshold values from within the command.
```SQL
SELECT name,
	CASE
  	WHEN review > 4.5 THEN 'Extraordinary'
    WHEN review > 4 THEN 'Excellent'
    WHEN review > 3 THEN 'Good'
    WHEN review > 2 THEN 'Fair'
    ELSE 'Poor'
  END AS 'Review'
FROM nomnom;
```
