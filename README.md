# ETL for Movie Data: A Comprehensive Data Pipeline

![CI](https://github.com/ksdisch/Movies-ETL/workflows/CI/badge.svg)

As an accomplished data professional, I am proud to showcase this ETL (Extract, Transform, Load) project. The purpose of this project is to efficiently extract data from sources like Wikipedia, Kaggle, and MovieLens, transform and clean it into a usable format, and finally load it into a database, ready for advanced analysis.

## Project Overview

This script is designed to perform an end-to-end ETL process, involving various stages of data cleaning, transformation, and loading. The outcome is a cleaned, transformed, and well-structured dataset derived from diverse sources that can be utilized for further in-depth analysis and potential machine learning applications.

## Skills Utilized

* **Data Extraction**: Efficiently extract data from JSON and CSV formats, utilizing libraries such as Pandas.
* **Data Cleaning**: Implemented comprehensive cleaning functions to handle missing values, correct data types, filter out irrelevant data, and manage data inconsistencies.
* **Data Transformation**: Demonstrated proficiency in transforming unstructured data into a structured format using Python and associated libraries.
* **Data Loading**: Loaded cleaned and transformed data into a database, ready for analysis or for use in machine learning models.

## Project Components

1. `clean_movie()`: A function that deals with alternative titles and merges columns with similar data in the movie data extracted from Wikipedia.
2. `extract_transform_load()`: The main function that performs the entire ETL process. It does the following:
    * Reads in Kaggle metadata and MovieLens rating data as Pandas DataFrames, along with Wikipedia data as a JSON object.
    * Filters out TV shows from the Wikipedia data and applies `clean_movie()` function to this data.
    * Further cleans the Wikipedia data by handling missing values, parsing box office, budget, release date, and running time data.
    * Cleans the Kaggle data by filtering out adult movies, correcting data types, and converting timestamps to datetime format.
    * Merges the cleaned Wikipedia and Kaggle dataframes, drops unnecessary columns, fills missing Kaggle data with Wikipedia data, and renames columns for better organization.
    * Transforms and merges the ratings data from MovieLens to the combined movies dataframe.

## Technologies Used

* Python: The main programming language used for writing the ETL script.
* Pandas: A powerful Python library used for data manipulation and analysis.
* PostgreSQL: An advanced, open-source relational database system used for storing the final structured data.
* pgAdmin4: The most popular administrative and management tool for PostgreSQL, used for managing the database and executing SQL queries.

## Data Sources

* wikipedia-movies.json
* ratings.csv
* movies_metadata.csv

Take a look around the repository to get an understanding of my technical capabilities and this project's full potential. Enjoy!
