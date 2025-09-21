# Predictive-Modeling-of-Student-Mathematics-Performance-Multinomial-Logistic-Regression-Analysis

📄 Full Report: [View Analysis](Predictive Modeling of Student Mathematics Performance/ Multinomial Logistic Regression Analysis.html)

## Overview
This project develops and evaluates a multinomial logistic regression model to predict mathematics achievement levels (Poor, Average, Good, Excellent) among 358 final-year Junior High School students in Oforikrom Municipality, Ghana, based on a 2024 survey. Exploratory analyses reveal 62% high proficiency, with significant associations between performance and factors like math enjoyment, family support, and homework frequency (p<0.05). The core model (AIC=611.0) identifies math enjoyment (OR=36.38 for Excellent vs. Poor, p=0.003) and family support (OR=8.31 for Good vs. Poor, p=0.018) as key predictors, achieving 55.7% accuracy (Kappa=0.333) and AUCs of 0.693–0.789. Findings emphasize fostering intrinsic motivation and parental involvement to address performance gaps, offering actionable insights for educators and policymakers to enhance equitable mathematics outcomes in resource-constrained settings.

## Dataset Summary
- **Source**: Secondary survey data from final-year Junior High School students in three schools, Oforikrom Municipality, Ghana (2024).
- **Sample Size**: 358 respondents.
- **Key Variables**: Proficiency levels (Poor, Average, Good, Excellent); demographics (age, gender); socio-economic (family support, financial status, pocket money); behavioral (math enjoyment, homework frequency, study hours, attendance); school-related (teaching quality, teacher relations, extra classes, class size); environmental (classroom conduciveness, ventilation, home environment).

- 
## Objectives
- Examine relationships between socio-economic, environmental, school-related, and behavioral factors and students’ mathematics achievement across proficiency levels.
- Develop a predictive multinomial logistic regression model to quantify factor impacts on mathematics performance.
- Evaluate the model's classification performance, including accuracy, confusion matrix, and discriminatory ability via ROC curves.
- Identify influential factors and derive practical implications for interventions to improve mathematics achievement.



## Methods
- Descriptive statistics (frequencies, percentages, means) and visualizations (bar plots, boxplots) for exploratory analysis of distributions and associations.
- Inferential tests including chi-square and Fisher’s exact tests for categorical associations between factors and proficiency levels.
- Multinomial logistic regression for predictive modeling, with model selection via AIC/BIC, multicollinearity checks (VIF), and evaluation using accuracy, Kappa, confusion matrix, sensitivity/specificity, F1-score, and ROC-AUC.

## Key Findings
- High proficiency dominates (62%, n=222).  strong family support (77% "Good" rating vs. 44% for low proficiency).
- Significant associations (p<0.05) with behavioral factors like math enjoyment (84.2% "Yes" in high vs. 40% in low) and homework frequency (89.6% regular in high vs. 52% in low), plus socio-economic (family support) and school-related (teacher ratings) elements.
- Core model highlights math enjoyment (OR=36.38, p=0.003) and family support (OR=8.31, p=0.018) as top predictors; accuracy 55.7% with strong mid-level classification (Good: 78% sensitivity) but challenges for extremes (Poor: 28.6%, Excellent: 24%).
- AUCs indicate fair-good discrimination (0.693–0.789); misclassifications suggest overestimation of low performers, emphasizing need for targeted support.



## How to Reproduce the Analysis
### Requirements
- R (version 4.0 or higher)
- RStudio
- R packages: tidyverse, ggplot2, dplyr, nnet (for multinomial logistic), pROC (for ROC), car (for VIF), broom

### Steps
1. Clone this repository.
2. Open `analysis.Rmd` in RStudio.
3. Install required packages if not already installed (e.g., `install.packages(c("tidyverse", "nnet", "pROC"))`).
4. Knit the R Markdown file to generate the HTML report.
Data not included due to confidentiality. Please contact me for collaboration requests.

## Repository Structure
├── analysis.Rmd         # R Markdown source file  
├── analysis.html        # Knitted HTML report  
├── figures/             # Plots and visualizations  
├── README.md            # Project description  

## License / Citation
This project is for academic and research purposes. Please cite appropriately if referenced, e.g., Sei, Lawrence. (2025). Predictive Modeling of Student Mathematics Performance: Multinomial Logistic Regression Analysis.
