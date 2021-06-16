# Movies-ETL
## Overview
The Movies-ETL process is the first step inparing for a hackathon which 
In the Movies-ETL project, we our extract data from two data sources, transform the data, merge them and load the merged data in a database. from both Wikipedia and Kaggle, combine them, and save them into a SQL database so that the hackathon participants have a nice, clean dataset to use. To do this, she will follow the ETL process: extract the Wikipedia and Kaggle data from their respective files, transform the datasets by cleaning them up and joining them together, and load the cleaned dataset into a SQL database. In the Extract phase, data is pulled from external or internal sources, possibly disparate. you'll extract scraped Wikipedia data stored as a JSON, and Kaggle data stored in CSVs.
In the Transform phase, The transformation phase can be accomplished with Python and Pandas, pure SQL, or specialized ETL tools like Apache Airflow or Microsoft SQL Server Integrated Services (SSIS). Python and Pandas are especially good for prototyping an ETL transformation because they provide flexibility and interactivity (especially in a Jupyter Notebook), without enforcing any complicated frameworks. We will use Python and Pandas to explore, document, and perform our data transformation.
Finally, after the data is transformed into a consistent structure, it's loaded into the data target. Britta has determined that a SQL database is the best solution for sharing the data in the hackathon, so we'll be loading our data into a PostgreSQL table.

## Control Flow
1. Extract the Wikipedia Movies JSON
  2. Load the JSON into a List of Dictionaries
  3. Inspect the data
4. Extract the Kaggle Data
  5. Inspect the data
