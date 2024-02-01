# Table of Contents

- [Uses](#uses)
- [Introduction](#introduction)
  - [Objective](#objective)
  - [Dataset](#dataset)
  - [Parameter of Interest](#parameter-of-interest)
- [Methodology](#methodology)
  - [Frequency Table and Bar Chart](#frequency-table-and-bar-chart)
- [Analysis](#analysis)
  - [Estimated Percent of People Who Have Tried Their Lasagna](#estimated-percent-of-people-who-have-tried-their-lasagna)
  - [Sample Size](#sample-size)
- [Hypothesis Testing](#hypothesis-testing)
  - [Formulation of Hypotheses](#formulation-of-hypotheses)
  - [Formula for the Test Statistic](#formula-for-the-test-statistic)
- [Statistical Testing](#statistical-testing)
  - [Assumptions](#assumptions)
    - [Assessment of Normal Distribution Assumption](#assessment-of-normal-distribution-assumption)
  - [Test Statistic](#test-statistic)
  - [P-value](#p-value)
- [Results and Interpretation](#results-and-interpretation)
  - [Significance Level](#significance-level)
  - [Decision](#decision)
- [Conclusion](#conclusion)


# Uses
- Marketing - determining brand awareness
  
# Introduction
## Objective 
The makers of Momma Mia Lasagna want to know if more than half the population has tried their lasagna. 

## Dataset
The data collected from a survey study are in the file Momma Mia Lasagna.jmp.

## Parameter of Interest
p: proportion of people who have tried Momma Mia Lasagna.

# Methodology
## Frequency Table and Bar Chart

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Hypothesis%20Testing%20-%20Proportions/Screenshot%202024-02-01%20at%202.13.07%20PM.png))

# Analysis
## Estimated Percent of People Who Have Tried Their Lasagna
It is estimated 58.52% of people have tried their lasagna.

## sample size
Sample size is 1162 people.

# Hypothesis Testing
## Formulation of Hypotheses
- **Null Hypothesis (𝐻₀):** 𝑝 = 0.5
- **Alternative Hypothesis (𝐻ₐ):** 𝑝 > 0.5

## Formula for the Test Statistic
- **Formula for the Test Statistic:**
  ![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Hypothesis%20Testing%20-%20Proportions/Screenshot%202024-02-01%20at%202.17.24%20PM.png)

# Statistical Testing
## Assumptions
- **Assessment of Normal Distribution Assumption:**
  
  a. 𝑛𝑝₀ = (1162)(.5) = 581 > 10
  
  b. 𝑛(1 ― 𝑝₀) = 1162(1 ― .5) = 581 > 10
  
  **Conclusion:** We can assume the test statistic has a standard normal distribution.

## Test statistic
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Hypothesis%20Testing%20-%20Proportions/Screenshot%202024-02-01%20at%202.34.25%20PM.png)

## P-value
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Hypothesis%20Testing%20-%20Proportions/Screenshot%202024-02-01%20at%202.36.48%20PM.png)

Using the formula, I got the exact value as shown in column 2 and with JMP, we can see that p-value is <.0001.

# Results and Interpretation
## Significance Level
Assume: α = 0.05

## Decision?
Since p <.0001< α = 0.05, p-value is less than significance level so we reject the null hypothesis.

# Conclusion
There is sufficient evidence at a 5% significance level to support the claim that more than half the
population has tried Momma Mia’s lasagna


