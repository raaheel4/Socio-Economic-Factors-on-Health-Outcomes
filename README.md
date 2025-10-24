# Socio-Economic Determinants and Health Outcomes in India: NFHS-5 District-Level Analysis
This analysis aims to present a comprehensive view of how Socio-Economic Factors shape Health Outcomes, using the microdata from National Family Health Survey (NFHS-5, 2019–21). 
# Project Overview
This project investigates how key socio-economic factors impact child and maternal health outcomes across Indian districts. Through descriptive statistical analysis and visualisation tools, the study examines relationships between education, infrastructure access, and health indicators such as anaemia and malnutrition. The intent is to clarify the socio-developmental drivers of health disparities in India and inform evidence-based policy recommendations.
# Repository Contents
* **[/dataset](https://github.com/raaheel4/Socio-Economic-Factors-on-Health-Outcomes/tree/main/dataset)**: Contains the raw NFHS-5 district-level dataset and a cleaned version used for the analysis.
*  **[/code](https://github.com/raaheel4/Socio-Economic-Factors-on-Health-Outcomes/tree/main/code)**: Includes the Jupyter notebooks used for data sourcing, cleaning, analysis, and visualization.
* **[/graphs](https://github.com/raaheel4/Socio-Economic-Factors-on-Health-Outcomes/tree/main/graphs)**: Stores the key plots and figures generated during the analysis.
# Approach and Methodology
#### 1. *Data Cleaning and Sourcing*
* Source: NFHS-5 District Factsheet taken from MoHFW archive and from SaiSiddhardhaKalla's GitHub Repository (https://github.com/SaiSiddhardhaKalla/NFHS/blob/main/India.csv)
* The district-level dataset was cleaned for variables like literacy, household infrastructure (electricity, sanitation, clean fuel), insurance, and health outcomes (anaemia, stunting, underweight) were extracted and standardized for analysis.
* Since the NFHS survey does not include a direct income questionnaire, certain proxies such as access to electricity, subscription to insurance schemes, and others have been used to approximate household economic status. These proxies were carefully selected to accurately capture the influence of socio-economic factors on health outcomes.
* Handle missing and or negative values.
#### Summary of Key Indicators (District-level)
| Indicator | Mean | Min | Max | Std. Dev. |
| :--- | :---: | :---: | :---: | :---: |
| Female Literacy Rate (%) | 74.3 | 38.6 | 99.7 | 12.3 |
| Child Anaemia Rate (%) | 65.8 | 25.0 | 95.0 | 24.9 |
| Stunting Rate (%) | 33.5 | 13.2 | 60.6 | 8.5 |
| Households with Electricity (%) | 97.0 | 68.4 | 100.0 | 4.4 |
#### 2. *Data Analysis and Visualisation*
* Distribution plots (histograms, boxplots) were used to understand the spread, typical values, and outliers for each critical indicator across all districts.
* Relationship & Correlation: Scatterplots compared socio-economic measures with health outcomes (e.g., literacy vs. anaemia), and a correlation matrix summarized the strength of associations between variables.
* Group Comparisons: Districts were grouped by state and by quartiles of development proxies (e.g., electricity access) to highlight interstate and developmental disparities in health outcomes.
#### 3. *Visualization*
* Key findings were presented through clear, annotated plots, making trends and geographic variations easily comprehensible.
#### 4. *Summary Table*
* All main indicators with mean, min, max, and standard deviation.
# Key Findings and Insights
#### 1. *Descriptive Distribution Analysis*
* Histograms and boxplots show that health outcomes and socio-economic indicators have wide, often skewed, distributions across Indian districts. For example, children’s anaemia rates peaked in the 60-70% range, with the majority of districts showing moderate to high prevalence. Women’s literacy rates and electricity access varied greatly, confirming persistent geographic and social disparities.
#### 2. *Correlation & Bivariate Analysis*
* Pearson correlation coefficients highlighted strong negative relationships between socio-economic development and negative health outcomes: 
    * Districts with higher female literacy rates consistently had lower rates of childhood anaemia and malnutrition. Access to electricity and clean cooking fuel were reliably linked with improved nutritional outcomes for children. 
    * The correlation matrix heatmap revealed moderate to strong associations (often |r| > 0.5) between improved infrastructure indicators and lower rates of child undernutrition.
#### 3. *Regression & Predictive Modeling*
Simple linear regression models (visualized in scatterplots with fitted lines) showed that each 10 percentage point increase in female literacy predicted a statistically significant reduction in anaemia and stunting rates at the district level. These models provided evidence for the predictive value of socio-economic variables. When grouping districts by quartiles of infrastructure/income access like electricity, boxplots demonstrated that districts in the best-developed quartiles had substantially lower mean rates of negative health outcomes.
#### 4. *Grouped Comparisons & State Variation*
Boxplots and grouped summaries revealed that states like Kerala, Tamil Nadu, and Punjab consistently outperformed states like Jharkhand, Bihar and Uttar Pradesh in both development proxies and health indicators. Even within advanced states, intrastate disparities persisted, which underlines the importance of sub-state (district) analysis.
#### 5. *Key Policy and Research Implications*
The combined regression, correlation, and groupwise comparisons strengthen the evidence for a causal link between women's education, basic amenities, and health improvement. The analysis goes beyond describing rates—it quantifies associations and clearly visualizes actionable disparities. The study’s findings suggest that integrated interventions (simultaneously addressing education, infrastructure, and health services) are likely to yield the greatest improvements in child and maternal health outcomes across India.
# Policy Implications:
* The results confirm that improving education and basic infrastructure in lagging districts offers huge potential to reduce anaemia, malnutrition and other related health risks. Comprehensive, integrated development strategies—targeting both social and physical determinants are essential for closing health gaps across India.
# Limitations:
* District-level infant mortality and fertility rates were not available; state-level proxies were noted.
* The analysis is cross-sectional and does not take into account causal mechanisms, but highlights strong associations and disparities.
# Statistical note:
All results are exploratory and based on available district-level cross-sectional NFHS-5 data; correlations/regressions do not establish causality but strongly indicate priority areas for further intervention and research.


