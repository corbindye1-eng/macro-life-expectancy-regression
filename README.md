# Macroeconomic Drivers of Life Expectancy
**An Econometric Regression Analysis: Developed vs. Developing Nations**

## Executive Summary
This project utilizes a semi-standardized Ordinary Least Squares (OLS) regression model to isolate the macroeconomic/social drivers of life expectancy across all World Health Organization (WHO) recognized countries. By splitting the countries in the WHO data set based on wether they were developed or developing, the model mathematically proves that as economies develop, the most important aspects to human longevity fundamentally shift from foundational survival to lifestyle and resource optimization. The insights generated are designed to guide targeted social investments and policies.

## Tech Stack & Skills
* **Language:** Python
* **Python Libraries:** Pandas, NumPy, Statsmodels, Matplotlib, Seaborn
* **Statistical Tools:** Ordinary Least Squares Regression, Semi-Standardization, Residual Diagnostics (Q-Q Plots, Skewness analysis)

## Key Findings & Policy Implications

**1.Developing Nations: The Survival Frontier**
* **Top Factors:** HIV/AIDS, Adult Mortality, and Schooling.
* **Main Insights:** Lifespan in developing countries are mostly affected by health crises and basic infrastructure. 
* **Policy Action:** Social capital must focus on infectious disease containment and education as the ultimate tool to improve life expectancy.

**2.Developed Nations: The Lifestyle Frontier**
* **Top Factors:** Income Composition of Resources, Alcohol, and Thinness (1-19 Years).
* **Main Insights:** Once basic societal needs are met, the effect of a country's raw diminishes. Longevity is rather mostly affected by wealth distributed and lifestyle choices.
* **Policy Action:** Investment must pivot away from basic infrastructure and toward health choices, substance abuse intervention, and equitable resource allocation.

## Methodology: Semi-Standardized Regression
To ensure both mathematical rigor and business interpretability, this model employs a **semi-standardized approach**:
* **Independent Variables:** Standardized (Z-scored) to eliminate scale differences (e.g., comparing raw GDP to years of schooling). This allows us to rank variables on the same scale.
* **Dependent Variable:** Left unstandardized (raw years) to ensure coefficients remain interpretable (e.g., A 1-standard-deviation improvement in schooling yields X real-world years of life).

## Repository Structure
```text
├── Data/
│   └── life_expectancy_data.csv       # Raw WHO panel data
├── Notebook/
│   └── life_expectancy_analysis.ipynb # Core OLS pipeline and EDA
├── LICENCE                            #Code Usage Licence             
├── README.md                          # Project documentation
└── requirements.txt                   # Python dependencies
