## Table of Contents

- [Uses](#uses)
- [Objective](#objective)
- [Dataset](#dataset)
  - [Original Dataset](#original-dataset)
  - [Combined Dataset](#combined-dataset)
- [Methods](#methods)
  - [Data Visualization](#data-visualization)
  - [Hypothesis](#hypothesis)
  - [Test Statistic](#test-statistic)
- [Results](#results)
  - [JMP Analysis](#jmp-analysis)
- [Conclusion](#conclusion)

# Uses
- Contingency tables
- Chi-squared distribution
- Test for Independence

# Objective
Determine if there is a dependence between gender and favourite type of snack food.

# Dataset

## Original Dataset

|                   | Sweets (Candy & Baked Goods) | Ice Cream | Chips & Pretzels | Fruits & Vegetables | Total |
|-------------------|-------------------------------|-----------|------------------|----------------------|-------|
| Male              | 8                             | 9         | 12               | 7                    | 36    |
| Female            | 6                             | 9         | 4                | 0                    | 19    |
| Total             | 14                            | 18        | 16               | 7                    | 55    |

Female fruits and vegetables counts were 0, so I combined Fruits & Vegetables with Chips & Pretzels. If the expected count for a category is too low, it is recomended to combine that category with adjacent categories to achieve the minimum expected count. 

## Combined Dataset
|                   | Sweets (Candy & Baked Goods) + Ice Cream  | Chips & Pretzels + Fruits & Vegetables | Total |
|-------------------|-------------------------------------------|----------------------------------------|-------|
| Male              | 17                                        | 19                                     | 36    |
| Female            | 15                                        | 4                                      | 19    |
| Total             | 32                                        | 23                                     | 55    |

From the combined chart, it looks like men prefer salty and savoury snacks, and women prefer sweet snacks.

# Methods
## Data Visualization
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Test%20for%20Independence/Screenshot%202024-02-02%20at%2012.10.46%20PM.png)

In the Mosaic plot, the ratios are different, indicating that there might be a dependence between gender and the favorite type of snack food.

## Hypothesis  
H0: There is no dependence between gender and favorite type of snack food.
H1: There is a dependence between gender and favorite type of snack food.

## Test Statistic
- The test statistic used in this scenario is a Chi-square value and has a null distribution with (2-1)(2-1) = (2-1)(2-1) = 1 degrees of freedom.
- The Chi-square test statistic measures the difference between the expected and observed frequencies in a contingency table. 
- The expected frequency is calculated under the assumption of independence between the two variables. If the observed and expected frequencies are similar, the Chi-square value is small, suggesting that any differences are likely due to random chance. However, if the Chi-square value is larger than the critical value, it suggests a significant difference between observed and expected frequencies, and this may indicate a relationship between the variables.

| Gender |        Favorite Snack         | Observed |   Expected    |   Difference   |     Square    |     Ratio     |
|--------|-------------------------------|----------|---------------|----------------|---------------|---------------|
| Male   | Sweets (Candy & Baked Goods) + Ice Cream  | 17        | 20.9454545455 | -3.9454545455 | 15.5666115706 | 0.74319760102 |
| Male   | Chips & Pretzels + Fruits & Vegetables    | 19        | 15.0545454545 | 3.9454545455  | 15.5666115706 | 0.22272727273 |
| Female | Sweets (Candy & Baked Goods) + Ice Cream  | 15        | 11.0545454545 | 3.9454545455  | 15.5666115706 | 1.40816387564 |
| Female | Chips & Pretzels + Fruits & Vegetables    | 4         | 7.94545454545 | -3.94545454545| 15.5666115702 | 1.95918452257 |

The test statistic is the sum of all the ratios, so Ts = 4.33325. 

We reject H0 because 4.33325 > 3.8415.  We have statistically significant evidence at α=0.05 to show that H0 is false, or based on the observed data, there is enough evidence to conclude a significant relationship between the variables "Gender" and "Favorite Snack."

# Results
## JMP Analysis
Using JMP:

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Test%20for%20Independence/Screenshot%202024-02-04%20at%207.16.16%20PM.png)

The p value is .0200 for the likelihood ratio and Pearson Chi-Square Test, which means the p-value is less than 0.05 suggesting that there is evidence to reject the null hypothesis at a significance level of 0.05.

# Conclusion: 

We have statistically significant evidence in JMP that favorite snack food is not equal among genders. This
agrees with our hypothesis test and mosaic plot comparison from before. The variables are dependent.







