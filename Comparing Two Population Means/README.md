# Objective
- Determine, at a 5% significance level, whether there is a significant difference in the deflection temperature under load between two types of plastic pipes (type 1 and type 2).

# Datset
Two random samples of 15 pipe specimens were tested, and the deflection
temperatures observed are reported here (in ºF).

| Type 1 | Type 2 |
|--------|--------|
| 206    | 177    |
| 188    | 197    |
| 205    | 206    |
| 187    | 201    |
| 194    | 180    |
| 193    | 176    |
| 207    | 185    |
| 185    | 200    |
| 189    | 197    |
| 213    | 192    |
| 192    | 198    |
| 210    | 188    |
| 194    | 189    |
| 178    | 203    |
| 205    | 192    |

# Parameter of interest
- mu1 = avg deflation temp observed of type 1
- mu2 = avg deflation temp observed of type 2
- mu1-mu2, the difference between the temperature means of two types populations.
  
# Point estimate for the parameter of interest
- sample mean 1 = avg sample deflation temp observed of type 1 = 196.4
- sample mean 2 = avg sample deflation temp observed of type 2 = 192.06666666667
- (sample mean 1) – (sample mean 2), the difference between the temperature means of two types
samples = 4.33334

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%202.44.35%20PM.png)

# Asumptions/Requirements
- We don’t know population std1 and population std2, so we will find simple std1 and simple
std2.

| Type   | std                  |
|--------|----------------------|
| Type1  | 10.479912758634      |
| Type2  | 9.4375137968994      |

- The sample mean and std for Type1 is higher suggesting that values are larger and more spread out from the mean. 
- Because the observation from one sample does not influence the observations in another sample, the samples are independent.
- Samples are random.

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%202.57.40%20PM.png)
- From the quantile plots I can see both distributions are normal as there is a good fit to a straight
line for both. Hence  both the distribution of temperatures is close to normal.

# Hypothesis
- H0: mu1-mu2 = 0 or mu1 = mu2
- h1: mu1-mu2 != 0 or mu1 != m2
  
# Test Statistic 
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%203.07.58%20PM.png)

- The data are independent, and the population variances are not known but equal (the normal
quantile plot are parallel and normal) so we are doing a pooled t-test.
- When std is unknown, we approximate using sample std from each sample. Sample std 1 =
10.480 degrees and sample std 2 = 9.438 degrees.
- We also need to assume that the std of each population is approximately the same (std1 = std2).
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%203.22.50%20PM.png)

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%203.23.06%20PM.png)

- JMP shows: t = -1.190
- The test statistic follows a t distribution with 28 degrees of freedom
- The negative sign of the t-value suggests that the mean of the first sample is lower than the mean of the second sample.
  
# P-value
- If the p-value is less than the significance level (commonly 0.05), reject the null hypothesis that the population means are equal.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%203.38.40%20PM.png)

- JMP shows the p value is .2440. The result is not significant at p <.05

# Conclusion
- Fail to reject the null hypothesis because the p-value is greater than the significance level.
- There is not enough evidence at a 5% significance level to warrant rejecting the claim that they
both have the same temperature.

# 5% confidence interval for the mean difference (does is agree with the hypothesis test?) 
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Comparing%20Two%20Population%20Means/Screenshot%202024-01-31%20at%203.43.04%20PM.png
)
- JMP indicates a 95% confidence interval for the difference in true mean temperatures, ranging from -11.792 to 3.641 degrees.
- This implies that we are 95% confident that the actual difference in mean temperatures falls within this interval. Moreover, we can state with 95% confidence that the difference in true mean temperatures is between -11.792 and 3.641 degrees, and this interval includes 0 degrees. This aligns with the conclusion from the hypothesis test, indicating insufficient evidence at a 5% significance level to reject the claim that both temperatures are the same (i.e., we cannot reject μ1 = μ 2​ or μ 1 − μ 2 = 0).
