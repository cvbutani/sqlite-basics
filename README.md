## SQLITE3 GUIDE
- All SQL commands should end with a semicolon(;).
- SQL commands are capitalize but not necesssary.
- dot(.) commands are specifically for sqlite3. e.g, open or close database.
- dot commands are case sensitive.
- Primary Key: Ensures uniqueness. There can only be one primary key per table.
- Auto Increment: Automatically calculates new integer when row is added for IDs.
- NOT NULL - Null values are not allowed for this column.
- Default<value> - When inserting a new row, if no value is defined, the default value given will be used.

##### Open Sqlite3
```
sqlite3
```

##### Help
```
.help
```

##### Create/Open new file
```
.open your_db_name.db
```

##### Check if table exists or not
```
.tables
```

##### Create table with primary key
```
CREATE TABLE table_heading(_id INTEGER PRIMARY KEY AUTOINCREMENT, column_heading1 TEXT, column_heading2 INTEGER, column_heading3 INTEGER, column_heading4 TEXT);
```
##### Create table
```
CREATE TABLE table_heading(_id INTEGER, column_heading1 TEXT, column_heading2 INTEGER, column_heading3 INTEGER, column_heading4 TEXT);
```

##### Header on
```
.header on
```

##### Schema used to create table
```
.schema table_heading
```

##### Print column headings
```
PRAGMA TABLE_INFO(table_heading);
```

##### Insert information in table
```
INSERT INTO table_heading(_id, column_heading1, column_heading2, column_heading3, column_heading4)
    VALUES (1, "TABLE1", 89, 5, "HEAD1");
```

##### Reading single column from table
```
SELECT column_heading1 FROM table_heading;
```

##### Reading everything from table
```
SELECT * FROM table_heading;
```

##### Reading methods
```
SELECT * FROM table_heading WHERE _id == 1;
SELECT * FROM table_heading WHERE column_heading1 >= 3;
SELECT column_heading1, column_heading3 FROM table_heading;
SELECT * FROM pets ORDER BY column_heading1 ASC;
SELECT * FROM pets ORDER BY column_heading1 DSC;
```

##### Reading modes
```
.mode tabs
.mode ascii
.mode column
.mode list
```

##### Edit/Update table
```
UPDATE table_heading SET column_heading2 = 5 WHERE column_heading3 = 1;
```

##### Delete table data
```
DELETE FROM table_heading WHERE _id = <id_you_want_to_delete>;
```

##### Delete table
```
DROP TABLE table_heading;
```

FOR MORE INFORMATION [CLICK HERE](https://d17h27t6h515a5.cloudfront.net/topher/2016/September/57ed880e_sql-sqlite-commands-cheat-sheet/sql-sqlite-commands-cheat-sheet.pdf)
