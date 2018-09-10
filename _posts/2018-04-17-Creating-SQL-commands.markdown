---
layout: post
title:  "Creating SQL Tables"
date:   2018-04-17 22:42:40 -0700
categories: SQL
---

Here are some of the SQL table creation exercises from Codecademy. I have added my own explanations to them to aid in my memorization.

Here's the basic SQL command to create a table. This table is called friends. It has a column named id that accepts integers, a column called name, that accepts text, and a birthday, that accepts dates.
```SQL
CREATE TABLE friends (
	id INTEGER,
  name TEXT,
  birthday DATE
);
```

You can insert into a table with the INSERT command. In this case, we are inserting into the table called friends, that has columns of id, name, and birthday. The values that are being inserted are 1, Jane Doe and the birthday.
```SQL
INSERT INTO friends (id, name, birthday)
VALUES (1, 'Jane Doe', '1990-05-30');
```

This command is essential! It prints out all of the entries from a selected table.
```SQL
SELECT * FROM friends;
```

The INSERT INTO command is used here to add two rows to the friends table. Note that the first parenthesis holds the column names and the second parenthesis sets are for the values that are getting added.
```SQL
INSERT INTO friends (id, name, birthday)
VALUES (2, 'Chris', '1976-05-12');
INSERT INTO friends (id, name, birthday)
VALUES (3, 'Jeff', '1993-03-22');
```

The UPDATE command can change values that are already in a table. Here Jane Smith's last name is being changed to Doe.
```SQL
UPDATE friends
SET name = 'Jane Smith'
WHERE name = 'Jane Doe';
```

ALTER TABLE, in this case, is being used to add a column called email that accepts text values.
```SQL
ALTER TABLE friends
ADD COLUMN
email TEXT;
```

This set of three SQL commands gives out email addresses to three different individuals. Note that WHERE is being used to select the id of each individual.
```SQL
UPDATE friends
SET email = 'email_Jane@gmail.com'
WHERE id = 1;

UPDATE friends
SET email = 'chris@chris.net'
WHERE id = 2;

UPDATE friends
SET email = 'Jeff@jeff.net'
WHERE id = 3;
```

Here, the DELETE command is being used to remove Jane Smith from the table.
```SQL
DELETE FROM friends
WHERE name = 'Jane Smith';
```
