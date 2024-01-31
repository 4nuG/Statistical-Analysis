## Uses
- Quality Assurance in Data Analysis
- Risk Management

## Objective
- Determine if the process that produces 0.5 mm lead refills for mechanical pencils is still on target. To assess this, a sample of 20 of these leads is randomly selected. For these refills to fit the pencils properly, they need to have an average diameter of 0.5 mm.

## Data Set
- Lead_Diameters.jmp
  
### Numberic Feature 
- Lead Diam: lead diameter in mm
  
## Method
- one-sample hypothesis testing
- confidence interval construction

## Parameter of Interest
- The parameter of interest is the mean/average diameter of leads.

## Point Estimate for the Parameter of Interest
- The point interest estimates the population parameter.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.33.02%20PM.png)

##  Assumptions for a Confidence Interval 
- x₁, x₂, ..., xₙ is a random sample of size n from a population, which is true becuse we have a random sample size of 20 pieces of lead.
- The population is normally distributed or if not, the conditions of the central limit theory apply
(n>=30). The conditions of the central limit theory do not apply since n = 20. However, the graph is
normally distributed as there is a good fit to a straight line: The distribution of diameters values
is close to Normal.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.42.24%20PM.png)

##  Hypothesis Test with Known Standard Deviation
- Hypothesis test to determine if the process appears to still be on target (0.05 significance level).
- Let’s assume that it is known that the standard deviation of the diameters is 0.02 mm.
- In JMP, since we know the standard deviation, we can enter that value as the True Standard Deviation so that the z-test is performed.

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.50.41%20PM.png)

H₀: μ = 0.5
H₁: μ ≠ 0.5

Test statistic = -1.4974
P-value: prob > |z| = 0.1343

- Fail to reject the null hypothesis because the p-value (.1343) is greater than the significance level (.05).


- Calculated test statistic:
- Calculatedp-value for the t:

## Conclusion of Hypothesis Test with Known Standard Deviation 
There is not sufficient evidence at a 5% significance level to support the claim that the avg lead
diameter is .5 mm.

##  95% confidence interval with Standard Deviation
- Using 0.95 for the confidence level and 0.02 for the population standard deviation.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.58.59%20PM.png)
- The lower mean confidence interval is .484538 and the upper is .502069. Since the null hypothesis value (.5)
falls in the interval, we do not reject. This is similar to number the hypothesis test.

Assuming population standard deviation is unknown:

## Point Estimate of the standard deviation
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%204.05.18%20PM.png)
.01496

##  Hypothesis Test without known standard deviation
- Hypothesis test to determine if the process appears to still be on target (0.05 significance level).
- In JMP, since we do not know the standard deviation, do not enter a standard deviation so that a t-test is
performed.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%204.10.01%20PM.png)

H₀: μ = 0.5
H₁: μ ≠ 0.5

Test statistic = -2.0019
P-value: Prob > |t| = 0.0598

- Fail to reject the null hypothesis because the p-value (0.0598) is greater than the significance level
(.05).

## Conclusion of 95% confidence interval with Standard Deviation
There is not sufficient evidence at a 5% significance level to support the claim that the mean
diameter of the led is .5mm

##  95% confidence interval without Standard Deviation 

8. 2 / 3 pts Explain why they are different. 

Part 3. 3 / 5 pts Their distributions and p-value are also different. This is due to estimating the population standard deviation resulting in different distribution for test statistic.

