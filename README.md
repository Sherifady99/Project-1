# Football Scouting Agency ™

Football Scouting Agency ™ offers data-driven solutions for football clubs to gain high-quality insights on top football talents worldwide. Leveraging APIs, web scraping, and advanced analytics, we help clubs discover players who deliver top performance at competitive costs.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Hypotheses](#hypotheses)
- [Data Sources & Collection](#data-sources--collection)
- [Data Cleaning & Wrangling](#data-cleaning--wrangling)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Visualization](#visualization)
- [Project Timeline](#project-timeline)
- [Team & Contribution Guidelines](#team--contribution-guidelines)
- [License](#license)

---

## Project Overview

**Football Scouting Agency ™** provides football clubs with actionable insights by analyzing performance metrics and transfer market data. Our objective is to identify top-performing yet cost-efficient players from the world's elite leagues.

---

## Problem Statement

**2024 Challenge:**  
Identify the top 5 most performance-efficient players in 2024 from the top 5 leagues—while ensuring they are also among the cheapest based on performance efficiency.

- **Leagues & IDs:**
  - **Premier League:** “GB1”
  - **La Liga:** “ES1”
  - **Série A:** “IT1”
  - **Ligue 1:** “FR1”
  - **Bundesliga:** “L1”
  
Total players from these leagues: **2,805**

---

## Hypotheses

1. **Cost Efficiency:** None of the top 5 players will be cheaper than 50M EUR.
2. **Performance Efficiency:** Performance efficiency is measured by goal contributions relative to minutes played. (Example metrics: *minutes played / (goals + assists)*
3. **Player Movement:** None of the top 5 players in 2022 will appear in the top 5 in 2024.

---

## Data Sources & Collection

Data is collected from multiple trusted sources:
- **APIs:** For example, `https://transfermarkt6.p.rapidapi.com/players/profile` to retrieve player information.

> **Note:** *Always save the fetched data locally (e.g., CSV files) to minimize API calls and manage rate limits.*

---

## Data Cleaning & Wrangling

Our data preprocessing involves:
- Handling null values and duplicates
- Dropping irrelevant columns
- Manipulating strings and formatting fields
- Creating new variables (e.g., goal contributions efficiency)

---

## Exploratory Data Analysis (EDA)

We employ EDA to:
- Validate hypotheses through univariate, bivariate, and multivariate analysis.
- Compare data across 2022 and 2024.
- Utilize descriptive statistics and visualization tools to extract actionable insights.
  
Key insights include:
- **Goal Contributions per Million Euros:** Efficiency comparison.
- **Minutes per Goal:** Performance metrics for top players.

---

## Visualization

Visualization strategies are chosen to clearly communicate insights:
- **Chart Types:** Bar charts for categorical comparisons, line charts for trends.
- **Design Principles:** Minimal clutter, focused attention using bold text and contrasting colors.
- **Interactive Elements:** Dashboards built with Python libraries, Seaborn and matplotlib

---

## Project Timeline

- **Day 1 (Thursday):**
  - Brainstorm interesting topics and formulate hypotheses.
  - Set up GitHub repository and create a Kanban board.
- **Day 2/3 (Saturday - Tuesday):**
  - Data Collection: Fetch data via APIs and web scraping.
  - Data Wrangling: Clean, transform, and structure the data.
- **Day 4 (Thursday):**
  - Finalize data cleaning, perform EDA, and refine code.
  - Prepare initial visualizations.
- **Day 5 (Saturday):**
  - Final presentation and demo.

**Checklist Highlights:**
- Decide on columns to keep for 2022 and 2024.
- Calculate and add goal contribution efficiency columns.
- Rank top 5 players.
- Merge DataFrames (performance metrics and additional info).
- Build charts comparing key performance indicators across years.

---

## Team & Contribution Guidelines

**Team Members:**
> Jorge info: 
- jorgemmlrodrigues@gmail.com
- https://www.linkedin.com/in/jorgemmlrodrigues/
Sherif info : 
- sherifady99@gmail.com
- https://www.linkedin.com/in/sherif-costantin-6a9219152/ 

**Contribution Guidelines:**
- Merge individual work into the shared document only after thorough testing.



## API Reference

#### API Endpoints

```https://rapidapi.com/ntd119/api/transfermarkt6```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |



## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`API_KEY`
ex: x-rapidapi-key=**************************************************


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)

