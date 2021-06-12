# Movies-ETL

## Overview

The purpose of this project was to gather movie data from Wikipedia and Kaggle. Then, we were to combine the data and save them into a SQL database. To do this, we will have to Extract, Transform, and Load the data.

## ETL_function_test.ipynb

This file shows the process of extracting data from Wikipedia and Kaggle. We first extract the Wikipedia data into a JSON file and then we read that into a Pandas DataFrame. Similarily, we extract the Kaggle data by downloading the csv files we are interested in. Then we read these csv files into a Pandas DataFrame. 

## ETL_clean_wiki_movies.ipynb

This file shows the process of transforming the Wikipedia data. In this file, we cleaned the Wikipedia data by removing or altering certain columns. We used regular expressions and lamdba functions to do this. We also added a function to standardize the values for both the budget and box office columns. After this step, the Wikipedia data was ready to merge with another DataFrame. 

## ETL_clean_kaggle_data.ipynb

This file shows the process of transforming the Kaggle data. We cleaned this dataset by removing columns and converting data types of several columns. Then, we merged the data with the Wikipedia DataFrame. We then dropped any redundant columns and filled in null values. We then reordered and renamed the columns in the new DataFrame. We also transformed and merged the ratings dataset as well. 

## ETL_create_database.ipynb

This file shows the process of loading the cleaned data into a SQL database. We added a database connection string and created a database engine. Then we imported the data to PostgreSQL and verified that it was completed.
