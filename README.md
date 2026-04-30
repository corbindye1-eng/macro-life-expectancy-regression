# Macroeconomic Drivers of Life Expectancy
**An Econometric Regression Analysis: Developed vs. Developing Nations**

## Executive Summary
This project utilizes a semi-standardized Ordinary Least Squares (OLS) regression pipeline to isolate the macroeconomic and social drivers of global life expectancy. By splitting World Health Organization (WHO) panel data into developed and developing cohorts, the model mathematically proves that as economies mature, the bottlenecks to human longevity fundamentally shift from foundational survival to lifestyle and resource optimization. The insights generated are designed to guide targeted social investment and macroeconomic policy.

## Tech Stack & Skills
* **Language:** Python
* **Libraries:** Pandas, NumPy, Statsmodels, Matplotlib, Seaborn
* **Statistical Methods:** Ordinary Least Squares (OLS) Regression, Z-Score Standardization (Semi-standardized approach), Residual Diagnostics (Q-Q Plots, Skewness analysis)
* **Domain Context:** Macroeconomics, Public Health Policy, Social Investment Strategy

## Key Findings & Policy Implications

**1.Developing Nations: The Survival Frontier**
* **Top Drivers:** HIV/AIDS, Adult Mortality, and Schooling.
* **The Insight:** Lifespan here is strictly capped by systemic health crises and baseline infrastructure. 
* **Policy Action:** Social capital must prioritize infectious disease containment and focus on primary education as the ultimate long-term economic lever.

**2.Developed Nations: The Lifestyle Frontier**
* **Top Drivers:** Income Composition of Resources, Alcohol, and Thinness (1-19 Years).
* **The Insight:** Once basic survival is met, raw GDP loses its impact. Longevity becomes dictated by how wealth is distributed and behavioral/mental health trends.
* **Policy Action:** Investment must pivot away from basic infrastructure and toward mental health, substance abuse intervention, and equitable resource allocation.

## Methodology: Semi-Standardized Regression
To ensure both mathematical rigor and business interpretability, this model employs a **semi-standardized approach**:
* **Independent Variables (Features):** Standardized (Z-scored) to eliminate scale discrepancies (e.g., comparing raw GDP to years of schooling). This allows for definitive ranking of variable importance.
* **Dependent Variable (Target):** Left unstandardized (raw years) to ensure coefficients remain highly interpretable for business stakeholders (e.g., *"A 1-standard-deviation improvement in schooling yields X real-world years of life"*).

## Repository Structure
```text
├── Data/
│   └── life_expectancy_data.csv       # Raw WHO panel data
├── Notebook/
│   └── life_expectancy_analysis.ipynb # Core OLS pipeline and EDA                 
├── README.md                          # Project documentation
└── requirements.txt                   # Python dependencies
