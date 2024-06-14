# Datasets2
# Netflix Shows Analysis

## Dataset Overview
The dataset contains information about various shows available on Netflix, including details like title, director, cast, country, date added, release year, rating, duration, listed genres, and descriptions.

## Import Process
The dataset was imported into MySQL Workbench using the following steps:
1. Created a table structure to match the dataset columns.
2. Loaded the CSV file into the table.
3. Converted data types where necessary to ensure compatibility.

## Difficulties
- Converting date formats and ensuring accurate data types for columns like `release_year` and `date_added`.
- Handling special characters in titles and descriptions.

## Interesting Finding
A significant number of shows are released around holiday seasons, which may suggest a strategy to capture holiday viewership.

## Cool Facts
1. The most common genre listed is "Documentaries."
2. The average release year of the shows is around 2016.

## Questions and Insights
1. **What is the most common genre?**
   - **Query**: `SELECT listed_in, COUNT(*) as count FROM netflix_shows GROUP BY listed_in ORDER BY count DESC LIMIT 1;`
   - **Insight**: Documentaries are the most common genre.
2. **What is the average release year of the shows?**
   - **Query**: `SELECT AVG(release_year) AS average_release_year FROM netflix_shows;`
   - **Insight**: The average release year is around 2016.

## Data Visualizations
1. **Number of Shows Released Each Year**
   - Bar chart showing the distribution of shows over the years.
2. **Distribution of Genres**
   - Pie chart depicting the percentage of each genre.
3. **Top 5 Most Popular Shows in the United States**
   - Bar chart listing the top 5 most popular shows.

## Summary
The project provided valuable insights into the Netflix dataset, revealing trends in show releases and genre popularity. The visualizations helped clarify these insights effectively.
