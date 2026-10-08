# U.S. Industry Wage Analysis, 2017–2024

This is an R-based analysis of wages and salaries per full-time equivalent (FTE) employee across major U.S. industries using data from the U.S. Bureau of Economic Analysis (BEA), Table 6.6D.

## Research Questions

1. How did wages and salaries per FTE employee differ across major industries in 2024?
2. Which major industries experienced the largest percentage increase between 2017 and 2024?

## Data

- **Source:** U.S. Bureau of Economic Analysis, Table 6.6D
- **Measure:** Wages and salaries per full-time equivalent employee
- **Period:** 2017–2024
- **Scope:** 20 selected major industry categories

The original BEA table contains both broad industries and sub-industries. This project selects broad industry categories to make cross-industry comparisons more consistent.

## Tools

- R
- tidyverse
- ggplot2
- knitr
- R Markdown

## Methods

The analysis:

- imports and cleans the BEA wage table;
- standardizes industry names;
- selects 20 major industry categories;
- calculates percentage wage growth from 2017 to 2024;
- compares 2024 wage levels across industries;
- calculates descriptive statistics including mean, median, standard deviation, minimum, and maximum;
- examines the correlation between 2017 wage levels and subsequent percentage growth;
- visualizes wage levels, wage growth, and 2017–2024 trends for selected industries.

## Key Findings

- The mean 2024 wage across the selected industries was approximately **$95,211**, while the median was **$84,996**.
- The standard deviation was approximately **$41,524**, indicating substantial cross-industry dispersion.
- **Information** had the highest 2024 wages and salaries per FTE employee, at approximately **$186,683**.
- **Accommodation and food services** had the lowest, at approximately **$43,985**.
- The average wage increase from 2017 to 2024 was approximately **35.4%**, compared with a median increase of **33.4%**.
- **Information** experienced the largest percentage increase, at approximately **62.6%**.
- The correlation between 2017 wage levels and percentage growth through 2024 was approximately **-0.11**, suggesting little relationship between initial wage levels and subsequent growth within the selected industries.

## Interpretation

The results show substantial variation in both wage levels and wage growth across industries. High initial wage levels were not strongly associated with faster wage growth over the period.

## Limitations

This analysis is descriptive rather than causal. The wage values are nominal and are not adjusted for inflation. The results therefore should not be interpreted as changes in real purchasing power or as evidence that industry characteristics caused the observed wage changes.

## Suggested Repository Structure

```text
bea-industry-wage-analysis/
├── README.md
├── BEA_Wages_Analysis.Rmd
├── data/
│   └── Table.csv
├── figures/
│   ├── wages_2024.png
│   ├── wage_growth_2017_2024.png
│   └── wage_trends.png
└── report/
    └── BEA_Wages_Final_Project.pdf
```

## Author

Zipeng Zhao
