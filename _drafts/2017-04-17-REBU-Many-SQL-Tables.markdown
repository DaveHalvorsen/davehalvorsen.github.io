---
layout: post
title:  "REBU Many SQL Tables"
date:   2017-04-17 22:42:40 -0700
categories: SQL
---
I am reviewing all of the Codecademy SQL exercises (I completed the Codecademy SQL track recently). I want to make sure that I learn the commands, so I am writing about them.

This returns all of the values from the three tables of: trips, riders, and cars.
```sql
SELECT * FROM trips;
SELECT * FROM riders;
SELECT * FROM cars;
```

I can't imagine when a CROSS JOIN would be useful. It's literally crossing every single row of the first table with every single row of the second table. Here, we're crossing all of the people with all of the cars.
```sql
SELECT riders.first,
	riders.last,
  cars.model
FROM riders, cars;
```

A LEFT JOIN joins *all* of the values from the first table, with the matching values from the second table. Values are matching when they have the same matching criteria. In this case, the matching criteria is trips.rider_id (the rider_id column from the trips table) and riders.id (the id column from the riders table).
```sql
SELECT *
FROM trips
LEFT JOIN riders
  ON trips.rider_id = riders.id;
```

Here, UNION is used to pool the output of two SELECT statements.
```sql
SELECT *
FROM riders
UNION
SELECT *
FROM riders2;
```

Here, the cost column is rounded to two decimal places from the trips table.
```sql
SELECT ROUND(AVG(cost), 2)
FROM trips;
```

How many cars are active? WHERE is used to find statuses that match 'active.'
```sql
SELECT COUNT(*)
FROM cars
WHERE status = 'active';
```

Which cars are used the most? SELECT is used to get the entire output from the cars table. ORDER BY is used to order the output as descending.
```sql
SELECT *
FROM cars
ORDER BY trips_completed DESC
LIMIT 2;
```
