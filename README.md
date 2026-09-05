# Neurosurgery Statistical Analysis

## Project Overview

This project analyzes a real-world healthcare dataset titled **"A List of OR for Neurosciences"**, published by King Faisal Specialist Hospital and Research Centre (KFSH&RC) on the Saudi Open Data Portal.

The dataset contains **749 neurosurgery cases** with information such as operation year and month, gender, nationality, marital status, region, facility, and department.

The main objective is to analyze how neurosurgery operations are distributed across regions and determine whether there are statistically significant differences between regions.

## Objectives

- Analyze the distribution of neurosurgery cases across Saudi regions.
- Explore patient characteristics such as gender and marital status.
- Examine the distribution of cases across healthcare facilities.
- Apply descriptive statistics to understand the dataset.
- Use **ANOVA** to test for significant differences in monthly neurosurgery operations between regions.
- Use **Tukey HSD** to identify which regional pairs have significant differences.

## Dataset

- **Dataset:** A List of OR for Neurosciences
- **Records:** 749 neurosurgery cases
- **Source:** Saudi Open Data Portal
- **Publisher:** King Faisal Specialist Hospital and Research Centre (KFSH&RC)

## Data Analysis

### Data Cleaning

The REGION column was cleaned by removing missing, empty, unknown, and undefined values before conducting the analysis.

### Descriptive Analysis

Descriptive statistics were used to summarize the dataset and examine the distribution of the variables.

The number of cases by region was:

| Region | Cases |
|---|---:|
| Central | 240 |
| Western | 210 |
| Southern | 120 |
| Northern | 82 |
| Eastern | 73 |

The facility distribution showed that Riyadh had the highest number of cases, followed by Jeddah and Madinah.

## Statistical Analysis

### ANOVA

A one-way ANOVA was conducted to determine whether there was a significant difference in the **mean monthly number of neurosurgery operations across regions**.

**Null Hypothesis (H₀):**  
There is no significant difference in the mean monthly number of neurosurgery operations across regions.

**Alternative Hypothesis (Hₐ):**  
There is a significant difference in the mean monthly number of neurosurgery operations across regions.

### Results

- **F-statistic:** 17.39
- **p-value:** 0.000168
- **Significance level:** 0.05

Since the p-value is less than 0.05, the null hypothesis was rejected. The results indicate a statistically significant difference in monthly neurosurgery operations across regions.

### Tukey HSD

A Tukey HSD post-hoc test was performed to identify which regions differed significantly.

The results showed significant differences involving the **Central** and **Western** regions when compared with the Eastern, Northern, and Southern regions.

No significant differences were found between:
- Central and Western
- Northern and Eastern
- Southern and Eastern
- Southern and Northern

## Visualizations

The project includes visualizations for:

- Number of operations by region
- Gender distribution
- Marital status distribution
- Tukey HSD regional comparisons

## Technologies

- R
- R Markdown
- ggplot2
- dplyr
- readxl
- psych
- knitr
- multcomp

## Project Files

- `neurosurgery_analysis.Rmd` — R Markdown analysis and statistical tests
- `neurosurgery_dataset.xlsx` — Dataset used for the analysis

## Conclusion

The analysis shows that neurosurgery operations are not equally distributed across regions. The ANOVA test found a statistically significant difference in the mean monthly number of operations between regions. The Tukey HSD analysis further identified the regional pairs responsible for these differences.

The findings provide an overview of the distribution of neurosurgery cases and can support better understanding of healthcare workload and resource allocation.

## Project Type

Academic Project — Statistical Analysis
