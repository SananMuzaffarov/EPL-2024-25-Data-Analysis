# EPL 2024-25 Season Analysis

A comprehensive SQL-powered analytics project exploring team performance, referee statistics, and match patterns in the English Premier League for the 2024-25 season, enhanced with **Power BI visualizations** for deeper insights.

## 📊 Project Overview

This project analyzes EPL match data to extract meaningful insights about team performance, referee tendencies, and seasonal trends. The analysis covers everything from basic team statistics to advanced metrics like conversion rates, shot accuracy, and comeback patterns. **Interactive visualizations in Power BI** bring these insights to life.

## 🛠️ Technical Stack

- **Database**: MySQL  
- **Data Source**: EPL 2024-25 season match data (CSV)  
- **Analysis Tool**: SQL queries for comprehensive analytics  
- **Visualization**: Power BI for dashboards and graphical insights  

## 📈 Key Analysis Areas

### Team Performance Metrics
- **Goal Conversion Rates** – Efficiency in converting shots to goals  
- **Shot Accuracy** – Shots on target vs total shots  
- **Home vs Away Performance** – Win/draw/loss records by venue  
- **Clean Sheets** – Defensive performance analysis  
- **Points Table** – Current league standings  

### Match Analysis
- **Highest Scoring Matches** – Games with most goals  
- **Biggest Win Margins** – Largest goal differences  
- **Comeback Matches** – Teams winning after trailing at halftime  
- **Scoring Patterns** – First-half vs second-half goals  

### Referee & Discipline
- **Referee Performance** – Cards and fouls per match  
- **Monthly Trends** – Variation in card counts over time  
- **Team Discipline** – Fouls-to-cards ratio analysis  

### Statistical Insights
- **Average Goals** – Per match, home vs away  
- **Shooting Statistics** – Total shots, shots faced  
- **Team Comparisons** – Goals scored/conceded averages  

## 📊 Statistical Analysis Notebook

The `EPL-2024_25-Data_Analysis.ipynb` notebook performs the following steps:

1. **Load Data:** Reads `season-2425.csv` into a pandas DataFrame.
2. **Calculate League Table:** Computes points, goal difference (GD), and league positions.
3. **Aggregate Team Stats:**  
   - Total Clean Sheets per team  
   - Total Cards per team (Yellow + Red)  
4. **Merge Data:** Combines league table and aggregated stats into a single `team_stats` DataFrame.
5. **Run Statistical Tests:**  
   - Pearson correlation: Clean Sheets vs League Position  
   - Pearson correlation: Total Cards vs League Position  
   - Paired t-test: Home vs Away Goals
6. **Output:**  
   - Displays top 5 teams with all stats  
   - Prints statistical test results with correlation coefficients and p-values  

> The notebook can be run interactively in [Google Colab](https://colab.research.google.com/) or locally via Jupyter.

## 🚀 Getting Started

### Prerequisites
- MySQL Database  
- EPL match data (CSV)  
- Power BI Desktop (for visualizations)
- Google Colab

## 📝 Key Files

- `EPL Queries.sql` – Complete set of analytical queries  
- `season-2425.csv` – Raw match data for the season  
- Power BI `.pbix` file – Interactive dashboards and visualizations  
- Various Excel/CSV outputs – Query results for different analyses
- `EPL-2024_25-Data_Analysis.ipynb` - Statistical Analysis of Performance Metrics

## 🔍 Analysis Highlights

The project reveals:
- Team efficiency metrics (conversion rates, shot accuracy)  
- Home vs away performance differentials  
- Referee consistency and disciplinary patterns  
- Seasonal trends in goals and cards  
- Defensive and offensive team rankings  

## 📋 Future Enhancements

In the next phase of this project, I plan to **expand the analysis beyond the English Premier League** by scraping and integrating data from other **top European leagues** such as:

- **La Liga (Spain)**
- **Serie A (Italy)**
- **Bundesliga (Germany)**
- **Ligue 1 (France)**

This will enable a **cross-league comparison** of performance metrics, including:

- Goal conversion rates and shooting efficiency  
- Defensive solidity and clean sheet ratios  
- Disciplinary patterns and referee trends  
- Home vs away performance contrasts  

Additionally, I will enhance the existing data model by:

- **Adding new variables** such as expected goals (xG), possession percentage, passing accuracy, and player-level metrics  
- **Writing new SQL queries** to generate advanced insights, trend analyses, and predictive statistics  
- **Updating Power BI dashboards** to include comparative visualizations between leagues, teams, and player performances  

These improvements aim to transform the project into a **comprehensive, multi-league football analytics platform**, offering a richer understanding of tactical differences, league competitiveness, and performance dynamics across Europe.
