## Working with SQLite3

### Instalation
www.sqlite.org
Download and Install SQLite3 tools for PC
Set Path in Enviroment Variables

### Overview

SQLite3 is a software library that provides a RDMS (Relational database management system). The lite in SQLite means lightweight in terms of setup, administration of db and required sources.

SQLite3 is serverless, self-contained and has zero-configuration. Unlike PostgreSQL, MySQL and etc, they require a separate server process to operate. It is intergrated within the application accessing the database. Applications will read and write directly from the database files stored on disk.

During the learnings I found that the database single connection to access multiple database files. This helps with features like joining tables in different databases or copying data between db in a single command. This is niiiiiice. 

### Database Data Info

release_list = [
    (1997, "Grand Theft Auto", "state of New Guernsey"),
    (1999, "Grand Theft Auto 2", "Anywhere, USA"),
    (2001, "Grand Theft Auto III", "Liberty City"),
    (2002, "Grand Theft Auto: Vice City", "Vice City"),
    (2004, "Grand Theft Auto: San Andreas", "state of San Andreas"),
    (2008, "Grand Theft Auto IV", "Liberty City"),
    (2013, "Grand Theft Auto V", "Los Santos")
]    

city_list = [
    ("Liberty City", "New York"),
    ("state of New Guernsey", "state of New Jersey"),
    ("Anywhere, USA", "all USA cities"),
    ("Vice City", "Miami"),
    ("state of San Andreas", "state of California"),
    ("Los Santos", "Los Angeles")
]


### Features Learned

- connection: To connect to a database, connection or "con" is typically used to do so. 

- cursor: A cursor or "cur" is used to perfrom SQL commands with execute.

- execute(): is a method used to perform SQL commands with cursor.

- executemany() : is a method that is used to perform multiple SQL commands.

- fetchall(): a method that fetches all (or all remaining) rows of a query result set and returns a list of tuples.

- connection.close(): used to close a connection to a SQL database. Sometimes "conn.close()" is used depending on how you originally connected to the database.
