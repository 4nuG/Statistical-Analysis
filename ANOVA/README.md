# Exploring the Relationship between Coffee Consumption and Physical Activity

Table of Contents
1. [Uses](#uses)
2. [Objective](#objective)
3. [Methods](#methods)
  1. [Data Collection](#data-collection)
  2. [Data Visualization - Association Plot Analysis of MET score and coffee consumption](#data-visualization---association-plot-analysis-of-met-score-and-coffee-consumption)
  3. [Assessment of Assumptions](#assessment-of-assumptions)
  4. [Analysis of Variance (ANOVA)](#analysis-of-variance-anova)
  5. [Post Hoc](#post-hoc)
4. [Conclusions](#conclusions)


## Uses
- ANOVA

## Objective
Caffeine is the world’s most widely used stimulant, with approximately 80% consumed in the form of coffee. 
- Determine whether the average physical activity level varies among the different levels of coffee consumption.

## Methods
### Data Collection
- Participants were randomly recruited from the undergraduate and graduate student populations of universities in the Boston/Cambridge area.
- Participants were asked to report the number of hours they spent per week on moderate (e.g., brisk walking) and vigorous (e.g., strenuous sports and jogging) exercise. Based on these data, the total hours of metabolic equivalent tasks (MET) per week is estimated, a value always greater than 0. 
- The file coffee.exercise.jmp contains simulated MET data for the study participants, based on the amount of coffee consumed. The consumption groups are labeled A - E.

  - A: 1 cup or less of caffeinated coffee consumed per week
  - B: 2 to 6 cups of caffeinated coffee consumed per week
  - C: 1 cup of caffeinated coffee consumed per day
  - D: 2 to 3 cups of caffeinated coffee consumed per day
  - E: 4 or more cups of caffeinated coffee consumed per day

### Data Visualization - Association Plot Analysis of MET score and coffee consumption
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Hypothesis%20Testing%20-%20Proportions/Screenshot%202024-02-01%20at%203.13.01%20PM.png)

The box plots for variables A-E are right skewed shown by the long right tails, so most types of consumption have a low metabolic equivalent tasks per week score and only some have a higher score. All categories have outliers on the right tail raising the MET per week mean which is 26.67684. The mean MET per week does not fall in the 95% confidence interval of A and B where A is below and B is above. This is an unbalanced design because the sample size in each group is not equal.

### Assessment of Assumptions 
- Assumptions: The assumptions for the analysis method (ANOVA)
  - All samples are drawn randomly and independently from one another with no pairing or underlying structure.
    - The participants were randomly selected in the Boston area.
    - ![image](https://github.com/4nuG/Statistical-Analysis/blob/main/ANOVA/Screenshot%202024-02-01%20at%203.33.51%20PM.png)
    - In the column 4 (order collected) vs residual graph, there is no pattern and random scatter. This makes sense as there is no relation between groups.
  - Each sample is from a normally distributed population
    - ![image](https://github.com/4nuG/Statistical-Analysis/blob/main/ANOVA/Screenshot%202024-02-01%20at%203.42.23%20PM.png)
    - The lines are relatively linear and do not have a skew so there is normallity in the groups.
  - Standard deviations are equal
    - ![image](https://github.com/4nuG/Statistical-Analysis/blob/main/ANOVA/Screenshot%202024-02-01%20at%203.46.42%20PM.png)
    - **Interquartile Ranges (IQRs):**
      - 𝐼𝑄𝑅𝐴 = 𝑄3 - 𝑄1 = 35.235 - 12.605 = 22.63
      - 𝐼𝑄𝑅𝐵 = 41.25 - 14.665 = 26.585
      - 𝐼𝑄𝑅𝐶 = 39.28 - 13.4 = 25.88
      - 𝐼𝑄𝑅𝐷 = 36.125 - 12.84 = 23.285
      - 𝐼𝑄𝑅E = 36.215 - 11.275 = 24.94
    - **Largest IQR:** 26.585
    - **2 times Smallest IQR:** 2 times 22.63 = 45.26
    - **Comparison:** Largest IQR < 2 times Smallest IQR, so standard deviations must be equal for all, which means the average distance that the data is from the mean for each group seems to be the same.
      
### Analysis of Variance (ANOVA)
Even with the unbalanced design, we can conduct an analysis to determine whether the average physical activity level varies among the different levels of coffee consumption.
- Parameter of interest: Mean MET per week for different levels of coffee consumption.     
- Hypothesis
  - Ho: μA = μB = μC = μD = μE
  - Ha: At least one pair of means from different categories are different from each other.
- Test Statistic (from ANOVA table from JMP)
  - F₀ = MST/MSE = 2577.28/294.90 = 8.7396
- Rejection criteria: P value method
  - P - value = P(F > F₀) < 0.001
- Decision: Reject H₀. The p-value (0.001) is less than the assumed critical value (0.05).
- Conclusion: There is sufficient evidence at a 5% significance level to warrant the claim that at least one pair of means from the different categories are different from each other.
  
### Post Hoc
- Having established a significant difference through the rejection of the null hypothesis in the ANOVA analysis, the next step is to identify which specific groups exhibit statistically significant differences. This is accomplished through the application of a post-hoc test or multiple comparison procedures.
- TVarious post-hoc tests are available, all designed to control Type I errors. This ensures that there is close to a 95% chance of not falsely rejecting any true null hypothesis. Alternatively, there is only a 5% chance of erroneously rejecting a true null hypothesis.
- Tukey's Honestly Significant Difference (HSD) test is one such post-hoc test that controls Type I errors in a distinctive manner. It achieves this by focusing on the distribution of maximum and minimum averages.
- ![image](https://github.com/4nuG/Statistical-Analysis/blob/main/ANOVA/Screenshot%202024-02-01%20at%205.54.55%20PM.png)
- Comparing the p-values, we see that the mean MET in group B is significantly different and the differences in the mean MET in the other catagories are not significantly different. We conclude that the MET in the group B differs from the MET in the other groups.
  
## Conclusions
- The hypothesis test determined that the average physical activity level varies among the different levels of coffee consumption.
- Given the statistically significant differences in mean MET based on consumption levels, there is tentative evidence suggesting that the number of cups does affect MET per week. However, making definitive claims about which amount of coffee consumption yields the best MET is challenging due to issues with data quality. To draw such conclusions, more data with improved sampling would be necessary.
