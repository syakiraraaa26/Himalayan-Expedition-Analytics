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

The dataset used in this project was provided as part of a **RevoU Mini Course** learning material and contains historical records related to Himalayan mountaineering expeditions.

The analysis uses three main datasets:

| Dataset | Description | Records |
|---|---|---:|
| `exped` | Historical expedition records and expedition outcomes | 11,423 |
| `members` | Records of expedition participants and their outcomes | 88,999 |
| `peaks` | Information about Himalayan peaks | 480 |

The cleaned dataset covers expedition records from **1905 to 2024**.

> **Data Source:** Dataset provided through the **RevoU Mini Course** for educational and analytical purposes.

> **Note:** The `members` dataset contains participation records. Therefore, record counts should not necessarily be interpreted as the number of unique individuals.

- **View the cleaned dataset:** [Himalayan_Expedition_Clean.xlsx](./data/Himalayan_Expedition_Clean.xlsx)

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



## Key Findings

_To be finalized after reviewing the complete dashboard analysis._

## Key Insights

_To be finalized after reviewing the complete dashboard analysis._

## Recommendations

_To be finalized after reviewing the complete dashboard analysis._

## Project Structure
    Himalayan-Expedition-Analytics/
    ├── README.md
    ├── data/
    │   └── Himalayan Expedition Clean.xlxs
    ├── notebooks/
    │   └── himalayan_expedition_analysis.ipynb
    └── dashboard/
        ├── 01_executive_overview.png
        ├── 02_success_risk_analysis.png
        └── 03_member_profile.png
