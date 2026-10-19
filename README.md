# Women vs. Men International Football Goals

## Overview
This project investigates whether more goals are scored in women's international football matches than in men's. The analysis uses official FIFA World Cup matches played since January 1, 2002, excluding qualifiers.

## Research Question
Are more goals scored in women's FIFA World Cup matches than in men's?

## Hypotheses
- **Null hypothesis (\(H_0\)):** The mean number of goals per match is the same for women's and men's matches.
- **Alternative hypothesis (\(H_1\)):** The mean number of goals per match is greater for women's matches than men's.

Significance level: **10% (\(\alpha = 0.10\))**

## Data
The analysis uses two datasets:
- `women_results.csv`
- `men_results.csv`

The data is filtered to include only official FIFA World Cup matches from January 1, 2002, onward, excluding qualifiers. Total goals per match are calculated by adding the goals scored by both teams.

## Methodology
- Clean and filter the datasets using pandas.
- Explore sample sizes and goal distributions.
- Assess distribution normality to inform test selection.
- Use the **Wilcoxon–Mann–Whitney test** to compare the two independent groups.
- Compare the p-value with the 10% significance level.

## Results
- **Test:** Wilcoxon–Mann–Whitney
- **P-value:** 0.00511
- **Decision:** Reject the null hypothesis.

Since the p-value is below 0.10, there is statistically significant evidence of a difference between the goal-scoring distributions of men's and women's FIFA World Cup matches.

The direction of the difference should be confirmed by comparing the groups' observed goal-scoring outcomes. The test does not directly establish that women's matches have a higher mean.

## Tools
Python, pandas, SciPy, Matplotlib, Seaborn.

## Conclusion
The hypothesis test identified a statistically significant difference between men's and women's FIFA World Cup match goal-scoring distributions. 
