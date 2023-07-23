# MICROSOFT MOVIE STUDIO PROJECT
## 1. INTRODUCTION
<img src = 'denise-jans-tV80374iytg-unsplash.jpg'>

Photo from  <a href="https://unsplash.com/photos/tV80374iytg">Unsplash</a> By Denise Jans

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

## 6. DATA ANALYSIS RESULTS

### 6.1 Genres Analysis
In genre analysis I will explore the distribution of movies genre i.e,. to check which genres are the most popular, most profitable, and the genres with highest production budget.

#### 6.1.1. Most Popular Genres

<img src = 'Images/most popular languages.png'>

The five most popular genres are Drama, Comedy, Action, Adventure & Thriller.

#### 6.1.1. Most Profitable Genres

<img src = 'Images/most profitable genres.png'>

The 5 most profitable genres are: Adventure, Action, Comedy, Drama and Sci-Fi

### 6.2 Month of release analysis

#### 6.2.1. Month with the highest profits

<img src = 'Images/month_of_release vs profit.png'>

The top 5 months the highest profit are June, November, July, December & May.

### 6.3 Language analysis

#### 6.3.1. Most Popular Languages

<img src = 'Images/most popular languages.png'>

The top 5 most popular languages are English, Danish, Telugu, Korean and Hindi.

#### 6.3.2. Most Profitable languages

<img src = 'Images/most profitable languages.png'>

The 5 most profitable languages are: Thai, Telegu, English, Hungarian and Hindi.

### 6.4 Correlation Analysis

#### 6.4.1. Correlation between all the columns

<img src = 'Images/Correlation using Heatmap.png'>

We have positive correlation between all the variables but varying in terms of strength.

##### Variables with strong positive correlation are:

1.production_budget and profit with a correlation of 0.662025.

2.popularity and production_budget with a correlation of 0.527787.

3.popularity and profit with a correlation of 0.521680.

##### Variables with weak positive correlation are:

1. averagerating and runtime_minutes with a correlation of 0.405544.

2. production_budget and runtime_minutes with a correlation of 0.354355.

3. popularity and runtime_minutes with a correlation of 0.318119.

4. averagerating and popularity with a correlation of 0.294996.

5. runtime_minutes and profit with a correlation of 0.276521.

6. averagerating and profit with a correlation of 0.258633.

7. averagerating and production_budget with a correlation of 0.144862.

#### 6.4.1. Relationship Between Production Budget and Total gross


<img src = 'Images/production budget vs profit.png'>

The relationship between production budget and profit is a positive one. This implies that as the production budget increases, the profit tends to increase, but the relationship is not very strong.

## 7. DATA ANALYSIS RESULTS

#### 7.1 What types of movie genres are doing the best at the box office?
After analyzing movie genres in terms of popularity, profitability, and budget, I found that Drama, Comedy, Action, and Adventure movies emerged as the most popular and profitable genres.

#### 7.2 Which languages are doing the best at the box office ?
Based on the analysis of original languages in terms of popularity, profitability, and rating, I found that English emerged as the most popular language, followed by Danish and Telegu. In terms of profitability, Thai, Telegu, and English were the top three languages. Finally, the highest-rated languages were German, Telegu, and English.

#### 7.3 Does release month affect profit ?
Yes, the months with the highest movie profits are June, May, July, November, and December. This can be attributed to School Holidays and Festive seasons in this months.

#### 7.4 Is there a correlatoon between production budget and profit ?
Yes. There a positive correlation between production budget and profit. This implies that as the production budget increases, profit also increases. Higher production budgets are associated with higher profits.


## 8. RECOMMENDATION

1. The best types of films to create are Drama, Comedy, and Action
2. The best languages for this films are English, Thai, Telegu
3. The best months to release the films are June, November and July.
4. For a successful new movie studio, Microsoft should invest in both production budget and marketing. This approach will enhance film quality and promotes broader audience reach, increasing the likelihood of success and profitability.


## GUIDE

The data used for the project can be found here https://github.com/willieki/Microsoft_movie_project/tree/master/DATA

The images from EDA can be found here https://github.com/willieki/Microsoft_movie_project/tree/master/Images

The notebook that contains the project can be found here https://github.com/willieki/Microsoft_movie_project/blob/master/student.ipynb

The presentation for this project can be found here https://github.com/willieki/Microsoft_movie_project/blob/master/presentation.pdf