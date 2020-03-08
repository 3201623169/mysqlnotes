# My MySQL Notes

It's a note book about mysql.

### :cyclone: Display Data (In order)

1. SHOW DATABASES;

2. USE (DATABASE_NAME);

3. SHOW TABLES;

4. SHOW COLUMNS FROM (TABLE_NAME);

5. SELECT (COLUMN_NAME) FROM (TABLE_NAME);

6. SELECT (COLUMN_NAME,COLUMN_NAME,COLUMN_NAME...) FROM (TABLE_NAME);

7. SELECT * FROM (TABLE_NAME);


### :zap: Display Data Advanced

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

9. SELECT (TABLE_NAME1.COLUMN_NAME...),(TABLE_NAME2.COLUMN_NAME) FROM (TABLE_NAME1),(TABLE_NAME2) WHERE (CONDITION);  
    **_It creates a temporary table with the joind table's data._**

10. SELECT (COLUMN_NAME...) FROM (TABLE_NAME1) (INNER/LEFT OUTER/RIGHT OUTER) JOIN (TABLE_NAME2) ON (CONDITION);  
    **_Inner join returns the columns are matched condition in both tables_**  
    **_Left join returns the columns from left table, if matched condition data will be used from right table, else data is null_**  
    **_Right join is similar to left join_**  

11. SELECT (COLUMN_NAME...) FROM (TABLE_NAME1)  
    UNION/UNION ALL  
    SELECT (COLUMN_NAME...) FROM (TABLE_NAME2);  
    **_Union combines multiple datasets into one dataset, and colums in queries must be the same, union will remove duplicates, but nion all will not._**  

### :star2: Operate Data

1.  INSERT INTO (TABLE_NAME) (COLUMN_NAME...) VALUES (VALUE...);  
    **_Insert data into a table_**  

2.  UPDATE (TABLE_NAME) SET (COLUMN_NAME...) WHERE (CONDITION);  
    **_Update data in a table_**  

3.  DELETE FROM (TABLE_NAME) WHERE (CONDITION);  
    **_Delete data in a table_**  

4.  CREATE TABLE (TABLE_NAME)
    (COLUMN_NAME DATA_TYPE(SIZE) (CONSTRAINT) (AUTO_INCREMENT)),...,PRIMARY KEY(COLUMN_NAME));  
    **_Create a new table and specifiy column's name and data type._**  
    **_Constraint includes NOT NULL, UNIQUE, PRIMARY KEY, CHECK, DEFAULT._**

5.  ALERT TABLE (TABLE_NAME) ADD (COLUMN_NAME DATA_TYPE);  
    ALERT TABLE (TABLE_NAME) DROP COLUMN (COLUMN_NAME);  
    ALERT TABLE (TABLE_NAME) CHANGE (COLUMN_NAME) (NEW_NAME) (DATA_TYPE)(SIZE);  
    DROP TABLE (TABLE_NAME);  
    RENAME TABLE (TABLE_NAME) TO (NEW_TABLE_NAME);  
    **_Alert table add or drop column in a table._**   
    **_Drop will drop the entire table._**  

6.  CREATE VIEW (VIEW_NAME) AS SELECT (COLUMN_NAME...) FROM (TABLE_NAME) WHERE (CONDITION);  
    CREATE OR REPLACE VIEW (VIEW_NAME) AS SELECT (COLUMN_NAME...) FROM (TABLE_NAME) WHERE (CONDITION);  
    DROP VIEW (VIEW_NAME);  
    **_View is a virtual table._**  


### :bulb: KEY NOTES

#### SQL is case insensitive.

which means we can use either upper case or lower case.

#### Fully Qualified Names

SELECT (COLUMN_NAME) FROM (TABLE_NAME) **_is equel to_** 

SELECT (TABLE_NAME.COLUMN_NAME) FROM (TABLE_NAME) 

#### COLUMN DATA TYPES

NUMERIC: INT, FLOAT, DOUBLE 

DATE AND TIME: DATE, DATETIME, TIMESTAMP, TIME 

STRING TYPE: CHAR, VARCHAR, BLOB, TEXT 





