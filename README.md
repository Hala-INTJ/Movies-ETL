# Challenge 8: Movies-ETL
## Overview of The Movies-ETL
This repository contains four jupyter notebooks:
- [ETL_function_test]()
Creating a function that reads in these three data files into three separate DataFrames:
* [wikipedia-movies.json]()
* [movies_metadata.csv]()
* [ratings.csv]()

- [ETL_clean_wiki_movies]()
Extracting and transforming the Wikipedia data [wikipedia-movies.json]() using regular expression strings and dropping duplicates, then converting the transformed data into a DataFrame.

- [ETL_clean_kaggle_data]()
Extracting and transforming the Kaggle metadata [movies_metadata.csv]() and MovieLens rating data [ratings.csv](), then converting the transformed data into separate DataFrames. Furthermore, the Kaggle metadata DataFrame is merged with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, the MovieLens rating data DataFrame is merged with the movies_df DataFrame to create the movies_with_ratings_df.

- [ETL_create_database]()
Adding the movies_df DataFrame and MovieLens rating CSV [ratings.csv]() to PostgreSQL into separate tables: movies and ratings.

| movie table | 
| ---------------- |
| ![]() | 
| The row count is ![]() |

| ratings table |
| ---------------- |
| ![]() |
| The row count is ![]() |


The loading of the ratings data was chuncked and the overal time to load into the database was measured.
![]()
