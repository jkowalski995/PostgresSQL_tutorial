# PostgreSQL with Python
This is a little tutorial for working with PostgreSQL in Python. \
It is based on https://www.postgresqltutorial.com 

## connect.py
 - source: https://www.postgresqltutorial.com/postgresql-python/connect/ 
    
   - How it works:
     - First, read database connection parameters from the database.ini file. 
     - Next, create a new database connection by calling the connect() function. 
     - Then, create a new cursor and execute an SQL statement to get the PostgreSQL database version. 
     - After that, read the result set by calling the  fetchone() method of the cursor object. 
     - Finally, close the communication with the database server by calling the close() method of the cursor and connection objects.

## config.py
 - source: https://www.postgresqltutorial.com/postgresql-python/connect/ 
   - How it works:
     - First, import Parser
     - Next, in database.ini search for postgresql section
     - Finally, read a configuration

## create_table.py
 - source: https://www.postgresqltutorial.com/postgresql-python/create-tables/ 
   - How it works:
     - First, construct CREATE TABLE statements. 
     - Next, connect to the PostgreSQL database by calling the connect() function. The connect() function returns a connection object. 
     - Then, create a cursor object by calling the cursor() method of the connection object. 
     - After that, execute the CREATE TABLE by calling the execute() method of the cursor object. 
     - Finally, close the communication with the PostgreSQL database server by calling the close() methods of the cursor and connection objects.
 
## insert_row.py and insert_many_rows.py and insert.py
 - source: https://www.postgresqltutorial.com/postgresql-python/insert/ 
   - How it works:
     - First, connect to the PostgreSQL database server by calling the connect() function of the psycopg module. 
     - Next, create a new cursor object by calling the cursor() method of the connection object. 
     - Then, execute the INSERT statement with the input values by calling the execute() or executemany() method of the cursor object. 
     - After that, use fetchone() to get returned value (in this case vendor_id). 
     - Next, commit changes to save them permanently into database.
     - Finally, close the communication with the PostgreSQL database server by calling the close() methods of the cursor and connection objects.
          
   #### insert.py is launching file for insert_row.py and insert_many_rows.py
