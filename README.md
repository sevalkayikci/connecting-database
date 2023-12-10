# connecting-database
connection to MySQL using Python










import : statement used to bring in external modules or libraries

mysql.connector: python driver for MySQL – it allows python programs to connect and interact
with MySQL databases.

pymysql:used to connect database and execute SQL queries.

conn: connection object represents the connection to database

cursor: pointer to result set

pymysql.connect(): used to establish a connection to SQL server.- parameters should include →
host, user,password

creating cursor → conn.cursor():used to interact with database and execute SQL queries

creating database → cursor.execute(): to create database we use CREATE DATABASE but if there is
a database with the same name it may cause error so we use IF NOT EXISTS to check then create

commiting changes → con.commit(): used to commit changes

closing cursor and connections → cursor.close(): close the cursor after executing all queries

conn.close():closes the database connection

pip install mysql-connector-python : we used this to import mysql connector library into python

mysql.connector.connect(): make connectipn to msql database server
you should add host, user,password and database as parameters to work

conn.is_connected() : used to check if the connection to database is open
returns bool(true or false)

cursor.fetchall() : fetches all rows in query
returns list of tuples (we used for loop to print all rows)
used after SELECT
