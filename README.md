# Movies-ETL
## Overview
The Movies-ETL process is the first step in preparing for a hackathon in which an algorithm will be developed to predict low-budget movies being released will become popular. Unfortunately, the dataset available for the hackathon is untidy and located multiple sources. In the Movies-ETL project, we extract data from both Wikipedia and Kaggle, transform the data, merge them and load the merged data to a SQL database so that the hackathon participants have a nice, clean dataset to use. To do this, we will follow the ETL process:
  * Extract the Wikipedia and Kaggle data from their respective files.
  * Transform the datasets by cleaning them up and joining them together.
  * Load the cleaned dataset into a SQL database.
We will extract scraped Wikipedia data stored as JSON and the Kaggle data stored in CSV in the Extract phase. In the Transform phase, we will utilize Python and Pandas in a Jupyter Notebook. We will use Python and Pandas to explore, document, and perform our data transformation. Finally, after the data is transformed into a consistent structure, it's loaded into the PostgreSQL database.

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






