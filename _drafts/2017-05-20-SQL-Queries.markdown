---
layout: post
title:  "SQL Queries"
date:   2017-04-18 22:42:40 -0700
categories: SQL
---
I completed the Codecademy SQL track a while back. This is part of a series of articles that I am writing to review that material, so that I can solidify all of the SQL commands in mind.

SELECT \* gets *all* of the values from the movies table.
```sql
SELECT * FROM movies;
```

Here, SELECT is used to get the column names of 'name' and 'genre' from the movies table.
```sql
SELECT name, genre
FROM movies;
```

You can use AS to create an alias for a selected column. In this case, the column name is given the alias of 'thing'.
```sql
SELECT name as 'thing'
FROM movies;
```

Here, DISTINCT is used to get a list of each genre type.
```sql
SELECT DISTINCT genre
FROM movies;
```

Here, WHERE is used to limit the totality of the movies table to only movies that had a rating of lower than 5.
```sql
SELECT * FROM movies
WHERE imdb_rating < 5;
```

Here, WHERE is used to limit the output of the movies table to movies that are newer than 2014.
```sql
SELECT * FROM movies
WHERE year > 2014;
```

The SQL command of LIKE, combined with the '\_' wildcard can be used to find internal matches for character searches. In this case, we are looking for a movie the starts with 'Se', has one character, and then ends with 'en.'
```sql
SELECT *
FROM movies
WHERE name LIKE 'Se_en';
```

The '\_' wildcard is for characters *within* a string. The '%' wildcard is for characters to the left or right of a given string.
```sql
SELECT *
FROM movies
WHERE name LIKE '%man%';
```

Here, IS NULL is being used to find moves that do not have a rating.
```sql
SELECT name
FROM movies
WHERE imdb_rating IS NULL;
```

This selects for movies that begin with d-f. Note that BETWEEN IS exclusive of the end for letters.
```sql
SELECT *
FROM movies
WHERE name BETWEEN 'D' AND 'G';
```


This selects movies from the 70s. Note that BETWEEN is inclusive of end for #s. I think this is silly to change syntax like this from the exclusive syntax for letters.
```sql
SELECT *
FROM movies
WHERE year BETWEEN 1970 and 1979;
```

What movies were released in the 70s *and* have an IMDB score of greater than 8?
```sql
SELECT *
FROM movies
WHERE year BETWEEN 1970 AND 1979
	AND imdb_rating > 8;
```

What about movies from older than 1985 and have the genre of horror?
```sql
SELECT *
FROM movies
WHERE year < 1985
	AND genre = 'horror';
```

This query gets movies after 2014 that are action.
```sql
SELECT *
FROM movies
WHERE year > 2014
OR genre = 'action';
```

This gets romance *or* comedy movies.
```sql
SELECT *
FROM movies
WHERE genre = 'romance'
	OR genre = 'comedy';
```

This query gets the name and year columns from the movies table. The results are ordered by name with the ORDER BY command.
```sql
SELECT name, year
FROM movies
ORDER BY name;
```

This SQL query gets the name, year, and imdb_rating columns from the movies table. The results are ordered by the rating. ORDER BY is how to order the results. DESC is how to select descending.
```sql
SELECT name, year, imdb_rating
FROM movies
ORDER BY imdb_rating DESC;
```

What are the best 3 movies? This query requests *everything* from the movies table. It uses ORDER BY with a selection of DESC and a LIMIT of 3 to properly query the table.
```sql
SELECT *
FROM movies
ORDER BY imdb_rating DESC
LIMIT 3;
```

CASE is the SQL method of using if, then, else logic. This SQL query will return 'Chill' for 'romance' genre. Otherwise, it will return 'Intense'.
```sql
SELECT name,
	CASE
  	WHEN genre = 'romance' THEN 'Chill'
    WHEN genre = 'comedy' THEN 'Chill'
    ELSE 'Intense'
  END AS 'Mood'
FROM movies;
```
