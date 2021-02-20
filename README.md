# Challenge 8: Movies-ETL
## Overview of The Movies-ETL
This repository contains four jupyter notebooks:
- [ETL_function_test](https://github.com/Hala-INTJ/Movies-ETL/blob/main/ETL_function_test.ipynb)<br/>
Creating a function that reads in these three data files into three separate DataFrames:
    * [wikipedia-movies.json](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/wikipedia-movies.json)
    * [movies_metadata.csv](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/movies_metadata.csv)
    * [ratings.csv]()

- [ETL_clean_wiki_movies](https://github.com/Hala-INTJ/Movies-ETL/blob/main/ETL_clean_wiki_movies.ipynb)<br/>
Extracting and transforming the Wikipedia data [wikipedia-movies.json](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/wikipedia-movies.json) using regular expression strings and dropping duplicates, then converting the transformed data into a DataFrame.

- [ETL_clean_kaggle_data](https://github.com/Hala-INTJ/Movies-ETL/blob/main/ETL_clean_kaggle_data.ipynb)<br/>
Extracting and transforming the Kaggle metadata [movies_metadata.csv](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/movies_metadata.csv) and MovieLens rating data [ratings.csv](), then converting the transformed data into separate DataFrames. Furthermore, the Kaggle metadata DataFrame is merged with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, the MovieLens rating data DataFrame is merged with the movies_df DataFrame to create the movies_with_ratings_df.

- [ETL_create_database](https://github.com/Hala-INTJ/Movies-ETL/blob/main/ETL_create_database.ipynb)<br/>
Adding the movies_df DataFrame and MovieLens rating CSV [ratings.csv]() to PostgreSQL into separate tables: movies and ratings.

| movies table | 
| ---------------- |
| ![](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/movies_query_sample.png) | 
| ![](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/movies_query.png) |

| ratings table |
| ---------------- |
| ![](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/ratings_query_sample.png) |
| ![](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/ratings_query.png) |


The loading of the ratings data was chuncked and the overal time to load into the database was measured.
![](https://github.com/Hala-INTJ/Movies-ETL/blob/main/Resources/Loading%20ratings%20data_%20elapsed%20time.png)
