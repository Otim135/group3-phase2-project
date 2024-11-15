# MOVIES ANALYSIS
## 1.0	Overview
Our company sees all the big companies creating original content and wants to join the fun. A decision has been made to create a new movie studio, but the company doesn’t know anything about creating movies. Our team has been tasked with exploring what types of films are currently doing the best at the box office. We must then translate those findings into actionable insights that the head of the company’s new movie studio can use to help decide what type of films to create.

## 2.0	Business Understanding
The movie-making industry is a complex, multi-billion-dollar global market that includes the development, production, distribution, and exhibition of films. This industry operates at the intersection of art, entertainment, and commerce, primarily producing films that attract audiences and generate substantial revenue.
### 2.1. Industry Context
The movie-making industry includes major film studios, production companies, and a vast network of support services such as talent agencies, production equipment suppliers, and post-production services. It is also heavily influenced by technological advancements, evolving customer preferences, and global marketing dynamics.

Revenue in the movie industry is derived from multiple sources as below:

- Box Office Sales – the primary revenue from ticket sales in theatres
  
- Streaming Platforms – services like Netflix
  
- Home Entertainment – includes digital purchases

### 2.2. Business Objective
The project analyzes select movie industry data, including audience preferences (IM.Db ratings) and financial performance (e.g. budgets and revenue) to make informed decisions that maximize profitability and audience satisfaction. This will also allow the company to derive actionable insights for the movie studio business.

Analyzing the identified data sources helps us determine which genres, storylines, and themes resonate most with audiences. This information can guide the studios in selecting projects more likely to succeed critically and commercially.

By studying ratings and reviews, producers can tailor content to specific age groups, cultural backgrounds, and other demographics that show high interest in certain types of movies.

We will see how analyzing financial data helps studios understand how budget size correlates with box office revenue. These insights can assist in deciding whether a high-budget blockbuster or a smaller film is a better investment for a particular market.

Our analysis will focus on the following objectives:

  1.	Identify Popular Genres: Analyze which genres tend to have higher ratings, more viewer engagement, high audience ratings, and are most profitable.

  2.	Analyze Characteristics of High-Rated Movies: Examine factors such as runtime, year of release, and genre combinations to see if they correlate with higher ratings.

  3.	Determine Key Contributors: Identify directors, writers, and actors who have contributed to successful movies, as potential partners for the new studio.

  4.	Investigate Trends Over Time: Look at how preferences in ratings, movie length, and genres have evolved over the years, highlighting trends that may be valuable for         the new studio to consider.

  5.	Correlate financial performance with popularity and ratings.

  6.	Offer genre and studio strategies for maximum ROI.

## 3.0	Data Sources and Understanding
We work with the following datasets:

 - IMDb Database: Contains movie ratings, genres, and key details.

 - TMDb Dataset: Includes popularity metrics, audience ratings, and genre encodings.

 - Budget Dataset: Provides production budgets, domestic and worldwide revenue.

The datasets will be merged using movie titles and release years.

Key Questions for Data Understanding:

 - What is the distribution of genres in the dataset?

 - Are there missing values in critical columns (e.g., ratings, genres, runtime)?

 - How are ratings distributed across movies?

 - What are the relationships between tables that can help us analyze contributor impact (e.g., directors, writers)?

## 4.0	Data Preparation
Steps:
  1.	Backing up of the data to avoid accidental loss during the data cleaning.
  
  2.	Understanding the data by reviewing the structure, and checking for data types, and constraints in the database. We also look at formatting and key relationships between tables.

  3.	We identify and remove duplicate records to reduce redundancy using methods such as DISTINCT in SQL or functions in data processing tools like Pandas (drop_duplicates()).

  4.	We then identify missing data points (NULL or NaN values) and decide on how to handle them: remove, replace with default values, or use statistical methods (e.g., mean, median, mode).
 
  5.	We structural errors by identifying issues with naming inconsistencies, typos, or formatting issues (e.g., Sci-Fi vs.SciFI). Therefore, standardizing naming conventions and formats.

  6.	Removing columns or rows that are not relevant to our analysis

  7.	Fix data type mismatches by ensuring each column has the correct data type (e.g., dates stored as DateTime objects, numbers stored as int or float). Then convert   types as necessary for consistency.

  8.	Standardize formatting; capitalization, and number precision to uniformity (e.g., changing all entries to lowercase or uppercase).

  9.	Identifying outliers using statistical methods and deciding on how to handle them: correct, sap, or remove them based on context.
 
  10.	Check referential integrity by verifying that the relationship between tables is maintained (e.g., foreign keys pointing to existing primary keys).

## 5.0	Modelling/ Analysis

The analysis includes several statistical and visualization techniques to uncover insights:

Univariate Analysis: Examining the distribution of single variables, such as production budgets and gross revenue, through histograms and summary statistics.

Correlation Analysis: Exploring relationships between financial variables to understand associations (e.g., production budget vs. worldwide gross).

Regression Analysis: Modeling the relationship between production budgets and worldwide gross to predict potential revenue.

Genre and Studio Analysis: Identifying top-performing genres and studios and examining their financial impact.

Multivariate Analysis: Combining multiple factors (budget, genre, year) to analyze financial outcomes using heatmaps, scatter plots, and regression models.

### 5.1. Visualizations
The following visualizations are included in this analysis:

Bar Charts: Showing movie count by genre and studio to highlight popularity and distribution.

Line Plots: Illustrating trends over time in production budgets and gross revenue.

Correlation Heatmap: Displaying relationships between key financial metrics.

Box Plots: Highlighting the spread and outliers in production budgets across genres.

Tree Maps: Visualizing the contribution of various genres or studios to overall revenue.

Histograms: Showing the distribution of average votes to understand movie ratings.

### Key Findings

Some insights uncovered during the analysis:

1. Genres like Action and Adventure are often associated with higher budgets and revenue.

2. Production budget has a positive correlation with worldwide gross, though other factors also play a significant role in profitability.

3. Studios with high output (e.g., Warner Bros, Universal Pictures) tend to dominate in revenue, but not always in ROI, indicating varied profitability.

### Pre-requisites:

Python libraries: pandas, matplotlib, seaborn, statsmodels

Tableau Public for interactive visualizations: https://public.tableau.com/app/profile/moses.musyoki/viz/cleaned_df/Dashboard1

### Instructions

- Clone this repository:

- bash

- Copy code

- git clone <[repository-url](https://github.com/Otim135/group3-phase2-project/tree/main)>

- Run financial_analysis.ipynb in Jupyter Notebook or any other compatible IDE.

- Use Tableau Public to create additional visualizations by importing movies.csv.

## 6.0 Conclusion

## 7.0 Recommendation

