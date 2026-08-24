# Kansora-Medical-High-Performer-Attrition-Analysis

### Using people analytics to identify the factors most strongly associated with attrition among high-performing employees and translate the findings into practical retention priorities.

## Project overview

This project analyses employee attrition among high-performing employees at Kansora Medical, a fictional Osaka-based medical-device manufacturer with approximately 5,000 employees.

The analysis uses the fictional IBM HR Analytics Employee Attrition dataset. In this case-study scenario, Kansora Medical's People Analytics team has been asked to investigate unwanted attrition among high performers, identify the strongest associated factors, and recommend evidence-based priorities for improving retention.

The analysed population consists of 1,470 employees rated `Excellent` or `Outstanding`, treated in this scenario as representing approximately the top 30% of the company's workforce.

## Objectives

The analysis was guided by four key questions:

- Where is attrition concentrated across the workforce?
- Which factors remain associated with higher or lower attrition after controlling for other workforce characteristics?
- Which findings provide the clearest and most actionable retention priorities?
- Can individual attrition risk be predicted usefully, and would such predictions be appropriate to use in practice?

## Analytical approach

The project followed three main stages.

First, descriptive and bivariate analysis was used to identify initial patterns in attrition. Multivariate logistic regression was then applied to assess which relationships remained after accounting for overlap between factors such as job level, tenure, pay, career experience, work demands, and employee attitudes.

Finally, logistic regression and decision-tree classification models were tested to assess the usefulness of individual-level attrition prediction. Model performance was considered alongside confidentiality, governance, and employee-labelling concerns.

## Key findings

- Attrition was most strongly associated with **work demands and employee experience**. Overtime and frequent business travel were associated with substantially higher attrition odds, while better work-life balance was associated with lower odds.
- Low job involvement and lower satisfaction with the job, work environment, and workplace relationships were also associated with higher attrition.
- Career and development factors showed additional relationships, although these were generally smaller.
- Salary increases and stock-option level showed little independent association with attrition after controlling for other workforce characteristics.
- Predictive models identified some attrition signal, but did not outperform the approximately 84% accuracy achieved by simply predicting that every employee would stay. Individual-level risk scoring was therefore not recommended for management use.

## Business implications

The findings suggest that retention efforts should focus primarily on managing persistent overtime, reviewing excessive business travel, improving work-life balance, and addressing local issues relating to involvement and satisfaction.

Business leaders and HRBPs should use the findings as a framework for local diagnosis and targeted action rather than applying a single organisation-wide solution. Compensation should not be treated as the primary retention lever in isolation.

The analysis also highlights an important People Analytics principle: a technically possible prediction is not automatically an appropriate management tool. Predictive performance, confidentiality, governance, and potential employee impact all need to be considered before individual-level analytics are deployed.

## Limitations

The findings show **association rather than causation**. Some survey-related variables also lack detailed construct definitions, and predictive performance for actual leavers remained limited.

Kansora Medical, its organisational context, and all business assumptions are fictional and are used solely for analytical illustration.

## Files included

- `employee_attrition_analysis.ipynb` – Data preparation, exploratory analysis, regression, predictive modelling, and interpretation
- `ibm_hr_analytics_employee_attrition_and_performance_revised.csv` – Dataset used in the analysis
- `kansora_medical_employee_attrition_analysis_presentation_EN.pdf` – English presentation
- `kansora_medical_employee_attrition_analysis_presentation_JP.pdf` – Japanese presentation
- `presentation_script_EN_JP.pdf` – Bilingual English/Japanese presentation script
- `README.md` – Project overview
