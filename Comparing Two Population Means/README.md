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

| Type   | Variance             |
|--------|----------------------|
| Type1  | 109.82857142857      |
| Type2  | 89.066666666667      |

- The sample mean and variance for Type1 is higher suggesting that values are larger and more spread out from the mean. 
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
We also need to assume that the std of each population is approximately the same (std1= std2).


# P-value
# Conclusion
# 5% confidence interval for the mean difference (does is agree with the hypothesis test?) 


# Points
5. 4 / 4 pts 6. 2 / 2 pts 7. 1 / 1 pt 8. 1 / 1 pt 9. 1 / 1 pt 10. 2 / 2 pts
