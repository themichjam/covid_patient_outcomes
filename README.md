# COVID-19 Mortality Prediction Project

This project develops a machine learning model to predict the mortality of COVID-19 patients based on their clinical data. The model is built using R and leverages several libraries for data manipulation, visualization, and modeling.

## Project Structure

- `covid_analysis.R`: Main R script containing the code for data importing, preprocessing, visualization, model building, and evaluation.
- `data/`: Directory containing the dataset used in the project.
- `README.md`: This file, providing an overview of the project.

## Dataset

The dataset used in this project contains anonymized patient data related to COVID-19, including pre-existing conditions and outcomes. It features 21 unique attributes for over a million patients. The data is sourced from a public health database (please replace with the actual source if known).

### Attributes Include

- `sex`: Gender of the patient (Male or Female).
- `age`: Age of the patient.
- `classification`: COVID-19 test results.
- `patient_type`: Hospitalization status.
- `pneumonia`: Presence of pneumonia.
- `pregnancy`: Pregnancy status.
- `diabetes`: Presence of diabetes.
- `copd`: Chronic Obstructive Pulmonary Disease status.
- `asthma`: Asthma status.
- `inmsupr`: Immunosuppression status.
- `hypertension`: Hypertension status.
- `cardiovascular`: Cardiovascular issues.
- `renal_chronic`: Chronic renal disease status.
- `other_disease`: Other diseases.
- `obesity`: Obesity status.
- `tobacco`: Tobacco usage.
- `medical_unit`: Type of medical care unit.
- `intubed`: Intubation status.
- `icu`: Intensive Care Unit admission.
- `death`: Mortality outcome.

## Installation

To run this project, you will need R installed on your system along with the following R packages:
- `tidyverse`
- `readr`
- `caret`
- `ROSE`

You can install these packages using R commands like:

```r
install.packages("tidyverse")
install.packages("readr")
install.packages("caret")
install.packages("ROSE")
```

## Usage
To run the analysis, navigate to the project directory in RStudio or any R environment and execute the script covid_analysis.R.

## Health Quality of Life (QoL) Analysis

### Overview
Health Quality of Life (QoL) is a critical component in understanding the broader impacts of COVID-19 on patients' lives, especially after the initial infection period. This project assesses QoL through various clinical indicators, including the extent of medical interventions required (e.g., ICU admission, need for intubation) and outcomes such as length of hospital stay and post-treatment health status.

### Methodology
We use patient data to create indices that reflect the QoL post-COVID-19 infection. This involves:
- Analyzing the severity of symptoms and subsequent recovery patterns.
- Assessing the impact of COVID-19 on daily living activities and long-term health consequences.

### Insights
By correlating clinical outcomes with patient demographics and pre-existing conditions, we aim to identify factors that significantly affect the QoL in COVID-19 patients. These insights can help healthcare providers improve treatment plans and support mechanisms for recovery.

## Indirect Treatment Comparison

### Overview
Indirect treatment comparison involves analyzing the effectiveness of different COVID-19 treatments administered across various patient groups within the dataset. This analysis is crucial for understanding which treatments yield the best outcomes under specific conditions.

### Methodology
We compare patient groups based on the type of treatment received, including medication, ICU support, and mechanical ventilation, among others. Statistical methods, such as propensity score matching and multivariable regression models, are used to adjust for confounding factors.

### Insights
The goal is to provide evidence-based recommendations on COVID-19 treatments, highlighting which therapies are most effective for particular patient profiles, including varying ages, pre-existing conditions, and severity of symptoms.

## Time-to-Event Analysis

### Overview
Time-to-Event (Survival) analysis is employed to determine the duration from the onset of COVID-19 symptoms to various endpoints, such as recovery or death. This analysis helps to understand the progression of the disease over time and factors influencing patient survival.

### Methodology
We use Kaplan-Meier estimates and Cox proportional hazards models to analyze time-to-event data. These models help to assess the impact of different variables, such as age, gender, and comorbidities, on the time to recovery or mortality.

### Insights
The findings from this analysis provide crucial insights into the risk factors for severe outcomes in COVID-19 patients and can guide public health decisions and patient management strategies to improve survival rates.

## Conclusion

The combined insights from the Health QoL, Indirect Treatment Comparisons, and Time-to-Event analyses enable a comprehensive understanding of the effects of COVID-19. These analyses aid in optimizing treatment protocols and improving patient care outcomes across diverse populations.

This project not only aids in clinical decision-making but also helps policymakers in crafting guidelines that can enhance patient care during and after the pandemic.

