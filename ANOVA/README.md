# Exploring the Relationship between Coffee Consumption and Physical Activity
## Introduction
Caffeine is the world’s most widely used stimulant, with approximately 80% consumed in the form of coffee. 
I want to determine if there exists a relationship between coffee consumption and exercise. 

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

## Data Visualization
### Association Plot Analysis of MET score and coffee consumption
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Hypothesis%20Testing%20-%20Proportions/Screenshot%202024-02-01%20at%203.13.01%20PM.png)

The box plots for variables A-E are right skewed shown by the long right tails, so most types of consumption have a low metabolic equivalent tasks per week score and only some have a higher score. All categories have outliers on the right tail raising the MET per week mean which is 26.67684. The mean MET per week does not fall in the 95% confidence interval of A and B where A is below and B is above. This is an unbalanced design because the sample size in each group is not equal.

## Analysis of Variance (ANOVA)
Even with the unbalanced design, we can conduct an analysis to determine whether the average physical activity level varies among the different levels of coffee consumption.
- Parameter of interest: Mean MET per week for different levels of coffee consumption
- Assumptions
  - The samples are independent and there is no pairing or underlying structure.
  - 

## Assessment of Assumptions

## Conclusions

