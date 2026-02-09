# Project: EDA on World Suicide Rates

## Overview
This project performs an extensive exploratory data analysis (EDA), data cleaning, and preparation on a dataset of world suicide rates. The goal is to transform raw data into a clean, well-structured format suitable for advanced visualization and dashboard creation using tools like PowerBI or Tableau.

## Dataset
The dataset used for this analysis is **`world_suicide_rates.csv`**, obtained from Kaggle. It contains suicide rate data across various countries and years.

## Project Phases

### 1. Data Loading
- The **`world_suicide_rates.csv`** file was loaded into a pandas DataFrame.

### 2. Exploratory Data Analysis (EDA)

**Initial Inspection**
- Reviewed the first few rows  
- Checked data types  
- Verified non-null counts  

**Descriptive Statistics**
- Generated summary statistics for numerical columns  

**Unique Values**
- Identified the number of unique countries and years  
- Confirmed data coverage: **233 countries, 22 years**

**Distribution of Suicide Rate**
- Visualized the overall distribution of **`Suicide Rate`** using a histogram to understand its spread  

### 3. Data Cleaning and Preparation

**Missing Values**
- Confirmed no missing values were present in the dataset  

**Column Name Standardization**
- Renamed columns to `snake_case` (e.g., `country_name`, `suicide_rate`) for consistency and ease of use in database/dashboard environments  

**Data Consistency Checks**
- Verified that each `country_name` consistently maps to a unique `country_code` and vice-versa, ensuring data integrity  

**Feature Engineering**
- `global_average_suicide_rate`: Calculated the average suicide rate across all countries for each year to observe global trends  
- `suicide_rate_change`: Computed the year-over-year change in suicide rates for each country, providing insights into rate fluctuations  

**Data Type Confirmation**
- Ensured all columns, including newly created ones, have appropriate data types  

### 4. Key Visualizations Generated

**Global Average Suicide Rate Over Time**
- A line plot showing the trend of global suicide rates from 2000 to 2021  

**Top 10 Countries by Average Suicide Rate**
- A bar chart highlighting countries with the highest average suicide rates  
- Includes data labels for precise comparison  

**Distribution of Suicide Rate Change**
- A histogram illustrating the year-over-year variations in suicide rates  

### 5. Saved Data
- The cleaned and prepared dataset has been saved as **`cleaned_world_suicide_rates.csv`**  
- This file is ready for direct import into visualization tools  

## PowerBI/Tableau Dashboard Focus Areas

### Overall Trends
- Visualize `global_average_suicide_rate` over `year` as a prominent line chart  

### Country-Specific Analysis
- Allow users to filter or select specific `country_name` or `country_code`  
- Display `suicide_rate` over `year` for selected countries  
- Show `suicide_rate_change` to identify periods of increase or decrease  

### Comparative Analysis
- Use bar charts to compare `suicide_rate` across different `country_name` values  
- Potentially show top/bottom N countries  

### Distribution of Changes
- Include a histogram or density plot of `suicide_rate_change` to understand the common magnitudes of year-over-year fluctuations  

### Key Performance Indicators (KPIs)
- Current year's global average suicide rate  
- Overall highest/lowest suicide rates  
- Largest year-over-year increase/decrease in suicide rate  

### Interactivity
- Provide slicers/filters for year range and `country_name`  
- Implement drill-down capabilities from global to country-specific views  

## Key Insights from EDA & Preparation
- The dataset is comprehensive, covering **233 countries over 22 years**, with no missing values initially  
- Consistent country identification is ensured through unique `country_name` to `country_code` mappings  
- New features `global_average_suicide_rate` and `suicide_rate_change` provide valuable metrics for trend and volatility analysis.
