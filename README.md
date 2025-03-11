# DSA210-Term-Project

I am a student from Sabancı University, Ada Dila Akbulut, and this is my DSA210 term project. The aim of this project is to analyze the impact of wage growth on access to health insurance in the USA, specifically between the years 1979 and 2019. 

## Topic Overview

This project explores how wage growth (both median and average hourly wages) has influenced health insurance coverage over time. Historically, many workers' ability to afford or access employer-sponsored health insurance has been closely tied to wage levels. This analysis will investigate how periods of stagnant wage growth, particularly for low- and middle-income workers, correlate with a decline in health insurance coverage.

**Key Focus**:  
The primary focus of the analysis is to examine whether periods of stagnant wage growth coincide with decreases in the percentage of people with health insurance, particularly employer-sponsored coverage. This includes analyzing trends in both median and average wages, as well as health insurance coverage data across various demographic groups.

---

## Contents

- [Motivation](#motivation)
- [Project Goal](#project-goal)
- [Data Sources and Preprocessing](#data-sources-and-preprocessing)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
- [Hypothesis Testing](#hypothesis-testing)
- [Limitations and Future Work](#limitations-and-future-work)

---

## Motivation

In recent decades, there has been significant discussion around wage growth and its impact on people's access to essential services, including healthcare. As wages have stagnated, especially among low- and middle-income workers, many people have lost access to employer-sponsored health insurance. This project aims to investigate the extent to which wage growth (or lack thereof) affects health insurance coverage, which is vital for the well-being of individuals and families. By exploring this relationship, we hope to understand how economic factors influence public health outcomes and healthcare access in the United States.

---

## Project Goal

The goal of this project is to analyze the relationship between wage growth and health insurance coverage in the United States from 1979 to 2019. Through this analysis, we aim to:

1. Examine how changes in both median and average hourly wages have affected health insurance coverage rates over time.
2. Identify periods of wage stagnation and explore if they coincide with declines in access to employer-sponsored health insurance.
3. Investigate other socio-economic factors that may contribute to these trends.

---

## Data Sources and Preprocessing

This project uses publicly available datasets from Kaggle to analyze the relationship between wage growth and health insurance coverage. The data sources and preprocessing steps are as follows:

1. **Health Insurance Coverage Data**  
   - The dataset includes health insurance coverage statistics for different types of insurance (e.g., employer-sponsored, public health insurance, and private insurance) across various U.S. states from 1979 to 2019.
   
2. **Wage Data**  
   - The dataset provides median and average hourly wage information in the USA from 1973 to 2022. It includes data on wage growth across different income groups and time periods.

### Preprocessing Steps:
- **Cleaning Data**: Any missing or inconsistent data points are handled using imputation or removal methods.
- **Data Transformation**: The data is formatted into a structured format, and relevant columns are selected for analysis.
- **Normalization**: The wage data and health insurance coverage rates are normalized to ensure consistency in comparisons over time.
  
These datasets will be merged by year and analyzed to explore correlations.

---

## Data Analysis

1. **Data Preprocessing**  
   The data preprocessing includes:
   - Merging wage data and health insurance data by year to track the changes in wage growth and health insurance coverage over time.
   - Handling missing data and outliers to ensure the dataset is clean for analysis.
   
2. **Exploratory Data Analysis (EDA)**  
   - Descriptive statistics will be used to explore key metrics such as average wages and health insurance coverage.
   - Trends in health insurance coverage rates will be visualized over the course of the selected years.
   
3. **Correlation Analysis**  
   - A correlation analysis will be conducted to assess the relationship between wage growth and health insurance coverage rates.
   - We will test whether stagnant wage growth periods align with decreases in health insurance coverage.
   
4. **Visualization**  
   - Various types of visualizations (line charts, bar charts, scatter plots) will be used to display trends in health insurance coverage and wage growth.
   - These visualizations will help identify patterns and provide clear insights into the data.

---

## Findings

Based on preliminary analysis, we expect to find that:

- **Wage Stagnation**: During periods of stagnant wage growth (e.g., the 1980s and early 2000s), there may be a corresponding decline in employer-sponsored health insurance coverage, particularly among low- and middle-income workers.
- **Shifting Health Insurance Landscape**: As wages stagnated, there could be a greater reliance on public health insurance programs like Medicaid, especially after the 2008 financial crisis.
- **Economic Disparities**: The disparity in wage growth across income groups may be linked to the widening gap in access to health insurance.

---

## Hypothesis Testing

This analysis will test the following hypotheses:

- **First Hypothesis**: During periods of stagnant wage growth, access to employer-sponsored health insurance decreases, especially among low- and middle-income workers.
- **Second Hypothesis**: Periods of strong wage growth are associated with an increase in health insurance coverage, particularly employer-sponsored insurance.

Statistical tests, including correlation analysis and regression models, will be used to test these hypotheses.

---

## Limitations and Future Work

### Limitations:
- **Data Availability**: The available datasets are limited to health insurance coverage and wage data; other socio-economic factors (e.g., unemployment rates, changes in healthcare policies) are not included but may also influence the outcomes.
- **Causality**: While correlations between wage growth and health insurance coverage can be observed, establishing direct causality requires a more complex analysis, which is beyond the scope of this project.

### Future Work:
- A more comprehensive model that includes other factors (e.g., healthcare policies, unemployment rates) could provide deeper insights into the determinants of health insurance coverage.
- A regional analysis could be conducted to examine how different states' wage growth affects health insurance coverage due to varying state-level policies.

---

This project aims to shed light on the complex relationship between wage growth and health insurance coverage, contributing valuable insights into how economic factors shape access to healthcare in the United States.
