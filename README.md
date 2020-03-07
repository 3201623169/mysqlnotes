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
3. SELECT * FROM (TABLE_NAME) ORDER BY (COLUMN_NAME);
    **_Data is sorted by (COLUMN_NAME) order._**

### :bulb: KEY NOTES

#### SQL is case insensitive.

which means we can use either upper case or lower case.

#### Fully Qualified Names

SELECT (COLUMN_NAME) FROM (TABLE_NAME) **_is equel to_** 
SELECT (TABLE_NAME.COLUMN_NAME) FROM (TABLE_NAME) 





