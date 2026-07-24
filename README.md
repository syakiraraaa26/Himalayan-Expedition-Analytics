# Himalayan-Expedition-Analytics
Data analysis project exploring Himalayan Expedition trends, success factors, safety risks, and climber profiles using Python and Looker Studio.


## Project Overview

The Himalayan region is home to some of the world's highest and most challenging mountain peaks. Over more than a century, thousands of expeditions have attempted to reach these summits under varying conditions, strategies, and levels of risk.

This project analyzes historical Himalayan expedition data from 1905 to 2024 to understand expedition performance, identify factors associated with summit success, examine historical safety risks, and explore the characteristics of recorded expedition members.

The project covers the complete analytical workflow, from data cleaning and exploratory analysis using Python to the development of an interactive dashboard in Looker Studio.

## Background

The Himalayan Database contains extensive historical records of mountaineering expeditions across the Himalayan region. The dataset includes information about expeditions, peaks, and expedition members, providing an opportunity to analyze more than a century of climbing activity.

However, the information is distributed across multiple datasets and contains numerous variables, making historical patterns difficult to interpret directly. This project transforms the data into a structured analytical framework and interactive dashboard that makes expedition trends, outcomes, risks, and participant characteristics easier to understand.

## Business Problem

How can historical Himalayan expedition data be transformed into actionable insights to better understand expedition performance, factors associated with success, safety risks, and climber characteristics?

## Objectives

- Analyze historical patterns and trends in Himalayan expedition activity.
- Evaluate expedition performance and summit success.
- Identify factors associated with expedition success.
- Examine common reasons for expedition failure and recorded causes of death.
- Compare historical risk patterns across different member groups.
- Explore the demographic and professional profiles of expedition members.
- Develop an interactive dashboard that makes complex expedition data easier to explore and understand.

## Business Questions

### Expedition Performance
- How has Himalayan expedition activity changed over time?
- Which seasons have the highest expedition activity?
- What is the overall success rate of recorded expeditions?
- What are the most frequently climbed peaks?
- What are the most common recorded reasons for unsuccessful expeditions?

### Success & Risk Analysis
- How does expedition success vary across seasons?
- How does expedition success differ between expeditions using and not using supplemental oxygen?
- What is the relationship between peak elevation and expedition success rate?
- What are the leading recorded causes of death among expedition members?
- How do fatality rates differ between hired and non-hired members?
- How do fatality rates compare between Sherpa and non-Sherpa members?

### Member Profile
- What are the general demographic characteristics of recorded expedition members?
- How does member success vary by gender?
- Which nationalities are most represented among expedition members?
- What are the most common occupations among expedition members?

## Dataset

The raw dataset used in this project was provided as part of the **RevoU Mini Course** learning material and contains historical records related to Himalayan mountaineering expeditions.

The original dataset consists of multiple related tables. For this analysis, three main datasets were selected and processed:

| Dataset | Description | Cleaned Records |
|---|---|---:|
| `exped` | Historical expedition records and expedition outcomes | 11,423 |
| `members` | Records of expedition participants and their outcomes | 88,999 |
| `peaks` | Information about Himalayan peaks | 480 |

The record counts shown above represent the **cleaned datasets used for analysis and dashboard development**, after data preparation and cleaning in Python.

The cleaned dataset covers expedition records from **1905 to 2024**.

> **Data Source:** Dataset provided through the **RevoU Mini Course** for educational and analytical purposes.

> **Note:** The `members` dataset contains participation records. Therefore, record counts should not necessarily be interpreted as the number of unique individuals.

- **View the cleaned dataset:** [Himalayan Expedition Clean.xlsx](data/Himalayan%20Expedition%20Clean.xlsx)

## Tools & Technologies

- **Python (Pandas)** — Data cleaning, preparation, and exploratory data analysis
- **Google Colab** — Python development environment
- **Google Sheets** — Cleaned data storage and dashboard data source
- **Looker Studio** — Interactive dashboard development
- **GitHub** — Project documentation

## Data Preparation & Cleaning

The raw datasets were cleaned and prepared using Python before being used for analysis and dashboard development.

The main preparation steps included:

- Selecting relevant columns based on the analytical objectives.
- Removing duplicate records.
- Handling missing values according to the meaning and usability of each field.
- Standardizing data types.
- Converting selected Boolean fields into analysis-ready formats.
- Resetting indexes after the cleaning process.
- Validating the final dataset dimensions and key analytical fields.

The complete data preparation and exploratory analysis process is available in the notebook folder, soon.

## Dashboard

The interactive dashboard is organized into three analytical sections:

### 1. Executive Overview

Provides a high-level overview of historical expedition activity, including expedition volume, overall success, seasonal activity, popular peaks, and common reasons for unsuccessful expeditions.


### 2. Success & Risk Analysis

Examines factors associated with expedition outcomes and historical safety risks, including seasonality, supplemental oxygen usage, peak elevation, causes of death, and fatality patterns across member groups.


### 3. Member Profile

Explores the characteristics of recorded expedition members through gender, age, nationality, occupation, member success, and detailed expedition records.

