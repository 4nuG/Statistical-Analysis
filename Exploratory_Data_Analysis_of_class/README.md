# Objective
- Conduct Exploratory Data Analysis (EDA) on student survey data and visualize both quantitative and categorical data using JMP software. 

# Exploratory Data Analysis
## Student data set 
The student dataset contains hours spent studying and other attributes of 68 statistics students. The raw data has 16 features - 2 ordinal (statistics, and college year), 5 Nominal (Timestamp, Gender, job during academic year?, Major, and lab section) and 9 numerical (Travel in the US, Travel Abroad, Height, Mother's Height, Father's Height, Social media, hours studying, Weight, and BMI).

The features are described as follows:
### Ordinal: 
Statistics: how important they think statistics is from 0 - 10 with 10 being the most important. 
College Year: credit posiiton from Freshman to Seinor.

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
