# Project Documentation

## 1. Business Problem

The tournament generated player-level batting, bowling, and fielding statistics through CricHeroes. However, the raw statistics were spread across separate datasets, making it difficult to compare players consistently across different areas of performance.

The objective of this project was to consolidate the tournament data, clean and validate the statistics, and develop an analytical solution that could:

- Evaluate batting, bowling, and fielding performance.
- Compare players and teams using meaningful KPIs.
- Identify top performers and multi-discipline contributors.
- Create a consistent player-performance scoring model.
- Present the results through SQL analysis and an interactive Power BI dashboard.

## 2. Project Objective

Build an end-to-end cricket analytics solution using Python/Pandas, SQL, and Power BI to transform raw tournament statistics into actionable performance insights.

## 3. Dataset

The analysis covers 21 players across 3 teams.

The raw data consisted of separate datasets for:

- Batting
- Bowling
- Fielding
- MVP

The data was collected from CricHeroes tournament statistics.

## 4. Data Preparation

Python and Pandas were used to:

- Load the raw Excel datasets.
- Inspect data structure and data types.
- Clean cricket-specific values such as not-out indicators (`*`).
- Convert numeric fields into appropriate data types.
- Handle undefined batting averages and bowling metrics.
- Convert cricket overs into actual balls for accurate calculations.
- Validate strike rate, bowling economy, bowling average, and fielding dismissals.
- Combine batting, bowling, and fielding data into a player-level analytical dataset.

## 5. SQL Analysis

SQLite was used to perform analytical queries including:

- Top run scorers.
- Players scoring 50+ runs.
- Team batting totals.
- Team bowling performance.
- Top strike rates.
- Batting performance classification using `CASE WHEN`.
- Top wicket takers.
- Player rankings using `DENSE_RANK()`.
- Team rankings.
- All-round performance analysis.
- Three-discipline player analysis.
- Final MVP leaderboard.

## 6. Performance Scoring Model

A weighted scoring model was developed to compare overall player performance.

| Component | Weight |
|---|---:|
| Batting | 50% |
| Bowling | 35% |
| Fielding | 15% |

The resulting score was used to create an overall player ranking.

This scoring model was created specifically for this project and is intended as an analytical methodology rather than an official cricket MVP formula.

## 7. Power BI Dashboard

The Power BI dashboard provides:

- Tournament-level KPIs.
- Team batting performance.
- Team bowling performance.
- Top run scorers.
- Top wicket takers.
- Overall player rankings.
- Batting vs bowling contribution analysis.
- Detailed player performance metrics.
- Interactive player and team filters.

## 8. Key Outcomes

The project demonstrates an end-to-end analytics workflow:

Raw Data → Python/Pandas → Data Validation → SQL Analysis → Power BI → Insights

The final solution provides a structured way to evaluate player and team performance across multiple dimensions rather than relying on a single statistic.
