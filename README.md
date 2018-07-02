# SQLITE3 GUIDE
- All SQL commands should end with a semicolon(;).
- SQL commands are capitalize but not necesssary.
- dot(.) commands are specifically for sqlite3. e.g, open or close database.
- dot commands are case sensitive.

#### OPEN SQLITE3
```
sqlite3
```

#### FOR HELP
```
.help
```

#### CREATE/OPEN NEW FILE
```
.open your_db_name.db
```

#### CHECK IF SQLITE HAS ANY TABLES
```
.tables
```

#### CREATE TABLE
```
CREATE TABLE table_heading(column_heading1 TEXT, column_heading2 INTEGER, column_heading3 INTEGER, column_heading4 TEXT);
```

#### STATEMENT USE TO CREATE TABLE
```
.schema table_heading
```

#### DISPLY HEADINGS OF COLUMN IN PARTICULAR TABLE
```
PRAGMA TABLE_INFO(table_heading);
```

#### DELETE TABLE
```
DROP TABLE table_heading;
```