- **Live Dashboard:** [Buka Laporan Penjualan di Looker Studio](https://datastudio.google.com/reporting/87f710c5-5126-4d29-8d2e-0749df96fe8b)

# Analysis, Insights & Recommendations

This section interprets the dashboard findings by connecting the visualizations with the original business questions. Each dashboard page is analyzed separately to highlight the main findings, practical insights, and data-driven recommendations.

## 1. Executive Overview

### Business Questions

- How has Himalayan expedition activity changed over time?
- Which seasons record the highest expedition activity?
- What is the overall expedition success rate?
- Which peaks are climbed most frequently?
- What are the most common reasons for expedition failure?

### Dashboard Snapshot

> **Figure 1. Executive Overview Dashboard**  
> Overview of expedition trends, seasonal activity, expedition outcomes, and climbing distribution across the Himalayan region.

GAMBAR DASHBOARD PAGES 1

### Key Findings

- Historical expedition activity increased substantially over time, particularly after the 1980s.

- Spring and Autumn accounted for most recorded expeditions, with Spring achieving the highest historical success rate (57.22%).

- Overall expedition success reached 54.94%, indicating that slightly more than half of recorded expeditions successfully reached the summit.

- Mount Everest appeared as the most frequently climbed peak in the dataset.

- Among unsuccessful expeditions, weather-related conditions and logistical challenges were the most common recorded termination reasons.

### Key Insights

- The dashboard suggests that Himalayan expeditions have become increasingly popular over time while remaining highly dependent on seasonal conditions.

- The concentration of climbing activity during Spring reflects historical planning preferences, where climbers tend to choose more favorable weather windows to improve expedition outcomes.

- Although expedition participation continues to grow, success rates remain relatively stable, indicating that increasing experience and technology do not completely eliminate environmental risks.

### Recommendations

- Prioritize expedition planning during historically favorable climbing seasons.
- Incorporate historical expedition records when selecting climbing windows.
- Combine historical trends with real-time weather forecasts to improve decision making.

## 2. Success & Risk Analysis

### Business Questions

- Does supplemental oxygen improve expedition success?
- How does success vary by season?
- Does peak elevation relate to expedition success?
- What are the major causes of fatalities?
- How do fatality rates differ across climber groups?

### Dashboard Snapshot
> **Figure 2. Success & Risk Analysis Dashboard**  
> Analysis of expedition success, oxygen usage, peak elevation, and fatality patterns.

GAMBAR DASHBOARD PAGES 2

### Key Findings

- Spring recorded the highest expedition success rate among all seasons, followed by Autumn.

- Expeditions that used supplemental oxygen had a much higher success rate (79.63%) than those without supplemental oxygen (44.57%).

- The scatter plot shows that expedition success generally becomes lower as peak elevation increases.

- Avalanches and falls were the most common causes of recorded fatalities.

- Fatality rates were slightly higher among hired members than non-hired members. Meanwhile, Sherpa and non-Sherpa members showed similar fatality rates.

### Key Insights

- The results suggest that expedition success is related to several factors instead of only one.

- Seasonal conditions appear to influence climbing outcomes, as Spring consistently recorded the highest success rate.

- Supplemental oxygen is associated with a much higher success rate. However, this result does not mean that oxygen alone determines expedition success, since weather, experience, route conditions, and other factors may also play important roles.

- Higher mountains generally show lower success rates, highlighting the additional challenges of climbing at extreme elevations.

- Although fatality rates differ slightly between some member groups, the differences are relatively small. This suggests that mountain risks affect most climbers regardless of their role.

### Recommendations

- Plan expeditions during seasons with historically higher success rates whenever possible.
- Consider supplemental oxygen as one of several factors in expedition planning, especially for high-altitude climbs.
- Strengthen safety preparation for higher peaks where climbing conditions are more challenging.
- Use historical fatality records to improve risk management and emergency planning.

## 3. Member Profile

### Business Questions

- What are the demographic characteristics of expedition members?
- Which nationalities participate most frequently?
- Which occupations are most common?
- What is the average climber age?
- How successful are expedition members overall?

### Dashboard Snapshot
> **Figure 3. Member Profile Dashboard**  
> Overview of climber demographics, participation patterns, and expedition member characteristics.

GAMBAR DASHBOARD PAGES 3

### Key Findings

- The dataset contains **88,999** expedition member records from many different countries.

- Male climbers accounted for most expedition members, while female participation represented a much smaller share.

- Nepal recorded the highest number of expedition members among all nationalities.

- Alpine Guide was the most common occupation in the dataset.

- The average climber age was approximately **33 years**, and the overall member success rate was **41.49%**.

### Key Insights

- The data shows that Himalayan expeditions involve participants from many countries, highlighting the global interest in high-altitude mountaineering.

- The large proportion of male climbers suggests that expedition participation is still dominated by men, although female climbers are also represented in the dataset.

- Nepal's leading position reflects its important role in Himalayan expeditions, both as the location of many major peaks and as the home country of many experienced climbers and mountain professionals.

- Although many people participate in expeditions, fewer than half of all recorded member attempts successfully reached the summit. This shows that climbing in the Himalayas remains physically demanding and challenging.


### Recommendations

- Improve climber preparation through physical training and high-altitude experience before major expeditions.
- Encourage knowledge sharing between experienced climbers and new expedition members.
- Continue collecting member data to better understand participation trends and support future expedition planning.


## Author

**Syakira Tsania Muthmainnah**  
Data Science Graduate | Aspiring Data Analyst & Data Scientist
- Email : syakiratsania24@gmail.com

This project was developed as a portfolio project to demonstrate skills in data cleaning, exploratory data analysis, data visualization, and business insights.

