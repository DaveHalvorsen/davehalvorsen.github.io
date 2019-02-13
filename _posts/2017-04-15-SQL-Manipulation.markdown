---
layout: post
title:  "Introduction to SQL"
date:   2017-04-15 22:42:40 -0700
categories: SQL
---

Here are some example commands for interacting with the celebs TABLE. This is from the Codecademy SQL course 'Introduction to SQL'.

This will create the celebs table.
```SQL
CREATE TABLE celebs (
	id INTEGER,
  name TEXT,
  age INTEGER
);
```

This will print everything from the celebs table.
```SQL
SELECT * FROM celebs;
```

Add a row to the celebs table with Justin Bieber's info.
```SQL
INSERT INTO celebs (id, name, age)
VALUES (1, 'Justin Bieber', 21);
```

View the updated celebs table.
```SQL
SELECT * FROM celebs;
```

Adding more celebrities to the table.
```SQL
INSERT INTO celebs (id, name, age)
VALUES (2, 'Beyonce Knowles', 33);

INSERT INTO celebs(id, name, age)
VALUES (3, 'Jeremy Lin', 26);

INSERT INTO celebs (id, name, age)
VALUES (4, 'Taylor Swift', 26);
```

Print just the names column from the celebs table.
```SQL
SELECT name FROM celebs;
```

Edit a table row to have a new age for id 1.
```SQL
UPDATE celebs
SET age = 22
WHERE id = 1;
```

Print just the names column from the celebs table.
```SQL
SELECT name FROM celebs;
```

Add a twitter handle column to the celebs table.
```SQL
ALTER TABLE celebs
ADD COLUMN
twitter_handle TEXT;
```

Print just the names column from the celebs table.
```SQL
SELECT name FROM celebs;
```

Update the twitter_handle for Taylor Swift.
```SQL
UPDATE celebs
SET twitter_handle =
'@taylorswift13'
WHERE id = 4;
```

Print just the names column from the celebs table.
```SQL
SELECT name FROM celebs;
```

Delete the row unless it has a twitter_handle value. This uses the NULL test.
```SQL
DELETE FROM celebs
WHERE twitter_handle IS
NULL;
SELECT * FROM celebs;
```

Create a new table with constraints of id being the primary key, recipient not allowing NULL values and aware name having a default value of "Grammy.""
```SQL
CREATE TABLE awards (
	id INTEGER PRIMARY KEY,
	recipient TEXT NOT NULL,
	award_name TEXT DEFAULT "Grammy"
);
```
