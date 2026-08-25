# Data Professional Survey Breakdown | Power BI Dashboard

## Overview

This project presents key insights and explores demographics, compensation benchmarks, tool adoption, and career satisfaction within the global data industry by analyzing survey responses from professionals across diverse domains (Data Science, Data Engineering, Data Analytics, Architecture, etc.). <br>
<br> Key questions explored encompass metrics such as salary distributions across roles, geographic representation, programming language preferences, perceived industry transition difficulty, and overall work/life balance. <br>
<br> The analysis is based on raw survey response data extracted from the Data Professional Survey dataset.

Power BI Desktop has been employed to execute this analysis, leveraging Power Query for extraction and cleaning, alongside DAX (Data Analysis Expressions) to create calculated fields and aggregation measures for comprehensive data exploration.

The interactive Power BI dashboard can be downloaded in `.pbix` format [here](Data%20Professional%20Survey%20Dashboard%20Project.pbix). <br>
The original dataset, consisting of an Excel spreadsheet, can be downloaded [here](data.xlsx).

## **Table of Contents** <br>
- [Dataset](#dataset) <br>
- [Methodology](#methodology)
- [Executive Summary](#executive-summary)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

## Dataset

The data was sourced from the Data Professional Survey dataset (`data.xlsx`), containing structured responses from industry participants.

The primary dataset attributes include:
+ **Demographics & Geography:** Respondent age, gender, and country of residence.
+ **Career Role & Compensation:** Specific job titles (Data Scientist, Data Engineer, Data Analyst, Data Architect, Database Developer, etc.) and associated average compensation bands.
+ **Technical Stack:** Favorite programming languages utilized (Python, R, C/C++, JavaScript, Java, etc.).
+ **Sentiment Scores:** Numeric ratings (1–10 scale) evaluating satisfaction with work/life balance and current compensation.
+ **Industry Transition:** Qualitative ratings indicating the perceived difficulty of breaking into the data industry.

## Methodology

The methodology employed for this project comprised standard end-to-end business intelligence phases: defining analytical requirements, data ingestion, data cleaning and transformation, measure formulation, UI/container design, testing and validation, and reporting.

1. **Data Cleaning & Transformation:** 
   * Ingested `data.xlsx` via **Power Query**.
   * Evaluated data types across numeric, textual, and categorical columns.
   * Standardized salary bands and computed average salary metrics per respondent for quantitative aggregation.
   * Grouped geographic locations and role titles to ensure clean aggregation in reporting visuals.

2. **DAX & Aggregations:**
   * Formulated aggregation measures to compute total respondents (`Total Survey Takers`), average age (`Average Age of Survey Taker`), and average satisfaction ratings for both work/life balance and salary.

3. **Visualization Design & Layout Architecture:**
   * Designed a high-contrast dark theme utilizing card containers to segment individual charts cleanly.
   * Employed gauge charts for rapid KPI assessment of satisfaction scores alongside horizontal bar charts and treemaps for multidimensional breakdowns.

![Dashboard Preview](dashboard_preview.png)

## Executive Summary

Below are the major insights that emerged from the analysis:
+ **Demographic Base:** The survey captures responses from **630 data professionals** with an average age of **29.87 years**.
+ **Geographic Concentration:** The United States represents the largest segment of survey respondents, followed by significant representation from India, the United Kingdom, and Canada.
+ **Top Compensation Bands:** Data Scientists and Data Engineers command the highest average compensation packages across the surveyed roles.
+ **Tool & Language Dominance:** Python is overwhelmingly favored as the top programming language across all job titles, with R and other specialized languages trailing behind.
+ **Satisfaction Divergence:** 
  * Respondents reported moderately positive sentiment toward **Work/Life Balance (5.74 / 10)**.
  * Sentiment toward **Salary Satisfaction is notably lower (4.27 / 10)**, highlighting a disparity between workload expectations and perceived compensation.
+ **Barrier to Entry:** A substantial share of respondents perceive breaking into the data industry as moderately difficult to very difficult.

## Recommendations

Based on the survey findings, the following recommendations are proposed:
+ **Skill Development & Curriculum Focus:** Educational programs, bootcamps, and upskilling initiatives should prioritize Python and core data engineering workflows, given their heavy dominance in industry preference and high-compensation bands.
+ **Compensation Realignment:** Organizations looking to retain skilled data talent should review compensation packages, as salary satisfaction lags behind work/life balance sentiment across most role titles.
+ **Bridging the Career Entry Gap:** Since many candidates find entering the field difficult, companies and industry groups can create structured junior pathways, internships, and mentorship programs to lower entry barriers for emerging professionals.

## Limitations

While the analysis provides clear industry insights, several limitations should be noted:
+ **Self-Reported Data:** Survey responses are self-reported, which may introduce subjective bias in compensation figures and sentiment scoring.
+ **Sample Distribution:** Regional representation is concentrated heavily in specific countries (such as the US), which may skew overall salary averages relative to global baseline markets.
+ **Static Point-in-Time Scope:** The dataset represents a single survey snapshot, limiting the ability to track multi-year longitudinal career growth or shifting language popularity trends over time.
