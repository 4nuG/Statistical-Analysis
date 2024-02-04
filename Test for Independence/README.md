# Uses
- Contingency tables
- Chi-squared distribution
- Test for Independence

# Objective
Determine if there is a dependence between gender and favourite type of snack food.

# Dataset

|                   | Sweets (Candy & Baked Goods) | Ice Cream | Chips & Pretzels | Fruits & Vegetables | Total |
|-------------------|-------------------------------|-----------|------------------|----------------------|-------|
| Male              | 8                             | 9         | 12               | 7                    | 36    |
| Female            | 6                             | 9         | 4                | 0                    | 19    |
| Total             | 14                            | 18        | 16               | 7                    | 55    |

Female fruits and vegetables counts were 0, so I combined Fruits & Vegetables with Chips & Pretzels.

|                   | Sweets (Candy & Baked Goods) + Ice Cream  | Chips & Pretzels + Fruits & Vegetables | Total |
|-------------------|-------------------------------------------|----------------------------------------|-------|
| Male              | 17                                        | 19                                     | 36    |
| Female            | 15                                        | 4                                      | 19    |
| Total             | 32                                        | 23                                     | 55    |

From the combined chart, it looks like men prefer salty and savoury snacks, and women prefer sweet snacks.

# Methods
## Data Visulization
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
| Male   | Sweets (Candy & Baked Goods)  | 8        | 9.16363636364 | -1.16363636364 | 1.35404958679 | 0.14776334776 |
| Male   | Ice Cream                     | 9        | 11.7818181818 | -2.7818181818  | 7.73851239659 | 0.65681818181 |
| Male   | Chips & Pretzels              | 12       | 10.4727272727 | 1.5272727273   | 2.33256198355 | 0.22272727273 |
| Male   | Fruits & Vegetables           | 7        | 4.58181818182 | 2.41818181818  | 5.84760330578 | 1.27626262626 |
| Female | Sweets (Candy & Baked Goods)  | 6        | 9.16363636364 | -3.16363636364 | 10.0085950413 | 1.0922077922  |
| Female | Ice Cream                     | 9        | 6.21818181818 | 2.78181818182  | 7.7385123967  | 1.24449760766 |
| Female | Chips & Pretzels              | 4        | 5.52727272727 | -1.52727272727 | 2.33256198346 | 0.42200956937 |
| Female | Fruits & Vegetables           | 0        | 2.41818181818 | -2.41818181818 | 5.84760330578 | 2.41818181815 |

The test statistic is the sum of all the ratios, so Ts = 7.48042. Since the test statistic is larger than the critical value (3.84), we can reject the null hypothesis. This suggests that, based on the observed data, there is enough evidence to conclude a significant relationship between the variables "Gender" and "Favorite Snack."

p-value: 

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-02-02%20at%202.10.52%20PM.png)

the p value is 0.54

Decision: Fail to reject null hypothesis because p value (.547) is greater than the assumed significance level of .05.

Conclusion: 
There is not enough evidence at a 5% level to claim that that there is no relationship between gender and favorite type of snack food. However failing to reject the null hypothesis does not prove that the null hypothesis is true; it simply means that there is not have enough evidence to confidently reject it based on the sample data.

# Same analysis in JMP:
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Test%20for%20Independence/Screenshot%202024-02-02%20at%202.27.07%20PM.png)

We have statistically significant evidence that favorite snack food is not equal among genders. This
agrees with our hypothesis test and mosaic plot comparison from before. The variables are depend.

