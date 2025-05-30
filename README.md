# DSA210-Term-Project
I am a student from Sabancı University, Elife Esin Topaktaş, and this is my DSA210 term project. The aim of this project is to analyze the correlation differences between wage growth and health insurance coverage based on race and gender in the USA, specifically between the years 2000 and 2019.
These two hypotheses will be tested:
## **Hypothesis**
- First Hypothesis: There is a stronger correlation between average hourly wages and health insurance coverage for men compared to women.
- Second Hypothesis: There is a stronger correlation between average hourly wages and health insurance coverage for White men compared to Black men.


## **Contents** 

- [Motivation](#motivation)  
- [Project Goal](#project-goal)  
- [Data Sources](#data-sources)  
- [Data Collection Process](#data-collection-process)
- [Data Preprocessing](#data-preprocessing)
- [Data Analysis](#data-analysis)
- [Findings](#findings)  
---

## **Motivation**  

For many people; wage stagnation has meant more than just financial struggles, it has made it harder to access basic needs like healthcare. As wages have stayed the same or even decreased over time, many individuals, especially from lower income backgrounds, have found it difficult to afford health insurance. This project aims to understand how wage growth or the lack of it has affected health insurance coverage. Ultimately, it’s about recognizing that everyone should have access to healthcare, no matter their income. This is a global issue, reflecting the bigger fight for fairness and equal access to essential resources.

---

## **Project Goal**  

The goal of this project is to analyze the relationship between wage growth and health insurance coverage in the United States from 2000 to 2019, with a focus on racial and gender disparities. This analysis aims to:

- Examine how changes in average hourly wages and health insurance coverage rates over time, and compare them based on race and gender differences.
- Explore socio-economic factors (such as race, gender) that may contribute to disparities in healthcare access.

By highlighting these trends, this project seeks to provide insights into the broader impact of economic inequality on healthcare access in the United States.

---

## **Data Sources**   

This project uses publicly available datasets from Kaggle (https://www.kaggle.com) to analyze the relationship between wage growth and health insurance coverage. The data sources are as follows:

### 1. Wage Data (1973-2022)  
This dataset provides median and average hourly wage information in the USA from 1973 to 2022. It includes data on wage growth across different income groups and time periods.
https://www.kaggle.com/datasets/asaniczka/median-and-avg-hourly-wages-in-the-usa-1973-2022
Link to access data: [https://github.com/esintopaktas/DSA-210/blob/main/median_average_wages.csv]

| Year | Median Wage | Average Wage | Men Median | Men Average | Women Median | Women Average | White Median | White Average | Black Median--
|------|------------|--------------|------------|-------------|--------------|--------------|--------------|--------------|--------------|
| 1973 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| 1974 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| 1975 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| ...  | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |
| 2022 | ...        | ...          | ...        | ...         | ...          | ...          | ...          | ...          | ...          |

---

### 2. Health Insurance Coverage Data (1979-2019)  
This dataset includes health insurance coverage statistics across various racial and gender groups in the United States from 1979 to 2019.https://www.kaggle.com/datasets/asaniczka/health-insurance-coverage-in-the-usa-1979-2019
Link to access data: [https://github.com/esintopaktas/DSA-210/blob/main/health_insurance_coverage.csv]

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

## Data Preprocessing 

This section summarizes the key preprocessing steps applied to the raw datasets (`median_average_wages.csv` and `health_insurance_coverage.csv`) to create the final dataset `Preprocessed_Dataset_for_Hypothesis_Testing.csv`.

### 1. Year Filtering
- Both datasets were filtered to include only data from **2000 to 2019** to ensure temporal consistency and focus the analysis period.

### 2. Column Selection
- Only the relevant demographic columns were retained for hypothesis testing:

From `median_average_wages.csv`:
- `year`, `men_average`, `women_average`, `white_men_average`, `black_men_average`

From `health_insurance_coverage.csv`:
- `year`, `men`, `women`, `white_men`, `black_men`

### 3. Data Merging
- The two datasets were merged on the `year` column using an inner join to ensure matched entries per year.

### 4. Feature Engineering
- New columns were created to calculate the difference between wage and insurance for each group as a proxy for correlation strength:
  - `men_diff` = `men_average` – `men`
  - `women_diff` = `women_average` – `women`
  - `white_diff` = `white_men_average` – `white_men`
  - `black_diff` = `black_men_average` – `black_men`

### 5. Output
- The resulting dataset `Preprocessed_Dataset_for_Hypothesis_Testing.csv` contains 20 rows (for each year from 2000 to 2019) and the following columns:
  - Wage columns, insurance columns, and their differences for men, women, white men, and black men.

This preprocessed dataset was used for visualization, correlation analysis, and hypothesis testing throughout the project.

## Data Analysis

### Exploratory Data Analysis (EDA)

The wage–insurance gap was analyzed for different demographic groups—men vs women and White men vs Black men—over the time period from 2000 to 2019.

Key insights from the analysis include:

- On average, **men had higher wages** and **higher wage–insurance differences** compared to women.
- The **gap between wage and insurance coverage** was **larger for White men** compared to Black men.
- While the wage values for all groups increased over time, the corresponding increase in insurance coverage was not proportional—resulting in rising differences, especially for men and White men.

This analysis helped identify long-term disparity patterns between wage growth and access to insurance among demographic groups.

---

###  Visualization

To better understand the trends and disparities, the following visualizations were created:

### a. Boxplots
- Compared the spread and variability of wage–insurance differences across groups.
- Helped detect which groups had more consistent or skewed disparities.

### b. Line Charts
- **Men vs Women**: Plotted wage and insurance coverage from 2000 to 2019 to observe trends over time.
- **White Men vs Black Men**: Similar trend analysis focused on racial disparity.


These visual tools allowed for a clear and interpretable comparison of wage and insurance dynamics across gender and race between 2000 and 2019.

## Findings

### Hypothesis Testing Results

### Hypothesis 1: There is a stronger correlation between average hourly wages and health insurance coverage for men compared to women.

- T-statistic: -0.6856  
- One-sided p-value: 0.7513  
- Significant at α = 0.05? No  
- Result: There is no strong evidence that the correlation between average hourly wages and health insurance coverage is stronger for men compared to women.
###- Conclusion: Although numerical differences in wages and insurance exist between men and women, statistically these do not support the claim that men benefit from a stronger correlation between rising wages and increased insurance access.

---

### Hypothesis 2: There is a stronger correlation between average hourly wages and health insurance coverage for White men compared to Black men.

- T-statistic: -0.8095  
- One-sided p-value: 0.7880  
- Significant at α = 0.05? No  
- Result: There is no strong evidence that the correlation between average hourly wages and health insurance coverage is stronger for White men compared to Black men.
###- Conclusion: Although numerical differences in wages and insurance exist between men and women, statistically these do not support the claim that men benefit from a stronger correlation between rising wages and increased insurance access.
  

**Note:** AI tools such as ChatGPT and Gemini were used during data cleaning, visualization, and statistical testing phases of this project.
##Future Works

- Extend the analysis using **multivariable regression models** to include additional socioeconomic factors such as education level, geographic location, or industry.
- Apply **causal inference techniques** (e.g., difference-in-differences, instrumental variables) to explore the direct effect of wage changes on health insurance coverage.
- Include data beyond 2019 to assess **post-pandemic shifts** in wage structure and healthcare access.
- Investigate the impact of **policy changes** (e.g., Affordable Care Act) on specific demographic groups.
- Utilize **interactive dashboards** (e.g., Plotly, Dash) for more dynamic exploration of trends and gaps.
## Future Works

- Extend the analysis using **multivariable regression models** to include additional socioeconomic factors such as education level, geographic location, or industry.
- Apply **causal inference techniques** (e.g., difference-in-differences, instrumental variables) to explore the direct effect of wage changes on health insurance coverage.
- Include data beyond 2019 to assess **post-pandemic shifts** in wage structure and healthcare access.
- Investigate the impact of **policy changes** (e.g., Affordable Care Act) on specific demographic groups.
- Utilize **interactive dashboards** (e.g., Plotly, Dash) for more dynamic exploration of trends and gaps.


## Limitations

- The proxy metric used (wage - insurance) may oversimplify the actual correlation between income and healthcare access.
- The analysis assumes a **linear and direct** relationship between wage and insurance coverage, which may not capture deeper structural factors.
- Only **annual average data** was used; more granular data (monthly, by state or occupation) could yield richer insights.
- The dataset does not account for **non-monetary factors** influencing insurance coverage, such as employer benefits or public aid.
- Statistical tests were conducted under **normality and independence assumptions**, which may not fully hold in real-world data.


