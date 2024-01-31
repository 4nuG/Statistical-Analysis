# Table of Contents

- [Uses](#uses)
- [Objective](#objective)
- [Data Set](#data-set)
- [Numeric Feature](#numeric-feature)
- [Method](#method)
- [Parameter of Interest](#parameter-of-interest)
- [Point Estimate for the Parameter of Interest](#point-estimate-for-the-parameter-of-interest)
- [Assumptions for a Confidence Interval](#assumptions-for-a-confidence-interval)
- [With Known Standard Deviation](#with-known-standard-deviation)
  - [Hypothesis Test with Known Standard Deviation](#hypothesis-test-with-known-standard-deviation)
  - [95% Confidence Interval with Known Standard Deviation](#95-confidence-interval-with-known-standard-deviation)
- [Without Known Standard Deviation](#without-known-standard-deviation)
  - [Point Estimate of the Standard Deviation](#point-estimate-of-the-standard-deviation)
  - [Hypothesis Test without Known Standard Deviation](#hypothesis-test-without-known-standard-deviation)
  - [95% Confidence Interval without Known Standard Deviation](#95-confidence-interval-without-known-standard-deviation)
- [Conclusion](#conclusion)

## Uses
- Quality Assurance in Data Analysis
- Risk Management

# Objective
- Determine if the process that produces 0.5 mm lead refills for mechanical pencils is still on target. To assess this, a sample of 20 of these leads is randomly selected. For these refills to fit the pencils properly, they need to have an average diameter of 0.5 mm.

# Data Set
- Lead_Diameters.jmp
  
## Numeric Feature 
- Lead Diam: lead diameter in mm
  
# Method
- one-sample hypothesis testing
- confidence interval 

# Parameter of Interest
- The parameter of interest is the mean/average diameter of leads.

## Point Estimate for the Parameter of Interest
- The point interest estimates the population parameter.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.33.02%20PM.png)

##  Assumptions for a Confidence Interval 
- x₁, x₂, ..., xₙ is a random sample of size n from a population. This is true becuse we have a random sample size of 20 pieces of lead.
- The population is normally distributed or if not, the conditions of the central limit theory apply
(n>=30). The conditions of the central limit theory do not apply since n = 20. However, the graph is
normally distributed as there is a good fit to a straight line: The distribution of diameters values
is close to Normal.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.42.24%20PM.png)

# With Known Standard Deviation
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
- There is not sufficient evidence at a 5% significance level to support the claim that the avg lead
diameter is .5 mm.

##  95% confidence interval with Known Standard Deviation
- Using 0.95 for the confidence level and 0.02 for the population standard deviation.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%203.58.59%20PM.png)
- The lower mean confidence interval is .484538 and the upper is .502069. Since the null hypothesis value (.5)
falls in the interval, we do not reject. This is similar to number the hypothesis test.

# Without Known Standard Deviation
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
- There is not sufficient evidence at a 5% significance level to support the claim that the mean
diameter of the led is .5mm

##  95% confidence interval without known Standard Deviation 
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Hypothesis%20Testing/Screenshot%202024-01-30%20at%204.16.58%20PM.png)

- The lower mean confidence interval is .486302, and the upper is .500305. Comparing this interval to the one previously obtained (known standard deviation), the interval here is slightly wider. This widening is due to the uncertainty introduced by estimating the standard deviation from the sample, as opposed to having a known population standard deviation.

- Since the null hypothesis value (.5) falls within the interval, we do not reject it.

# Conclusion
- The analysis suggests that the process producing the 0.5 mm lead refills for mechanical pencils appears to be on target based on the given sample data.

  
- The difference in interval width between known and unknown standard deviation reflects the impact of estimating the standard deviation from the sample, highlighting the inherent variability introduced by this estimation process.
- Part one had a known standard deviation, part two had an unknown standard deviation.
- The decisions and conclusions did not change between parts 1 and 2.
- In part 1, a two-tailed z test was employed, yielding a z test statistic of -1.4974. In contrast, part 2 utilized a two-tailed t test, producing a t test statistic of -2.0019. One notable difference arises from the estimation of the population standard deviation in part 2, leading to a different distribution for the test statistic. This divergence in distributions contributes to variations in p-values.
- Furthermore, the distributions and p-values are dissimilar between the two parts due to the inherent variability introduced by estimating the population standard deviation in part 2. The t test statistic in part 2, being on the edge of rejection, suggests a closer proximity to the 0.05 significance level, emphasizing the impact of the estimation process on the outcome. Despite these differences, the decisions and conclusions remained consistent in both parts. 
