# Migrate data from Microsoft database to the Redshift
Script takes data from MS SQL and splits it in chunks.

Redshift doesn't have primary key. Scripts generated hist_id based on id and row number. Delete statment removes all the duplicates.

The last step is to insert multiple rows into Redshift. On conflict function ignores rows, which already exist in the database.

### Installing
pip3 install pyodbc
pip3 install psycopg2
pip3 install

### Libraries
* pyodbc
* psycopg2
* time
* math

### Running<br>
python3 curing_values.py
