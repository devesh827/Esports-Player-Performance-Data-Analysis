# 🎮 Esports Player Performance Data Analysis

## 📌 Project Overview

This project performs an **end-to-end Exploratory Data Analysis (EDA)** on an esports tournament dataset to understand **player performance, team effectiveness, and match dynamics**. The analysis follows a structured data analysis workflow — from data cleaning to insight generation — using **Python, Pandas, and Matplotlib**.

The goal is to demonstrate **real-world data analysis skills** suitable for **data analyst / data science roles**, interviews, and portfolios.

---

## 📂 Dataset Description

The dataset contains **2,800 match-level records** capturing player, team, and match performance metrics from esports tournaments.

### 🔹 Key Columns

| Column Name         | Description                                       |
| ------------------- | ------------------------------------------------- |
| `record_id`         | Unique match record ID                            |
| `player_id`         | Unique player identifier                          |
| `team_name`         | Team name                                         |
| `player_role`       | Role of player (Flex, Support, Sniper, IGL, etc.) |
| `map_played`        | Map on which the match was played                 |
| `match_type`        | Match stage (Final, Playoff, Semi-Final)          |
| `kills`             | Number of kills                                   |
| `assists`           | Number of assists                                 |
| `deaths`            | Number of deaths                                  |
| `accuracy_percent`  | Shooting accuracy percentage                      |
| `reaction_time_ms`  | Reaction time in milliseconds                     |
| `fatigue_index`     | Player fatigue level (0–1)                        |
| `performance_score` | Composite performance metric                      |
| `win_probability`   | Estimated probability of winning                  |
| `match_outcome`     | Match result (Win/Loss)                           |
| `mvp_award`         | MVP award indicator (Yes/No)                      |

---

## 🛠️ Tools & Technologies Used

* **Python 3**
* **Pandas** – Data manipulation & analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Jupyter Notebook / VS Code**

---

## 🧹 Data Cleaning Steps

* Removed duplicate records
* Handled missing values:

  * Numerical columns → filled with mean
  * Categorical columns → filled with "Unknown"
* Verified data types and ranges

---

## 🔍 Exploratory Data Analysis (EDA)

### ✅ Easy-Level Analysis

* Total number of matches
* Most active teams
* Average performance score

### ✅ Medium-Level Analysis

* Performance comparison by player roles
* Impact of match type on win probability
* Relationship between kills and performance score

### ✅ Hard-Level Analysis

* Correlation analysis of performance metrics
* MVP vs Non-MVP performance comparison
* Fatigue impact on win probability
* Elite player identification (Top 10%)

---

## 📊 Key Visualizations

* Performance score distribution (Histogram)
* Player role frequency (Bar chart)
* Correlation heatmap (Matplotlib)
* MVP vs Non-MVP performance comparison (Boxplot)
* Pivot table heatmap: **Map vs Team performance**

---

## 🧠 Feature Engineering

### 🔹 Efficiency Score

A custom metric was created to evaluate **player efficiency**:

```
Efficiency Score = ((Kills + Assists) / (Deaths + 1)) × (1 − Fatigue Index)
```

This metric:

* Rewards high contribution
* Penalizes excessive deaths
* Adjusts for player fatigue

---

## 📌 Key Insights

* **Performance score** is the strongest indicator of success
* Higher accuracy and lower reaction time increase win probability
* Fatigue negatively impacts match outcomes
* MVP players consistently outperform non-MVPs
* Certain teams perform better on specific maps

---

## 📈 Business & Analytical Conclusions

* Teams should prioritize **high-efficiency, low-fatigue players**
* Player–map specialization improves win chances
* Data-driven player selection can enhance tournament outcomes
* Custom metrics help identify hidden top performers

---


