# Objective 
Estimate the mean house price of houses in New York, NY. 
- State clearly how you are defining the type of house: single family or condominiums.
- Go to a real estate website such as Realtor.com or Zillow.com.
- Obtain at least 20 data values.
- If you search results in a large number of houses, take a random sample.

# Dataset
- On 04/05/2021 at 10:39 am there were 3,795 Agent listed “for sale” single-family houses on Zillow at New York, NY (by the end of the day there were 5 more!).
- I used the free trial version of WebHarvy to extract the data from Zillow.
- The free trial version was only able to extract the first 40 listings under “homes for you”, which would make this an inadequate selection of data and counterproductive. I then created a JMP file with 3,795 rows that contained values 1- 3,795 and randomly chose 20 rows. I selected rows>row selection>select randomly and choose a value of 20 to get my 20 random data values. Below is an example of one of the randomly selected points.
  
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.29.28%20PM.png)

With 40 listings per page, I was able to find which page all the listings were in and was about to create another JMP file with only the selected houses. Unfortunately, Zillow only listed 20 pages of information which is 800 houses (40 houses/page). Since my data consisted of 800+ houses I had to reselect my data samples to be 20 of the 800 listed. Again I did the rows>row selection>select randomly and choose a value of 20 to get my 20 random data values from the 800. Below are the randomly selected houses with the column “house” associated to the position in the list of 800 houses and “price” referring to the price of the selected house:

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.31.26%20PM.png)

# Mean House Price
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.34.07%20PM.png)

The estimated average price for a house in New York, NY is $828,539. If we were to conduct a 95% confidence interval we would use the following formula:
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.35.57%20PM.png)

Here x̅ is the sample mean and s is the sample standard deviation. Our significance level α is .05 and our n is 20. The t ratio can be derived from the t values chart or JMP. We can use this formula to find the interval because all the assumptions are met. As previously stated all the samples were collected randomly by the JMP software ensuring a random sample of size 20.
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.38.16%20PM.png)

From the normal quantile plot above it is evident that the data is normally distributed. There is a good fit to a straight line and the distributions of the house prices are close to normal. In addition, the samples are independent and are less than 10% of the population. Therefore we can proceed with a confidence interval which will provide a better true population mean. This plausible range of values will be more likely to contain the true population mean.
( 542434.34 ) ( 542434.34 )
828,539.25 − 𝑡(.025, 19)( 20 ) < μ < 828,539.25 + 𝑡(.025, 19)(
( 542434.34 ) ( 542434.34 )
20 ) We are 95% confident that the true mean house price in New York, NY is between $574, 675. 08
828,539.25 − (2.093)( 20 ) < μ < 828,539.25 + (2.093)( 20 ) (574, 675. 08) < μ < (1, 082, 403. 418)
and $1, 082, 403. 418.

![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.42.31%20PM.png)

According to the Zillow website, the typical price for a home in NYC is $652,012 (the graph says New York but it’s referring to NYC). This value is almost $200,000 less than the estimated mean obtained from JMP, this is unquestionably because our sample size was very small. Since the average NYC house is in our 95% confidence interval, (574, 675. 08, 1, 082, 403. 418), our interval was a good estimator of the true mean value. Because the actual average is lower than our estimated sample average, we can see that our sample is right-skewed and our CI is the reason we were able to get close to the actual population average.

Had we taken a larger sample, let's say all 800 houses that were provided by Zillow, then our point estimate would have been more likely to be closer to the actual average according to the law of large numbers (more trials = closer to the actual value).

# How does this value compare to the average home price in your state and the national average?
![image](https://github.com/4nuG/Statistical-Analysis/blob/main/One%20Sample%20Inference%20for%20the%20Mean/Screenshot%202024-01-31%20at%204.45.03%20PM.png)
- The average house price in New York state is $331,459, which is less than our CI and actual NYC average. This makes sense as New York is a very large state so we cannot expect to find the average for the state from a sample taken from one city alone. The city we did take samples from happens to be the most inhabited and in-demand location for houses which is why NYC has such a high average. The same cannot be said of the state as a whole which has multiple metropolitan and rural areas averaging the high and low prices.
- The average price to buy a home in the United States is $272,446, according to Zillow which is way less than the estimated mean price of a home in NYC. New York is a very popular city and the price of a home takes into consideration a multitude of factors among them being: the proximity to public facilities, the scenery, education, utilities, and a lot more than a homeowner would know. On top of all the regular considerations in buying a house, with NYC having some of the nation’s best minds and resources, a house there would be very coveted (there are more apartments than houses listed, supply and demand).
