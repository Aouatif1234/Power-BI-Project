# Power BI Project - Data Professionals Salary Survey

This repository contains a Power BI report based on the survey data collected from data professionals. The report explores various aspects of job satisfaction, career challenges,  and salary expectations in the field of data science.

## Report Overview

The report provides insights into:
- **Job Satisfaction**: Ratings on satisfaction with management, upward mobility, and work-life balance.
- **Career Challenges**: How difficult respondents found it to break into the data field.
- **Job Preferences**: Key factors data professionals consider when searching for a new job (e.g., remote work, better salary).
- **Demographics**: Breakdown of gender, age, ethnicity, and education levels.
- **Salary Analysis**: Average salary computed for each respondent and exploration of salary trends based on demographic and professional factors.


## Data Cleaning & Preparation

- The dataset was cleaned by removing missing and inconsistent entries.
- The **average salary** was computed for each respondent based on the available salary data provided in the survey.

## Calcul du KPI - Satisfaction au Travail

Un des KPIs dans ce projet mesure le pourcentage de professionnels des données satisfaits de leur équilibre travail/vie personnelle. La formule DAX suivante est utilisée pour calculer ce KPI :

### Formule DAX

DAX
KPI_Satisfaction_High = 
DIVIDE(
    COUNTROWS(FILTER('Data Professional Survey', 'Data Professional Survey'[Q6 - How Happy are you in your Current Position with the following? (Work/Life Balance)] > 4)),
    COUNTROWS('Data Professional Survey')
)

## File Description

- `analysis_data.pbix`: The Power BI report file that contains visualizations and analysis of the survey data.

## Usage

To view the report:
1. Download the `.pbix` file.
2. Open it using [Power BI Desktop](https://powerbi.microsoft.com/desktop).

## Visualizations

The following visualizations are included in the report:
- **Bar charts**: Job satisfaction metrics and career challenges.
- **Pie charts**: Gender and age group distributions.
- **Maps**: Geographic distribution of respondents.
- **Tables**: Salary breakdowns and factors affecting job preferences.

