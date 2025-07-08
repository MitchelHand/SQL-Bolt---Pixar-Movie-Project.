# SQL Bolt Project: Pixar Movies Data Analysis

## Overview

This repository features solutions to the SQL Bolt challenges, specifically focusing on the "Pixar Movies" dataset. This project demonstrates practical SQL querying skills for data retrieval, joining multiple tables, and ordering data to gain insights into movie characteristics, sales performance, and audience ratings.

## Objective

The primary objective of this project was to successfully complete a series of SQL tasks using the `movies` and `boxoffice` tables. Each task required precise data extraction and manipulation to answer specific questions about Pixar films, their sales figures, and critical reception.

## Key Skills Demonstrated

* 🐍 **SQL Querying:** Fundamental to intermediate SQL syntax for data selection.
* 🐼 **Database Joins:** Proficient use of `JOIN` clauses to combine data from multiple related tables (e.g., `movies` and `boxoffice`).
* ⚙️ **Data Filtering:** Applying `WHERE` clauses to specify conditions for data retrieval.
* 📊 **Data Ordering:** Utilizing `ORDER BY` to sort results based on numerical (e.g., `Rating`, `Domestic_sales`, `International_sales`) criteria.
* 🎯 **Data Comparison:** Identifying records based on comparative values (e.g., international sales greater than domestic sales).
* 📈 **Data Interpretation:** Deriving insights from movie data, including sales trends and audience preferences.

## Project Exercises & Insights

The following tasks were successfully completed, showcasing a range of SQL techniques:

### 1. Find the domestic and international sales for each movie.

**SQL Syntax (Example Query Structure):**
```sql
SELECT
    movies.title,
    boxoffice.domestic_sales,
    boxoffice.international_sales
FROM
    movies
JOIN
    boxoffice ON movies.id = boxoffice.movie_id;
```

**Technique:** `INNER JOIN` on `movies.id` and `boxoffice.movie_id` to link movie titles with their sales figures.
**Insight:** This fundamental join operation is critical for combining related information stored across different tables, providing a complete view of each movie's financial performance.

### 2. Show the sales numbers for each movie that did better internationally rather than domestically.

**SQL Syntax (Example Query Structure):**
```sql
SELECT
    movies.title,
    boxoffice.domestic_sales,
    boxoffice.international_sales
FROM
    movies
JOIN
    boxoffice ON movies.id = boxoffice.movie_id
WHERE
    boxoffice.international_sales > boxoffice.domestic_sales;
```

**Technique:** `WHERE` clause with a comparison operator (`>`) to filter results based on a specific sales condition.
**Insight:** Demonstrates the ability to filter data based on calculated or comparative metrics, identifying movies with stronger international market appeal.

### 3. List all the movies by their ratings in descending order.

**SQL Syntax (Example Query Structure - as seen in screenshot):**
```sql
SELECT title, rating
FROM movies
JOIN boxoffice ON movies.id = boxoffice.movie_id
ORDER BY rating DESC;
```

**Technique:** `ORDER BY` clause with `DESC` to sort results from highest to lowest rating.
**Insight:** Essential for ranking and prioritizing data, in this case, identifying the most critically acclaimed or highly rated films.

## Tools and Environment

* 💻 **SQL Bolt Platform:** The project was completed using the interactive SQL Bolt learning environment, which provides a hands-on experience with SQL syntax and database concepts.
* 📝 **SQL (Structured Query Language):** The core language used for all data interactions and problem-solving.
* 🎬 **Pixar Movies Dataset:** Experience working with a structured dataset comprising movie details and box office performance.

## Conclusion

This SQL Bolt project highlights my foundational and practical SQL skills, particularly in querying, joining, filtering, and ordering data within a relational database. My ability to interpret requirements and translate them into efficient SQL queries is a valuable asset for any data-focused role.

---
![unnamed](https://github.com/user-attachments/assets/7350b0c7-7a2a-4f67-b459-a2cb38d53cf7)


