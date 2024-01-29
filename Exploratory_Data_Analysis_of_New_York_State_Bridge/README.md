Data is in 'Bridge data.jmp' and can be opened using JMP.

## Introduction
- In 2007, the I-35 Bridge in Minneapolis, Minnesota collapsed during rush hour traffic.
- In response, the governor of New York established a task force to assess the safety of similar structured bridges in the state.

## Dataset
- NYSDOT AVG Condition Rating - condition rating scale ranges from 1 to 7, with 7 being in new condition and a rating of 5 or greater considered as good condition.
- Flagging Status - safety flag.

Task Force Mandate
- The task force's primary objectives were to investigate the safety of bridges in New York.
- The focus was on bridges with designs similar to the I-35 Bridge, evaluating inspection standards and procedures.

Reports Presentation
- The task force presented two key reports:
a) Initial Report (August 31, 2007)
b) Final Report (November 30, 2007)

Data Set in the Initial Report
- The August report includes data on inspections of 49 deck truss highway bridges in New York.
- These bridges share a design akin to the I-35W Bridge in Minnesota.

Sample or Population?
- The data set in the August report represents a sample.
- Explanation: The 49 deck truss highway bridges served as a sample to draw conclusions about the broader population of bridges in New York with a similar design and type as the I-35W bridge.
- Note: 24 private bridges were not included, reinforcing the characterization of the data set as a sample.

The task force's findings in the August report play a crucial role in determining the safety of bridges in New York with designs resembling the I-35W Bridge. The reliance on a sample reinforces the importance of robust inspections and standards for ensuring the safety of the broader bridge population.

## Exploratory data analysis of the NYSDOT Average Condition Rating

### Histogram and Boxplot
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_New_York_State_Bridge/Screenshot%202024-01-29%20at%204.56.02%20PM.png)
- Upon examination of the NYSDOT boxplot, a notable observation is the symmetry in the distribution.
- The closeness of the mean and median, along with a small standard deviation of 0.73, further supports the symmetric nature of the data.
- The boxplot reveals an outlier as evidenced by a point outside the right whisker.
  
Lower Outlier = 3.9575 – 1.5(5.0025-3.9575) = 2.39 avg rating

Upper outlier = 5.0025 + 1.5(5.0025-3.9575) = 6.57 avg rating

- Calculation of outliers using Tukey's method indicates a lower outlier threshold of 2.39 average rating and an upper outlier threshold of 6.57 average rating.
- Since the lowest value recorded is 2.92, and the highest is 6.61, there is one outlier in the histogram. The histogram is right-skewed, as the mean is larger than the median value.
