Data is in 'Bridge data.jmp' and can be opened using JMP.
# objective
- Determine if the protocol used in final task force report dated November 30, 2007 is effective and correct.
   
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

### Numeric summaries of the NYSDOT Average Condition

| NYSDOT Average Condition Rating  |                         |
|----------------------------------|-------------------------|
| X (Mean)                         | 4.489 avg rating        |
| s (Standard Deviation)           | 0.734 avg rating        |
| Min                              | 2.92 avg rating         |
| Q1 (First Quartile)              | 3.958 avg rating        |
| Q2 (Second Quartile/Median)      | 4.415 avg rating        |
| Q3 (Third Quartile)              | 5.0025 avg rating       |
| Max                              | 6.61 avg rating         |
| IQR (Interquartile Range)        | 1.045 avg rating        |

- The mean indicates that, on average, the bridges are receiving a rating of 4.49. This is concerning because a bridge typically needs a rating of at least 5 to be considered in "good condition." Consequently, with a mean below 5, it suggests that, theoretically, approximately half of the bridges fall into the category of "bad condition."
- The small standard deviation of only 0.73 further emphasizes that the ratings are closely clustered around the mean. This supports the assumption that about half of the bridges may indeed be below "good condition," as the ratings exhibit limited variation from the average.

Minimum usual value: 4.489 − 2 × 0.734 = 3.021 avg rating 

Maximum usual value: 4.489 + 2 × 0.734 = 5.957 avg rating 

- While the average of the ratings is 4.489, it is not uncommon to observe ratings between 3.021 and 5.957. This range explains why the maximum rating of 6.61 is considered an outlier.

### Exploratory data analysis of Flagging Status
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_New_York_State_Bridge/Screenshot%202024-01-29%20at%205.12.40%20PM.png)

- The bar chart indicates that the majority of the bridges did not receive any flags. Specifically, 60% of the inspected bridges did not receive any type of flag, while the remaining 40% received some form of flag. Notably, only one out of the 50 inspected bridges received a red flag.
- Upon closer examination of the bar chart, it becomes apparent that more than one-third of the bridges exhibit some condition other than having no flags.

### Conclusion
The November 30, 2007, report asserts that "the deck truss bridges in New York State are safe for public travel, and the bridge inspection protocols used in New York are effective." However, I dispute the claim that the bridges are safe for travel and question the effectiveness of the protocols.

According to the report, 14% of the bridges exhibit conditions that pose safety hazards to the public (e.g., cracked sidewalks) or to traffic (e.g., bridge rail requiring repair). Although the report does not explicitly specify why a bridge is flagged yellow, I argue that both conditions are potentially dangerous for anyone using the bridge, especially damaged bridge rails, which are accidents waiting to happen.

Furthermore, 10% of the bridges are in conditions that, if left unattended until the next scheduled inspection, would likely progress to a more critically deficient state. If these issues are not addressed promptly, they will necessitate an annual inspection. It seems there is an option to either correct the condition promptly or wait and opt for a yearly inspection. Regardless, these bridges have the potential to become hazardous if not addressed promptly. Another 14% of bridges face both of the aforementioned conditions. Consequently, just a little above 50% of the bridges can be considered free from danger. The November report should have stated that "a majority of the deck truss bridges in New York State are safe for public travel."

There are also discrepancies that cause me to not trust the reports. Both reports state that the "Newburgh-Beacon twin-span bridge is considered a single bridge out of the total of 49 deck truss highway bridges." However, if it is considered a single bridge, it should be one of the 49 bridges. Yet, the total number of bridges in the study is listed as 50. Further inspection reveals that this specific bridge is listed twice. Although these bridges have no flags, one of them is rated as "good," while the other is close to "good." This implies that these bridges raised the mean and the count of "none" flags.

The August report claimed that the protocol is aimed at "identifying and correcting problems early before they become serious and compromise a bridge’s ability to remain in service." However, both reports also note that "approximately 5% of all bridge inspections result in a flagged condition being discovered." This could mean that 5% of the bridges have flagged conditions, or it could imply that inspections have a 5% chance of discovering conditions. Given that 40% of the bridges have flags, I suspect the latter, indicating that 5% of the inspections conducted reveal conditions. If there is such a low chance of discovering conditions, there is a likelihood that more conditions are being overlooked.

While numerous other points could be argued, the analysis conducted reveals a right-skewed histogram, an unstable standard deviation (far from 0), a mean below "good," only 25% of the bridges above "good," and 40% of the bridges flagged. Consequently, I do not believe the bridges are safe, and the protocols are not efficient.
