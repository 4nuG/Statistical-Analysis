# Uses
- Contingency tables
- Chi-squared distribution
- Test for Independence

# Objective
Determine if there is a dependence between gender and favorite type of snack food.

# Dataset

|                   | Sweets (Candy & Baked Goods) | Ice Cream | Chips & Pretzels | Fruits & Vegetables | Total |
|-------------------|-------------------------------|-----------|------------------|----------------------|-------|
| Male              | 8                             | 9         | 12               | 7                    | 36    |
| Female            | 6                             | 9         | 4                | 0                    | 19    |
| Total             | 14                            | 18        | 16               | 7                    | 55    |

Female fruits and vegetables counts was 0 so I combined Fruits & Vegetables with Chips & Pretzels.

|                   | Sweets (Candy & Baked Goods) | Ice Cream | Chips & Pretzels | Fruits & Vegetables | Total |
|-------------------|-------------------------------|-----------|------------------|----------------------|-------|
| Male              | 8                             | 9         | 12               | 7                    | 36    |
| Female            | 6                             | 9         | 4                | 0                    | 19    |
| Total             | 14                            | 18        | 16               | 7                    | 55    |

# Methods
## Data Visulization
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Test%20for%20Independence/Screenshot%202024-02-02%20at%2012.10.46%20PM.png)

In the Mosaic plot, the ratios are different indicating that there might be a dependence between gender and favorite type of snack food.

## Hypothesis 
H0: There is no relationship between gender and favorite type of snack food.
H1: There is an association between gender and favorite type of snack food

## Test Statistic
The test statistic is a Chi-square value and has a null distribution with (2-1)(2-1) = (2-1)(2-1) = 1 degrees of freedom.
The Chi-square test statistic measures the difference between the expected and observed frequencies in a contingency table. 
The expected frequency is calculated under the assumption of independence between the two variables. If the observed and expected frequencies are similar, the Chi-square value is small, suggesting that any differences are likely due to random chance. However, if the Chi-square value is large, it suggests a significant difference between observed and expected frequencies, and this may indicate a relationship between the variables.
After calculating the Chi-square value, you would compare it to the critical value from the Chi-square distribution with 3 degrees of freedom to determine whether to reject the null hypothesis. If the Chi-square value is greater than the critical value, you may have evidence to reject the null hypothesis, suggesting a significant relationship between gender and favorite type of snack food.

| Gender | Favorite Snack | Observed | Expected | Difference | Square | Ratio   |
|--------|----------------|----------|----------|------------|--------|---------|
| Male   | Sweets (Candy & Baked Goods) + Fruits & Vegetables | 15   | 13.5   | 1.5        | 2.25   | 0.167   |
| Male   | Chips & Pretzels + Ice Cream                          | 21   | 21.857 | -0.857     | 0.734  | 0.034   |
| Female | Sweets (Candy & Baked Goods) + Fruits & Vegetables | 6    | 7.125  | -1.125     | 1.266 | 0.178   |
| Female | Chips & Pretzels + Ice Cream                          | 13   | 11.536 | 1.464      | 2.143 | 0.186  |

The test statistic is the sum of all the ratios, so Ts = .56

p-value: 

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-02-02%20at%202.10.52%20PM.png)

the p value is 0.54

Decision: Fail to reject null hypothesis because p value (.547) is greater than the assumed significance level
of .05.

Conclusion: There is not enough evidence at a 5% level to claim that that there is no relationship between
gender and favorite type of snack food.

# Same analysis in JMP:
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Test%20for%20Independence/Screenshot%202024-02-02%20at%202.27.07%20PM.png)

Conduct the analysis in JMP. Compare answers. Are they the same? Please include the JMP
output.

## points
1. 3.75 / 3.75 pts 
2. 2 / 2 pts Sorry, In the Lab, I made wrong statement. If their proportions are not the same, it indicates they have some relationship. 
3. a. 2 / 2 pts b. 2 / 2 pts c. 5 / 5 pts d. 1 / 1 pt e. 1 / 1 pt f. 1 / 1 pt The conclusion should include the significance level. 
4. 2 / 2 pts
