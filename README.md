# 📊 Netflix Movies & TV Shows Analysis Using SQL

![Netflix Logo](https://github.com/najirh/netflix_sql_project/blob/main/logo.png)

## 🚀 Project Overview

This project dives deep into Netflix’s catalog of movies and TV shows using **SQL** to uncover meaningful insights. The analysis addresses several business questions, helping to understand content distribution, trends, and patterns that can influence strategic decisions.

---

## 🎯 Objectives

- Analyze the distribution between movies and TV shows.
- Identify the most common content ratings.
- Examine content trends by release year, country, and duration.
- Explore genres and keyword-based content categorization.

---

## 📂 Dataset

- **Source:** [Kaggle Netflix Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows?resource=download)
- The dataset includes information like titles, types, directors, casts, countries, dates added, release years, ratings, durations, genres, and descriptions.

---

## 🗄️ Database Schema

```sql
DROP TABLE IF EXISTS netflix;
CREATE TABLE netflix
(
    show_id      VARCHAR(5),
    type         VARCHAR(10),
    title        VARCHAR(250),
    director     VARCHAR(550),
    casts        VARCHAR(1050),
    country      VARCHAR(550),
    date_added   VARCHAR(55),
    release_year INT,
    rating       VARCHAR(15),
    duration     VARCHAR(15),
    listed_in    VARCHAR(250),
    description  VARCHAR(550)
);
