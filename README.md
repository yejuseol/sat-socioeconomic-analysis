# SAT Socioeconomic Analysis

## Overview
This project investigates factors that influence SAT scores beyond academic ability. Using a dataset of Massachusetts public schools, we analyze how socioeconomic background, demographic composition, and educational resources relate to differences in SAT performance.

The goal of this analysis is to explore whether SAT scores truly reflect academic merit or whether external structural factors such as economic inequality and access to educational resources also play an important role.

---

## Research Question
Are SAT scores influenced by factors beyond academic ability?

We examine whether variables such as socioeconomic status, school funding, and demographic characteristics correlate with SAT performance across schools.

Our hypothesis is that SAT scores are not purely measures of academic ability. Instead, socioeconomic conditions and access to educational resources may significantly influence outcomes. :contentReference[oaicite:0]{index=0}

---

## Dataset
The dataset used in this project is **MA Public Schools 2017**, which contains demographic and performance data for public schools in Massachusetts.

Key variables include:

- Average SAT scores
- Percentage of economically disadvantaged students
- School district expenditure per pupil
- Teacher salary
- Percentage of students attending college
- Ethnicity distribution
- Gender ratios

The dataset was obtained from Kaggle and includes information on Massachusetts public schools in 2017. :contentReference[oaicite:1]{index=1}

### Dataset Limitations
- Includes only Massachusetts schools
- Uses the older SAT scoring scale
- Contains only public schools

Because of these limitations, results cannot be generalized to all U.S. schools.

---

## Data Processing
Before conducting the analysis, several preprocessing steps were performed:

- Removed elementary and middle schools that do not report SAT scores
- Removed irrelevant variables such as AP scores
- Renamed variables for clarity
- Converted the old SAT scoring scale to the current scale

These steps ensured consistency and relevance for modeling and analysis.

---

## Exploratory Data Analysis (EDA)

Exploratory analysis was conducted to understand patterns in the data using:

- Histograms and boxplots to examine variable distributions
- Scatter plots to identify relationships between variables
- Heatmaps to visualize geographic patterns and correlations

For example, counties with higher percentages of economically disadvantaged students tended to show lower average SAT scores. :contentReference[oaicite:2]{index=2}

---

## Modeling Approaches

Three modeling approaches were used to examine relationships between SAT scores and explanatory variables.

### Multiple Linear Regression
Used to estimate the relationship between SAT scores and socioeconomic and demographic factors.

### Relaxed LASSO
Used for feature selection and identifying the most influential predictors of SAT performance.

### Decision Tree
Used to visualize nonlinear relationships and understand variable interactions.

---

## Key Findings

Several variables were found to be significantly associated with SAT scores.

Negative correlations:
- Percentage of economically disadvantaged students
- Percentage of African American students

Positive correlations:
- Percentage of Asian students
- Percentage of multi-racial students
- Percentage of alumni attending college

These findings suggest that socioeconomic conditions and educational environment influence SAT performance. :contentReference[oaicite:3]{index=3}

---

## Implications
The results suggest that SAT scores may not be purely standardized measures of academic ability. Differences in socioeconomic status, school resources, and educational environment may contribute to disparities in test outcomes.

Improving access to educational resources and preparation opportunities may help reduce these disparities. :contentReference[oaicite:4]{index=4}

---

## Limitations

This analysis has several limitations:

- The dataset only includes Massachusetts public schools
- Results cannot be generalized to private schools
- Demographic compositions vary significantly across states

Therefore, findings should be interpreted within the context of Massachusetts public schools.

---

## Repository Structure

```text
sat-socioeconomic-analysis/
├── README.md
├── analysis/
│   └── Wharton_Final_Project_clean.Rmd
├── data/
│   └── MA_Public_Schools_2017.csv
│   └── data.final.csv
└── Analyzing Factors Affecting SAT Scores.pdf
```

- **analysis/** contains the R Markdown file used for data cleaning, exploratory analysis, and modeling.  
- **data/** contains the datasets used in the analysis.  

---

