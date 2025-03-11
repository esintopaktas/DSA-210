# DSA210-Term-Project
I am a student from Sabancı University, Elife Esin Topaktaş, and this is my DSA210 term project. The aim of this project is to analyze the impact of wage growth on access to health insurance in the USA, specifically between the years 2000 and 2019.



## **Contents** 

- [Motivation](#motivation)  
- [Project Goal](#project-goal)  
- [Data Sources](#data-sources)  
- [Data Collection Process](#data-collection-process) 
---

## **Motivation**  

For many people; wage stagnation has meant more than just financial struggles, it has made it harder to access basic needs like healthcare. As wages have stayed the same or even decreased over time, many individuals, especially from lower income backgrounds, have found it difficult to afford health insurance. This project aims to understand how wage growth or the lack of it has affected health insurance coverage. Ultimately, it’s about recognizing that everyone should have access to healthcare, no matter their income. This is a global issue, reflecting the bigger fight for fairness and equal access to essential resources.

---

## **Project Goal**  

The goal of this project is to analyze the relationship between wage growth and health insurance coverage in the United States from 2000 to 2019, with a focus on racial and gender disparities. This analysis aims to:

- Examine how changes in median and average hourly wages have affected health insurance coverage rates over time, particularly for Black, Hispanic, and female workers.
- Identify periods of wage stagnation and investigate whether they coincide with declines in health insurance coverage among historically marginalized groups.
- Explore socio-economic factors (such as race, gender, and income inequality) that may contribute to disparities in healthcare access.

By highlighting these trends, this project seeks to provide insights into the broader impact of economic inequality on healthcare access in the United States.

---

## **Data Sources**   

This project uses publicly available datasets from Kaggle (https://www.kaggle.com) to analyze the relationship between wage growth and health insurance coverage. The data sources are as follows:

### 1. Wage Data (1973-2022)  
This dataset provides median and average hourly wage information in the USA from 1973 to 2022. It includes data on wage growth across different income groups and time periods.
https://www.kaggle.com/datasets/asaniczka/median-and-avg-hourly-wages-in-the-usa-1973-2022

| Year | Median Wage | Average Wage | Men Median | Men Average | Women Median | Women Average | White Median | White Average | Black Median |
|------|------------|--------------|------------|-------------|--------------|--------------|--------------|--------------|--------------|
| 1973 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| 1974 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| 1975 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| ...  | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| 2022 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |

---

### 2. Health Insurance Coverage Data (1979-2019)  
This dataset includes health insurance coverage statistics across various racial and gender groups in the United States from 1979 to 2019.https://www.kaggle.com/datasets/asaniczka/health-insurance-coverage-in-the-usa-1979-2019

| Year | All | White | Black | Hispanic | Men | White Men | Black Men | Hispanic Men | Women |
|------|-----|-------|-------|----------|-----|-----------|-----------|--------------|-------|
| 1979 | ... | ...   | ...   | ...      | ... | ...       | ...       | ...          | ...   |
| 1980 | ... | ...   | ...   | ...      | ... | ...       | ...       | ...          | ...   |
| 1981 | ... | ...   | ...   | ...      | ... | ...       | ...       | ...          | ...   |
| ...  | ... | ...   | ...   | ...      | ... | ...       | ...       | ...          | ...   |
| 2019 | ... | ...   | ...   | ...      | ... | ...       | ...       | ...          | ...   |

---
## **Data Collection Process**

The data collection process includes the following steps:

1. **Identifying Sources:** Relevant and reliable official institutions' websites that provide data directly related to the research topic were identified.

2. **Data Downloading:** Data for the relevant years were downloaded from the specified websites. The data is typically in CSV or Excel format and organized on an annual basis.

3. **Data Integration:** Data related to wages, health insurance coverage, and socio-economic factors were merged using common keys (e.g., year, age group, racial/ethnic group).

4. **Preparation for Analysis:** The integrated data was transformed into appropriate formats for statistical analysis and visualizations.

