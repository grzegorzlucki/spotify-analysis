# Spotify Analysis

**Data Source:** [Top Spotify Songs 2023 on Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023)

## Overview

This repository contains an in-depth analysis of the Top Spotify Songs dataset for the year 2023. The analysis explores various aspects of the data, including data cleaning, exploratory data analysis, statistical tests, and machine learning modeling.

## Analysis Steps

### 1) Data Cleaning:
- Removed rows with invalid or missing values in specific columns (`in_deezer_playlists`, `in_shazam_charts`, `streams`).
- Cleaned and transformed data types of columns.
- Handled missing values in the `mode` column.
- Converted categorical values in the `key` column into numerical representation.

### 2) Exploratory Data Analysis:
- Calculated summary statistics of the dataset, including mean, standard deviation, and quartiles.
- Conducted Shapiro-Wilk tests to check the normality of certain variables (`in_spotify_playlists`, `streams`, `bpm`).
- Visualized distributions of variables using histograms and density plots.

### 3) Statistical Analysis:
- Tested correlation between `in_spotify_playlists` and `streams` using the Spearman rank correlation coefficient due to non-normal distributions.
- Checked correlation between `bpm` and `streams`.

### 4) Machine Learning Model:
- Utilized a Random Forest Classifier to predict the `mode` of the songs based on other attributes.
- Split the data into training and testing sets.
- Achieved an accuracy score of approximately 62% on the test data.
