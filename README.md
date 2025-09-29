📌 Project Overview

This project explores COVID-19 data using SQL Server. The analysis focuses on cases, deaths, and vaccinations across countries and continents. The goal is to uncover key insights such as infection rates, death percentages, vaccination progress, and global trends.

The project demonstrates SQL concepts such as:

Data cleaning and filtering

Aggregations and groupings

Window functions

Common Table Expressions (CTEs)

Temporary tables

Views for visualization

📂 Dataset

Two datasets were used from the PortfolioProject database:

CovidDeaths – contains information on COVID-19 cases, deaths, and populations.

CovidVaccinations – contains vaccination data by location and date.

⚙️ Key Queries and Insights
1. Data Preparation

Filtered out null continent values to ensure data integrity.

Selected relevant columns for analysis (location, date, cases, deaths, population).

2. Case and Death Analysis

Total Cases vs Total Deaths: Calculated death percentages to estimate the likelihood of dying if infected.

Total Cases vs Population: Measured infection rates relative to population size.

Highest Infection Rates: Identified countries with the highest infection percentages.

Highest Death Counts: Ranked countries and continents by total COVID-19 deaths.

3. Global Numbers

Aggregated new cases and deaths worldwide.

Computed global death percentage across all reported cases.

4. Vaccination Analysis

Population vs Vaccination: Used a CTE to track cumulative vaccinations (rolling totals).

Temporary Table: Stored intermediate vaccination results for further exploration.

View Creation: Built a reusable view (PercentPopulationVaccinated) to simplify later visualizations in BI tools like Tableau or Power BI.

🛠 SQL Techniques Demonstrated

Filtering (WHERE, IS NOT NULL)

Aggregations (SUM, MAX, CAST)

Window Functions (SUM() OVER (PARTITION BY ...))

Grouping (GROUP BY, ORDER BY)

Common Table Expressions (CTEs) for cleaner logic

Temporary Tables for intermediate calculations

Views for storing reusable queries

📊 Next Steps

Connect the SQL views to Tableau or Power BI for dashboard visualization.

Expand analysis to trends over time (7-day rolling averages, growth rates).

Compare vaccination rollout speed with infection/death trends.

✅ Conclusion

This project provides a structured SQL-based approach to analyzing COVID-19 data. It highlights important trends at global, continental, and national levels while showcasing practical SQL techniques useful for real-world data analytics projects.
