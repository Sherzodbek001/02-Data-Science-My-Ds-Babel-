# Description

It stands for Structured Query Language. It helps you perform queries in a database. The query will have the format of:

SELECT (GET)
INSERT
UPDATE
DELETE
It has a specific syntax:

SELECT * FROM table;
INSERT INTO table_name(id, name) VALUES(1, 'Pacific Ocean');
UPDATE ...
DELETE ...

# Task

Part I SQLtoCSV. We will start with the SQL format to CSV

Your function will receives a connection (an sqlite3 object from import sqlite3 which will be already connected), table_name. Your function will transform the content of table_name to CSV format and return it. (Columns separated by comma and rows separated by \n)

Part II CSVtoSQL Your function will transform the content to SQL format by creating the table_name and adding each row.

Part III a) You will use your function to convert the list of all volcanos from CSV to SQL.

b) You will use your function to convert the list of all fault lines from SQL to CSV. Data are inside the table named: fault_lines.

Technical specifications
Write two functions:

def sql_to_csv(database, table_name):
def csv_to_sql(csv_content, database, table_name):
1# sql_to_csv will receive two strings as parameters and return a string. the database is a filename where sql_to_csv will fetch the information. table_name is the table from the database file to fetch the information. your return value will be a CSV formatted string: "ColA,ColB,ColC\n1,2,3\n4,5,6\n"

2# csv_to_sql will receive three strings as parameters and return nothing. csv_content is a StringIO following the CSV format. the database is a filename where csv_to_sql will push the information. table_name is the table from the database file to insert the data.

DoYourJob libraries are not authorized. We won't list all of them. If you are not doing the sql request by yourself then you are using a "doyourjob library". An example is: sqlalchemy

# Installation & Usage
pip install sqlite3
pip install csv
pip install pandas

python my_ds_babel.py