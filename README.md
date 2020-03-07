# My MySQL Notes

It's a note book about mysql.

### :cyclone: Display Information (In order)

1. SHOW DATABASES;

2. USE (DATABASE_NAME);

3. SHOW TABLES;

4. SHOW COLUMNS FROM (TABLE_NAME);

5. SELECT (COLUMN_NAME) FROM (TABLE_NAME);

6. SELECT (COLUMN_NAME,COLUMN_NAME,COLUMN_NAME...) FROM (TABLE_NAME);

7. SELECT * FROM (TABLE_NAME);

### :zap: Display Information Advanced

1. SELECT DISTINCT (COLUMN_NAME...) FROM (TABLE_NAME);
    **_As it is distinct, so there will be no duplicate value._**

2. SELECT (COLUMN_NAME...) FROM (TABLE_NAME) LIMIT (NUMBER) / (FROM,NUMBER);
    **_As limited, only (number) records are diplayed._**

3. SELECT * FROM (TABLE_NAME) ORDER BY (COLUMN_NAME...) (DESC);
    **_Data is sorted by (COLUMN_NAME) (DESC) order._**

4. SELECT (COLUMN_NAME) FROM (TABLE_NAME) WHERE (CONDITION);

   SELECT (COLUMN_NAME) FROM (TABLE_NAME) WHERE (CONDITION) AND/OR/NOT IN/IN (CONDITION);

   SELECT (COLUMN_NAME) FROM (TABLE_NAME) WHERE (COLUMN_NAME) LIKE (PATTERN);
    **_The WHERE clause is used to extract only those records that fulfill a specified criterion._**

5. SELECT CONCAT(COLUMN_NAME,SEPRATOR,COLUMN_NAME...) FROM (TABLE_NAME);
    **_The concat function concats two or more columns with a seprator._**

6. SELECT UPPER(COLUMN_NAME).../LOWER(COLUMN_NAME)... FROM (TABLE_NAME);
    **_The upper and lower function converts string to uppercase or lowercase._**

7. SELECT SUM(COLUMN_NAME) FROM (TABLE_NAME);
    **_The sum function calculates the sum of a column's values._**

8. SELECT MIN(COLUMN_NAME) FROM (TABLE_NAME);
    **_The min function return the min value in a column._**

### :bulb: KEY NOTES

#### SQL is case insensitive.

which means we can use either upper case or lower case.

#### Fully Qualified Names

SELECT (COLUMN_NAME) FROM (TABLE_NAME) **_is equel to_** 

SELECT (TABLE_NAME.COLUMN_NAME) FROM (TABLE_NAME) 





