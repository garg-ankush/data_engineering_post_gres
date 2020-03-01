## Goals:

A relational database gives Sparkify the ability to collect song and user activity data on their platform, and analyze usage. This database unlocks several key metrics such as top songs listened, time spent on the platform etc. 

## Database Design:

Database consists of 4 dimension tables, and 1 fact table normalized to 3NF, and constructed using star schema.

#### Database details below:

songplay_table_drop - Fact Table - records in log data associated with song plays i.e. records with page
user_table_drop - Dimension Table - users in the app
song_table_drop - Dimension Table - songs in music database
artist_table_drop - Dimension Table - artists in music database
time_table_drop - Dimension Table - timestamps of records in songplays broken down into specific units

#### ETL scripts used:

sql_querries.py - Details sql querries to create, insert and delete tables (if already existing)
etl.py - Details python functions that utilize sql_querries.py to insert data from log files into their respective tables
create_tables.py - Details python functions for setting up the database connection, create and drop tables


#### Execute project

Run create_tables.py to create a connection to the database
Run etl.py file to read data from song and log files, and insert data into their respective tables
