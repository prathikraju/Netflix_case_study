# Netflix Content Strategy Case Study

An exploratory data analysis on Netflix's Movies and TV Shows catalog, looking at how Netflix's content strategy breaks down by type, genre, country, and rating, and how it has shifted over time.

## About the Data

The dataset has 8,807 rows and 12 columns. Each row is one title on Netflix, either a movie or a TV show. The columns include show id, type, title, director, cast, country, date added, release year, rating, duration, listed in (genre), and description.

## What This Project Covers

- **Data cleaning**: fixed a column shift error in the rating field, converted date added to a real date format, and made informed decisions on how to handle missing values in director, cast, and country
- **Non graphical analysis**: counts and percentages for type, rating, genre, and country
- **Pre processing**: unnested columns like country and genre that had multiple values packed into a single cell
- **Univariate visuals**: countplots for type and rating, barplots for genre and country
- **Bivariate visuals**: type versus country, and type versus year over time
- **Duration analysis**: split movie minutes and TV show seasons apart, then built histograms and boxplots for both
- **Outlier check**: used the IQR method on movie duration and verified the shortest titles by hand
- **Insights and recommendations**: a full write up covering attribute ranges, distribution patterns, and a comment on every plot, followed by business recommendations

## Key Findings

- About 70 percent of the catalog is movies and 30 percent is TV shows, though TV shows have been slowly gaining ground since 2018
- Around 70 percent of titles are rated for teens or above, showing Netflix mainly targets older audiences
- International Movies, Dramas, and Comedies are the most common genres
- The United States and India lead in total titles, but South Korea and Japan stand out by leaning heavily toward TV shows instead of movies
- Most TV shows last only 1 or 2 seasons, while movie runtimes cluster around 90 to 100 minutes

## Files in This Repository

- `Netflix_Case_Study.ipynb` — the full analysis notebook, from data loading through insights
- `netflix.csv` — the dataset used
- `Netflix_Case_Study_Report.docx` — a written report covering the process, findings, and recommendations

## Tools Used

Python, pandas, matplotlib, seaborn, Jupyter Notebook
