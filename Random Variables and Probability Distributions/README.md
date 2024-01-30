## Uses
- Detecting Systematic Biases or Irregularities
- Assessing Data Reliability and Accuracy
- Quality Control in Data Collection

## Objective
Determine if a discrete data set exhibits a non-random distribution in the last digits, as this could suggest a potential pattern or bias in the way the data was collected. The analysis of the last digits may provide insights into whether the data has been systematically rounded, reported, or manipulated by subjects, thereby influencing the reliability and accuracy of the dataset.

## Method 
Use probability distributions to determine whether results can be reasonably explained by chance or whether chance alone does not appear to be feasible, so other factors are influencing results.

## Random Variable
A random variable is a variable whose value is a numerical outcome of the random phenomenon. The random variable here is the last digit in the given heights of each building and the value for these random variables are 0-9.

## Probabaility Distribution
The probability distribution is 0.1 for the random variable.

|       | Ending Value | Theoretical Probability Distribution  |
|-------|--------------|---------------------------------------|
|       | 0            | 0.1                                   |
|       | 1            | 0.1                                   |
|       | 2            | 0.1                                   |
|       | 3            | 0.1                                   |
|       | 4            | 0.1                                   |
|       | 5            | 0.1                                   |
|       | 6            | 0.1                                   |
|       | 7            | 0.1                                   |
|       | 8            | 0.1                                   |
|       | 9            | 0.1                                   |
|Total: |              | 1                                     |


## Expected Value and the Standard Deviation
Expected Value = (0+1+2+3+4+5+6+7+8+9)/10 = 4.5

Standard Deviation = 

$`\sqrt{0.1(0-4.5)^2 + 0.1(1-4.5)^2 + 0.1(2-4.5)^2 + 0.1(3-4.5)^2 + 0.1(4-4.5)^2 + 0.1(5-4.5)^2 + 0.1(6-4.5)^2 + 0.1(7-4.5)^2 + 0.1(8-4.5)^2 + 0.1(9-4.5)^2}`$ = 2.87

## Distribution of the Last Digit of the Measurements

| Number of Times  | Ending Number | Percentage |
|------------------|---------------|------------|
| 2                | 0             | 6.6%       |
| 3                | 1             | 10.0%      |
| 2                | 2             | 6.6%       |
| 5                | 3             | 16.6%      |
| 2                | 4             | 6.6%       |
| 1                | 5             | 3.3%       |
| 4                | 6             | 13.3%      |
| 4                | 7             | 13.3%      |
| 1                | 8             | 3.3%       |
| 6                | 9             | 20.0%      |


## Mean and the Standard Deviation of the Frequency Distribution 
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Random%20Variables%20and%20Probability%20Distributions/Screenshot%202024-01-30%20at%201.35.27%20PM.png)
The Mean is 4.967 and the Standard deviation is 2.906

## Conclusion 
Comparing the theoretical distribution mean (4.5) with the frequency distribution mean (4.967), it appears that the values were obtained from actual measurements. The similarity between these mean values suggests an even spread of ending digits. However, the observed distribution is not perfectly even, possibly due to the small sample size (only 30 data points). With a larger sample size, the theoretical standard deviation would likely align more closely with the frequency standard deviation, as more data would contribute to making the variance from the mean more similar to the theoretical standard deviation.

