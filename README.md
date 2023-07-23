# MICROSOFT MOVIE STUDIO PROJECT
## 1. INTRODUCTION
<img src = 'images/samuel-regan-asante-wMkaMXTJjlQ-unsplash-1.jpg'>

Photo from  <a href="https://unsplash.com/photos/q8P8YoR6erg">Unsplash</a>

### 1.1 Project Overview
To use Explanatory Data Analysis(EDA) to generate actionable insights to the head of Microsoft's new movie studio, that he/she can use to decide what type of films to create.

### 1.2 BUSINESS UNDERSTANDING
Microsoft has noticed that many major companies are successfully creating original video content, and they want to join the excitement. To do so, they have made the bold decision to establish a new movie studio. However, Microsoft lacks experience in the film industry, leaving them uncertain about the types of movies that perform best at the box office. Thus, they seek to explore and analyze the current trends and successful genres in the movie industry.

Project Objective:

The main objective of this project is to conduct thorough research and analysis on the types of films that are currently enjoying the greatest success. These findings will play a crucial role in guiding the decision-making process, helping Microsoft determine the most promising genres for their upcoming movie projects.

In order to make recommendations, this analysis is going to explore some questions which are:

1. What types of films are doing the best at the box office?

2. Which languages are doing the best at the box office?

3. Does Release month affect profit?

4. Is there a correlation between production budget and profit generated?

## 2. DATA UNDERSTANDING

The data sources for this analysis will be pulled from five separate files:

1. #### `bom.movie_gross.csv`

   A csv file with the following columns: Movie title, studio, domestic_gross, foreign_gross & year of release.
   
2. #### `title.basics.csv`

   A csv file with the following columns: tconst(unique identifier of the movie titles), primary_title, original_title,     start_year, runtime_minutes, genres.

3. #### `title.ratings.csv`
   A csv file with the following columns: tconst(unique identifier of the movie titles), averegarating, numvotes.

4.  #### `tmdb.movies.csv`
    A csv file with the following columns: genre_ids, Id, original_language, original_title, popularity, release_date, title, vote average, vote_count.

5.  #### `tn.movie_budgets.csv`
    A csv file with the following columns: Id, release_date, movie, production_budget, domestic_gross.

All the files are stored in a folder called data.

## 3. IMPORTING NECESSARY LIBRARIES
Load the libraries required for the analysis i.e pandas, numpy, matplotlib, and seaborn.

## 4. EXPLORING DATAFRAMES
Explore the dataframe to get more information about each dataframe.By checking for any missing values, the shape of each dataset, and the descriptive statistical summary.

## 5. DATA CLEANING
Data cleaning involves the preparation of data for analysis by removing irrelevant or incorrect information that could adversely impact the performance of models or algorithms. It includes identifying and handling missing values, correcting incorrect data, and reducing duplicates. 
I analysed each dataset separately because I have 5 different dataframes.

## 5. DATA ANALYSIS RESULTS

### 6.1 Genres Analysis
In genre analysis I will explore the distribution of movies genre i.e,. to check which genres are the most popular, most profitable, and the genres with highest production budget.

#### 6.1.1. Most Popular Genres

<img src = 'images/most popular languages.png'>

The five most popular genres are Drama, Comedy, Action, Adventure & Thriller.

#### 6.1.1. Most Profitable Genres

<img src = 'images/most profitable genres.png'>

The 5 most profitable genres are: Adventure, Action, Comedy, Drama and Sci-Fi
































