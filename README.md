# Project: Movie and Genre Analysis Over The Last 50 Years

<img src="assets/banner.gif" alt="banner" width="600">

**Team Members:** Mustapha, Zakir, Tea, Reyhane

## Table of Contents 📑

- [Project Overview](#project-overview)
- [Objectives 🎯](#objectives)
- [Data Description 📈](#data-description)
- [Software Used 💻](#software-used)
- [Data Cleaning 🧹](#data-cleaning)
- [Findings 🔍](#findings)
- [Conclusion 🎯](#conclusion)

---

<h2 id="project-overview">Project Overview</h2>
Movies hold a unique place in our cultural narrative, reflecting trends and shaping entertainment industries. This project investigates the performance of movie genres at the box office, focusing on key drivers of success, profitability patterns, and cultural influences over the past five decades.

[Explore the Looker Studio Report](https://lookerstudio.google.com/embed/reporting/f09a73c4-f328-4de2-8110-eddebb49830c/page/p_2snmvyv2ld)

---

<h2 id="objectives">Objectives 🎯</h2>

Our project sought to address these key questions:

- What genres yield the highest revenue? 💰
- How has the popularity of genres evolved over time? 📅
- Which countries are major contributors to movie distribution? 🌍
- How have box office revenues fluctuated over the years? 📈
- What production companies dominate in revenue generation? 🎬
- What seasonal patterns influence movie profitability? 📅💸
- How does each genre balance risk and reward? ⚖️
- How do cultural factors impact movie performance? 🧠
- What role do marketing strategies play in box office success? 📢

---

<h2 id="data-description">Data Description 📈</h2>

We utilized the following data sources for analysis:

1. **TMDB Movies Dataset (2024 Edition)**:  
   A detailed dataset provided by [Asaniczka on Kaggle](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies), containing 1,000,000 movies with attributes such as titles, genres, release dates, ratings, revenue, and budget.

2. **US Box Office Data**:  
   Extracted from [BoxOfficeMojo](https://www.boxofficemojo.com/chart/ww_top_lifetime_gross/), offering insights into weekly and total gross earnings.

3. **Barbenheimer Marketing Insights**:  
   Sourced from [Comscore](https://www.comscore.com/Insights/Blog/Barbenheimer-and-Redefining-Movie-Marketing-Strategies), analyzing the successful marketing campaigns for *Barbie* and *Oppenheimer*.

---

<h2 id="software-used">Software Used 💻</h2>

The following tools were employed in our analysis:

- **Python** (Google Colab) 🐍
- **pandas** 🧑‍💻
- **numpy** 🔢
- **matplotlib** 📊
- **plotly.express** 📈
- **seaborn** 📉
- **BigQuery** 🗃️
- **Looker** 📊

---

<h2 id="data-cleaning">Data Cleaning 🧹</h2>

To prepare the data for meaningful analysis, we undertook the following cleaning steps:

1. **Filtered Out Adult Content**:  
   Excluded adult-oriented movies to maintain relevance.

2. **Dropped Redundant Columns**:  
   Removed unnecessary fields like `Spoken_languages`, `original_title`, and `imdb_id`.

3. **Kept Only English-Language Films**:  
   Focused the analysis on English-language movies for global consistency.

4. **Limited Data to the Last 50 Years**:  
   Isolated movies released in the last five decades to align with modern trends.

5. **Managed Missing Data**:  
   - Removed records with null values in critical fields: `title`, `revenue`, `vote_count`, and `budget`.  
   - Filled missing `production_companies` and `country` fields with 'unspecified'.

6. **Handled Duplicate Data**:  
   Eliminated conflicting duplicates, such as different versions of the same movie.

7. **Merged Title and Year Columns**:  
   Combined `title` and `release_year` for better identification of movies with similar titles.

8. **Addressed Missing Genres**:  
   Substituted missing genre data with 'other' to preserve completeness.

9. **Split Genres into Separate Columns**:  
   Encoded the `genres` column, creating binary columns to represent genre presence.

10. **Expanded Rows for Multi-Genre Movies**:  
    Duplicated rows for movies with multiple genres to ensure accurate genre-level insights.

---

<h2 id="findings">Findings 🔍</h2>

Our analysis revealed key insights from 7,200 movies spanning the last 50 years:

- **Total Revenue and Profit**:  
  Movies collectively earned **$614.72 billion** in revenue, with a profit of **$394.73 billion**.

- **Top Genre by Popularity**:  
  **Drama** led in popularity, followed by **Comedy** and **Thriller**.

- **Leading Movie Production Country**:  
  The **United States** emerged as the largest movie-producing country, experiencing a notable slowdown in **2020** due to the pandemic.

- **Profitable Genres**:  
  - **Adventure**, **Action**, and **Comedy** dominated both market share and revenue.  
  - Genres like **Thriller**, **Family**, and **Sci-Fi** also contributed substantially to profitability.

- **Seasonal Revenue Trends**:  
  The most profitable months for movie releases are **June**, **December**, and **May**, while **January** and **August** tend to underperform.

- **Production Companies**:  
  Leading contributors to box office success include **Marvel Studios**, **Walt Disney Pictures**, **Pixar**, and **Lucasfilm**.

- **Budget vs Profitability**:  
  - Low-budget films, such as *The Blair Witch Project*, achieved exceptional returns.  
  - Genres like **History**, **Western**, and **War** often fail to recover their budgets.

- **Impact of Barbenheimer Marketing**:  
  The simultaneous release of *Barbie* and *Oppenheimer* proved successful, with *Oppenheimer* dominating awards and *Barbie* excelling commercially.

- **Franchise Success**:  
  Blockbusters like *Avatar*, *Shrek*, and *Frozen* released in peak months demonstrate the importance of franchises for consistent profitability.

---

<h2 id="conclusion">Conclusion 🎯</h2>

- The **US leads global movie production**, though production rates slowed significantly in 2020.
- **Drama** is the most prevalent genre, but **Action** and **Comedy** dominate box office revenue.
- Seasonal analysis highlights **June, December, and May** as the most profitable months for releases.
- **Franchises and low-budget successes** (e.g., *The Blair Witch Project*) highlight diverse paths to profitability.
- The **Barbenheimer phenomenon** underlines the power of strategic marketing and word-of-mouth campaigns.
- Despite challenges, the movie industry is **rebounding post-pandemic**, signaling a positive outlook for box office performance.

---

Thank you for exploring this cinematic analysis with us! 🎥✨
