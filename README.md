# Chess.com
This project aims to extract data from chess.com APIs with a python script. 
The data is then sent to a Data Lake in the form of three json files. 
As soon as the data is loaded into the Data Lake, it is ingested into an SQS Queue and then sent to a Snowflake Data Warehouse via a Snowpipe Pipeline. 
Finally, the data is analysed with SQL queries in the Snowflake tables. The execution of the script is orchestrated by Airflow to operate every hour.
