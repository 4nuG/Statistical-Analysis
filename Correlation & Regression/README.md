# Table of Contents
- [Uses](#uses)
- [Objective 1](#objective-1)
- [Dataset 1](#dataset-1)
- [Analysis 1](#analysis-1)
  - [Multivariate analysis](#multivariate-analysis)
  - [Correlation Coefficient](#correlation-coefficient)
- [Conclusion 1](#conclusion-1)
- [Objective 2](#objective-2)
- [Dataset 2](#dataset-2)
- [Analysis 2](#analysis-2)
  - [Scatter plot](#scatter-plot)
  - [Multivariate](#multivariate)
  - [Least Squares Regression](#least-squares-regression)
  - [Diagnostic plots](#diagnostic-plots)
- [Conclusion 2](#conclusion-2)

# Uses
- Correlation
- Simple Linear Regression

# Objective 1 
- The objective of the analysis is to explore the relationship between lung cancer mortality (dependent variable) and smoking habits (independent variable) among men in 25 occupational groups in England.

# Dataset 1
- Correlation-1.xlsx
- From the Data and Story Library at Carnegie Melon University. The original source was: Occupational Mortality: The Registrar General's Decennial Supplement for England and Wales, 1970-1972, Her Majesty's Stationery Office, London, 1978.
- The data summarize a study of men in 25 occupational groups in England. Two indices are
presented for each occupational group.
  - The smoking index is the ratio of the average number of
cigarettes smoked per day by men in the particular occupational group divided by the average
number of cigarettes smoked per day by all men. (Values greater than 100 are above average.)
  - The mortality index is the ratio of the rate of deaths from lung cancer among men in the particular occupational group divided by the rate of deaths from lung cancer among all men.
- Variable Names:
  - 1.Occupational_Group: Occupational Group
  - 2.Mortality: Lung cancer mortality index (100 = average)
  - 3.Smoking: Smoking index (100 = average

# Analysis 1
## Multivariate analysis 
<img width="321" alt="image" src="https://github.com/4nuG/Statistical-Analysis/assets/81456513/48379542-af38-4b3a-a7d8-d72b3e2b5788">

<img width="528" alt="image" src="https://github.com/4nuG/Statistical-Analysis/assets/81456513/7b06f839-2c54-43b1-a514-226a146a4a6e">

- The scatterplot matrix shows an increasing positive moderate linear relationship, also indicated by the correlation coefficient of 0.7162. This suggests that as smoking increases, mortality also tends to increase. However, correlation does not imply causation (cannot definitively say that smoking causes mortality), but there is a noticeable relationship.
- In the scatterplot matrix, there is one outlier on the outskirts of the density ellipse. This outlier has a smoking rate of 116 and a mortality rate of 137, which is above the 100 average for both. This outlier suggests an unusual case where both smoking and mortality rates are higher than the norm.

## Correlation Coefficient
R = .7162

The correlation coefficient of 0.7162 signifies a positively increasing linear correlation with a moderate strength.

# Conclusion 1
The analysis reveals a noticeable positive correlation between smoking habits and lung cancer mortality among men in various occupational groups in England. However, caution must be exercised in attributing causation solely based on correlation. The identification of an outlier underscores the presence of unique cases that deviate significantly from the observed trend, warranting further investigation.

# Objective 2
- Determine whether a running puse is a good predictor of the maximum pulse a person can achieve.

# Dataset 2
- pulse.JMP
- Running pulse, RunPulse(X), and maximum pulse, MaxPulse(Y) of 31 subjects.

# Analysis 2
## Scatter plot
<img width="459" alt="image" src="https://github.com/4nuG/Statistical-Analysis/assets/81456513/f6fce076-bb7f-46d0-8b2f-bdab4acbbac0">

The scatter plot indicates an increasing positive moderate linear relationship between .RSquare is .86, which means there is a moderate, almost very strong linear relationship between RunPulse and MaxPulse. 86% of the variability in the response MaxPulse can be attributed to this linear regression with RunPulse. There is one outlier at 170 RunPulse and 186 MaxPulse which does not follow the linear pattern. 

## Multivariate
<img width="541" alt="image" src="https://github.com/4nuG/Statistical-Analysis/assets/81456513/b7b0d530-e79c-47b2-8978-f47f467bbb56">

Correlation coeficient = 0.9298
- The positive sign indicates that as RunPulse increases, MaxPulse also tends to increase.
- The value of 0.9298 indicates a very high degree of correlation, implying that changes in RunPulse are strongly associated with changes in MaxPulse.

## Least Squares Regression
<img width="413" alt="image" src="https://github.com/4nuG/Statistical-Analysis/assets/81456513/2b431594-cfce-4564-8051-031c7a88335f">

Estimated Regression Line:

MaxPulse(Y)=32.783316+0.8310928×RunPulse(X)

- Intercept is 32.783316 but this value doesn’t make any sense as a run pulse of 0 is
impossible and you won’t be able to get a max pulse of 32.8 from it.
- The slope of the line is 0.8310928 meaning that for each increase in run pulse, the max
pulse increases by about 0.83.

- R2 (RSquare): 0.864442; This represents the proportion of the variance in the dependent variable (MaxPulse) that is predictable from the independent variable (RunPulse). In this case, approximately 86.44% of the variance in MaxPulse can be explained by the linear regression model.

## Diagnostic plots
Diagnostic plots used to assess the assumptions of the linear regression model:

<img width="492" alt="image" src="https://github.com/4nuG/Statistical-Analysis/assets/81456513/5eb0c71e-e5db-4a8a-a07e-b8af2cfe2931">

Residuals by Predicted Plot:
- Points are random near zero with no pattern.
- Indicates that errors are uncorrelated random variables with a mean of zero.

Residuals by X Plot:
- Points are random near zero with no pattern.
- Confirms that the variance is constant and independent.

Residuals by Row Plot:
- No pattern and randomness are observed.
- Demonstrates independence of errors.

Actual by Predicted Plot:
- Points fall on a line with one outlier.
- The presence of an outlier may need further investigation but overall suggests that the model is adequate.

Residual Normal Quantile Plot:
- Points mostly fall on the line of best fit with little skew.
- Indicates normalcy of residuals.
  
# Conclusion 2
Based on the analysis, there is compelling evidence for the predictive power of running pulse in estimating maximum pulse, supported by a well-fitted regression model and diagnostic plots that validate the assumptions of linear regression.
