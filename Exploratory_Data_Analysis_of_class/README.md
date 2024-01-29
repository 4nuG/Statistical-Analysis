Dataset is 'Class.jmp' and can be viewed using JMP.
# Objective
- Determine 'Does there exist a relationship between “Height” and “Mother’s Height”?
- Determine 'Does major appear to be independent of gender?'
- Determine 'Do students spend more hours per week on social media or studying.'
- Determine 'Does gender affect the amount of time spent on social media.'
- Conduct Exploratory Data Analysis (EDA) on student survey data and visualize both quantitative and categorical data using JMP software. 

# Exploratory Data Analysis
## Student data set 
The student dataset contains hours spent studying and other attributes of 68 statistics students. The raw data has 16 features - 2 ordinal (statistics, and college year), 5 Nominal (Timestamp, Gender, job during academic year?, Major, and lab section) and 9 numerical (Travel in the US, Travel Abroad, Height, Mother's Height, Father's Height, Social media, hours studying, Weight, and BMI).

The features are described as follows:
### Ordinal: 
- Statistics: how important they think statistics is from 0 - 10 with 10 being the most important.
- College Year: credit posiiton from Freshman to Seinor.

### Nominal:
- Timestamp: YYYY/MM/DD HH:MM:SS AM/PM EST
- Gender: Male or Female
- job during academic year?: yes or no
- Major: degree
- Lab Section: lab section number

### Numeric: 
- Travel in the US: Number of states visited
- Travel Abroad: Number of countries visited
- Height: in inches
- Mother's Height: in inches
- Father's Height: in inches
- Social media: Minutes spent on social media in a week
- hours studying?: hours spent studying in a week
- Weight: weight in lbs
- BMI: bmi

#### Table 1: Initial student dataset
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-28%20at%2012.51.24%20PM.png)

## Data Cleaning
### Histogram, outlier box plot and numeric summaries of the quantative data

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-28%20at%2011.23.48%20AM.png)
The points were considered outliers if they were located outside the whisker and more than 1.5 times the Interquartile Range (IQR) away from the box. 'Social Media', and 'How many hours do you spend studying' both have 1 outlier. The distribution for height is symmetric, while the distributions for social media and the number of hours spent studying per week are both right-skewed. Symmetry is visually evident in the height distribution, and the box-and-whisker plot confirms its symmetry. For social media and hours spent studying, their graphs show right-skewed distributions, with longer right whiskers in the box plot.

### Bar chart and frequency table of the catagorical data

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-28%20at%209.24.39%20PM.png)
- The gender bar chart indicates that there are more males than females taking this class with this teacher at this designated time.
- The Major bar chart reveals that Engineering is the most popular Major.
- The statistics bar chart shows that most people consider statistics to be important, rating it above 5 on a scale from 0 to 10.

### Scatter plot of the bivariate data

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-28%20at%209.37.16%20PM.png)
- The scatterplot suggests that there is no general correlation between mother’s height and height.
- This data cannot be employed to establish a causal relationship between "Height" and "Mother’s Height" becuase this is an observational study, and drawing causal conclusions from such studies is not feasible.

### Mosaic of Gender and Major

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-28%20at%209.42.09%20PM.png)
Major does not appear to be independent of gender. When variables are independent, all proportions are the same. However, in this case, the proportions of males and females in different Major are not the same. The difference in proportions suggests a dependence between gender and Major. Therefore, gender does influence the choice of Major.

Created a new variable “Social Media Hrs per Wk” because "Social Media” and “Studying Hrs per Wk” are in different units.

### Histogram, outlier box plot and numeric summaries of the numeric data

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-29%20at%201.49.52%20PM.png)
Uniform Scalling is applied to both "Social Media Hrs per Wk” and "Studying Hrs per Wk” to compare the variables using the same scale. 
- Based on the histograms and box plots, a brief comparison of the distributions of "Social Media Hrs per Wk" and "Studying Hrs per Wk" reveals that both variables exhibit right-skewed distributions with one outlier each. The mean for both variables falls between the 2nd (median) and 3rd quartile. "Studying Hrs per Wk" has a higher mean than "Social Media Hrs per Wk," and it also displays a higher standard deviation, indicating greater variability.
- "Social Media Hrs per Wk" has one more experimental unit than "Studying Hrs per Wk," potentially impacting its mean and median.

|                       | Social Media Hrs per Wk | Studying Hrs per Wk |
|-----------------------|-------------------------|---------------------|
| Mean (X̄)              | 13.108 hrs              | 15.075 hrs          |
| Standard Deviation (s)| 9.549 hrs               | 15.695 hrs          |
| Minimum               | 0 hrs                   | 1 hrs               |
| Q1 (First Quartile)   | 7 hrs                   | 6 hrs               |
| Q2 (Second Quartile)  | 10.5 hrs                | 12 hrs              |
| Q3 (Third Quartile)   | 18.375 hrs              | 20 hrs              |
| Maximum               | 42 hrs                  | 120 hrs             |
| IQR (Interquartile Range)| 11.375 hrs           | 14 hrs              |

Social Media Hrs per Wk:
- Min Usual Value =  13.108 − 2 ( 9.549 ) = − 5.99 
- Max Usual Value =  13.108 + 2 ( 9.549 ) = 32.206 
- The average time spent on social media per week is 13.108 hrs, and so it is not unusual to observe times between 0-32.206 hrs.

Studying Hrs per Wk:
- Min Usual Value = 15.075 − 2 ( 15.695 ) = − 16.315
- Max Usual Value = 15.075 + 2 ( 15.695 ) = 46.465
- The average time spent studying per week is 15.075 hrs, and so it is not unusual to see times between 0-46.465 hrs.

From the analysis, it's evident that the mean and median times spent studying surpass those for social media. This suggests a general trend of dedicating more time to studying than engaging with social media. However, it's important to note that the higher standard deviation in studying hours indicates increased variability and less stability compared to the more consistent hours spent on social media.

### Exploring Bivariate Data – Comparative Boxplots
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/Exploratory_Data_Analysis_of_class/Screenshot%202024-01-29%20at%203.55.46%20PM.png)

- The graphs for 'Social Media Hrs per Wk' for both genders are skewed right, as evidenced by the longer right whiskers in the box plots.
- The female distribution has no outliers. The lower outlier for females is calculated as 9.625 − ( 1.5 × ( 28 − 9.625 ) ) = − 17.938, and the upper outlier is 28 + ( 1.5 × ( 28 − 9.625 ) ) = 55.5625.
- The male distribution has 2 outliers. The lower outlier for males is 5.688 − ( 1.5 × ( 15.75 − 5.688 ) ) = − 9.405, and the upper outlier is 15.75 + ( 1.5 × ( 15.75 − 5.688 ) ) = 30.843.
- Their mean is between the 2nd (median) and 3rd quartiles.
  
- Females have a higher mean than males and also a higher standard deviation, indicating that their variability is less stable than that of males.
- Males have more experimental units than females, which could significantly impact the mean and median, potentially making them more accurate and explaining the smaller standard deviation.

Conclusion: Since this is an observational study, cause and effect cannot be derived. Therefore, we cannot logically imply that gender influences the time spent studying. Also, since there are fewer male students, I do not believe this study can generalize gender’s effect on time spent studying.
