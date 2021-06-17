# Movies-ETL
## Overview
The Movies-ETL process is the first step in preparing for a hackathon in which 
In the Movies-ETL project, we our extract data from two data sources, transform the data, merge them and load the merged data in a database. from both Wikipedia and Kaggle, combine them, and save them into a SQL database so that the hackathon participants have a nice, clean dataset to use. To do this, she will follow the ETL process: extract the Wikipedia and Kaggle data from their respective files, transform the datasets by cleaning them up and joining them together, and load the cleaned dataset into a SQL database. In the Extract phase, data is pulled from external or internal sources, possibly disparate. you'll extract scraped Wikipedia data stored as a JSON, and Kaggle data stored in CSVs.
In the Transform phase, The transformation phase can be accomplished with Python and Pandas, pure SQL, or specialized ETL tools like Apache Airflow or Microsoft SQL Server Integrated Services (SSIS). Python and Pandas are especially good for prototyping an ETL transformation because they provide flexibility and interactivity (especially in a Jupyter Notebook), without enforcing any complicated frameworks. We will use Python and Pandas to explore, document, and perform our data transformation.
Finally, after the data is transformed into a consistent structure, it's loaded into the data target. Britta has determined that a SQL database is the best solution for sharing the data in the hackathon, so we'll be loading our data into a PostgreSQL table.

## Control Flow
1. Extract the Wikipedia Movies JSON
2. Load the JSON into a List of Dictionaries
3. Inspect the data
4. Extract the Kaggle Data
5. Inspect the data
6. Design a Inspect, Plan, and Execute process for the Wikipedia data
   * Inpspect:  inspect our data and identify a problem
   * Plan: make a plan and decide whether it is worth the time and effort to fix it.
   * Execute: execute the repair
 7. Load the Wiki data to a DataFrame to inspect the columns
 8. Filter unwanted columns
 9. Write a function to inspect, clean, and consolidate column names
 10. Remove duplicate rows
 11. Remove Mostly Null Columns
 12. Make a Plan to Convert and Parse the data in numeric and datetime columns
 13. Design a Inspect, Plan, and Execute process for the Kaggle data
 14. Remove bad data
 15. Merge Wikipedia and Kaggle Metadata
 16. Remove redundant columns
 17. Transform and Merge Rating Data
 18. Connect Pandas and SQL

## Results
After the entire ETL process, we successfully reduced 191 messy columns down to 21 useful, data-filled columns. Similarly we reduced 7311 rows to 6052.

##### Wikipedia Cleaned Data
![wiki_movies_df](https://user-images.githubusercontent.com/67847583/122300112-7d896400-cec4-11eb-9659-34df646fab8b.png)
##### Merged Data with Ratings
![movies_with_ratings_df](https://user-images.githubusercontent.com/67847583/122300124-82e6ae80-cec4-11eb-9304-52c384edc05c.png)
##### Wikepedia Movies and Kaggle Metadata
![movies_df](https://user-images.githubusercontent.com/67847583/122300149-8aa65300-cec4-11eb-98f9-413fbb9da353.png)
##### Transformed Data in SQL Database
![movies_query](https://user-images.githubusercontent.com/67847583/122300175-91cd6100-cec4-11eb-8ed1-b6cfbb941bde.png)
##### Ratings Data in SQL Database
![ratings_query](https://user-images.githubusercontent.com/67847583/122300181-942fbb00-cec4-11eb-9b64-e1af1f9f3d7d.png)






