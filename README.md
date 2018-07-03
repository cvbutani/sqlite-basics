## SQLITE3 GUIDE
- All SQL commands should end with a semicolon(;).
- SQL commands are capitalize but not necesssary.
- dot(.) commands are specifically for sqlite3. e.g, open or close database.
- dot commands are case sensitive.
- Primary Key: Ensures uniqueness. There can only be one primary key per table.
- Auto Increment: Automatically calculates new integer when row is added for IDs.

##### OPEN SQLITE3
```
sqlite3
```

##### FOR HELP
```
.help
```

##### CREATE/OPEN NEW FILE
```
.open your_db_name.db
```

##### CHECK IF SQLITE HAS ANY TABLES
```
.tables
```

##### CREATE TABLE WITH PRIMARY KEY
```
CREATE TABLE table_heading(_id INTEGER PRIMARY KEY AUTOINCREMENT, column_heading1 TEXT, column_heading2 INTEGER, column_heading3 INTEGER, column_heading4 TEXT);
```
##### CREATE TABLE
```
CREATE TABLE table_heading(_id INTEGER, column_heading1 TEXT, column_heading2 INTEGER, column_heading3 INTEGER, column_heading4 TEXT);
```

##### HEADER ON
```
.header on
```

##### CREATE TABLE
```
.schema table_heading
```

##### PRINT HEADINGS OF COLUMN
```
PRAGMA TABLE_INFO(table_heading);
```

##### INSERT INFO IN TABLE
```
INSERT INTO table_heading(_id, column_heading1, column_heading2, column_heading3, column_heading4)
    VALUES (1, "TABLE1", 89, 5, "HEAD1");
```

##### READING SINGLE COLUMN FROM TABLE
```
SELECT column_heading1 FROM table_heading;
```

##### READING EVERYTHING FROM TABLE
```
SELECT * FROM table_heading;
```

##### READING MODES
```
.mode tabs
.mode ascii
.mode column
.mode list
```

##### DELETE TABLE
```
DROP TABLE table_heading;
```
