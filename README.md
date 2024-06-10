# Machine-Learning-Tasks

## 1.Outlier Detection(House price.ipynb):

Outlier detection is a crucial step in data analysis that involves identifying and handling data points that deviate significantly from the rest of the dataset. Outliers are observations that lie far away from the majority of the data points and can distort statistical analyses, leading to biased results and inaccurate interpretations. Detecting outliers is essential for ensuring the integrity and reliability of data analysis.

Various methods can be used to detect outliers, including statistical techniques and visualization methods. Statistical methods often rely on measures of central tendency and dispersion, such as the mean, median, standard deviation, and interquartile range (IQR). These methods define thresholds or ranges beyond which data points are considered outliers and are subsequently removed or treated.

Visualization techniques, such as box plots, scatter plots, and histograms, provide graphical representations of the data that facilitate the identification of outliers. Box plots, for example, display the distribution of the data and highlight potential outliers as points beyond the whiskers of the plot. Scatter plots allow visual inspection of relationships between variables, making it easier to identify data points that do not conform to the expected patterns.

It's essential to consider the context of the data and the specific objectives of the analysis when choosing an outlier detection method. While some methods are suitable for normally distributed data, others are more robust to skewed distributions or outliers of varying magnitudes. Additionally, outlier detection should be conducted iteratively, as removing outliers can impact subsequent analyses and may require reassessment of the data.

Overall, outlier detection is a critical aspect of data preprocessing that helps ensure the accuracy and validity of analytical results. By identifying and appropriately handling outliers, analysts can improve the quality of their analyses and make more informed decisions based on reliable data.

## Mean Function:

This method involves calculating the mean and standard deviation of the data. Outliers are then defined as data points that lie outside a certain range around the mean, typically a specified number of standard deviations. For example, outliers can be identified as data points lying more than 3 standard deviations away from the mean. These outliers are considered to be atypical and are removed from the dataset.

## Percentile Method (IQR):

The percentile method, also known as the Interquartile Range (IQR) method, involves calculating quartiles (Q1 and Q3) and the Interquartile Range (IQR = Q3 - Q1). Outliers are then defined as data points that fall below Q1 - 1.5 * IQR or above Q3 + 1.5 * IQR. This method is based on the spread of the middle 50% of the data and is less sensitive to extreme values than the mean method.

## IQR (Interquartile Range) Method:

Similar to the percentile method, the IQR method also relies on quartiles and the Interquartile Range. Outliers are defined as data points lying beyond a certain range from the first and third quartiles. However, unlike the percentile method, the IQR method does not involve specific percentiles and is often used to identify outliers in skewed distributions.

## Normal Distribution:

In this method, data points are evaluated based on their deviation from the mean in terms of standard deviations. Z-scores are calculated for each data point, representing how many standard deviations it is away from the mean. Typically, data points with a Z-score greater than a predefined threshold (e.g., 3) are considered outliers and are removed from the dataset. This method assumes that the data follows a normal distribution.

## Z-score Method:

The Z-score method is essentially the same as the normal distribution method. It calculates the Z-scores for each data point and compares them to a predefined threshold to identify outliers. However, unlike the normal distribution method, the Z-score method is more general and can be applied to any distribution, not just normal distributions.

## 2 - Hypothesis testing

Q1.Suppose a child psychologist claims that the average time working mothers spend talking to their children is at least 11 minutes per day. You conduct a random sample of 1000 working mothers and find they spend an average of 11.5 minutes per day talking with their children. Assume prior research suggests the population standard deviation is 2.3 minutes.Conduct a test with a level of significance of alpha = 0.05.

Q2. A coffee shop claims that their average wait time for customers is less than 5 minutes. To test this claim, a sample of 40 customers is taken, and their wait times are recorded. The sample mean wait time is found to be 4.6 minutes with a standard deviation of 0.8 minutes. Perform a hypothesis test at a significance level of 0.05 and determine whether there is enough evidence to support the coffee shop's claim.

## 3 - Data Preprocessing

Objective: The main objective of this project is to design and implement a robust data preprocessing system that addresses common challenges such as missing values, outliers, inconsistent formatting, and noise. By performing effective data preprocessing, the project aims to enhance the quality, reliability, and usefulness of the data for machine learning. 
Key Components to be fulfilled: Data Exploration: Explore the data, list down the unique values in each feature and find its length. Perform the statistical analysis and renaming of the columns. Data Cleaning: Find the missing and inappropriate values, treat them appropriately. Remove all duplicate rows. Find the outliers. Replace the value 0 in age as NaN Treat the null values in all columns using any measures(removing/ replace the values with mean/median/mode) Data Analysis: Filter the data with age >40 and salary<5000 Plot the chart with age and salary Count the number of people from each place and represent it visually Data Encoding: Convert categorical variables into numerical representations using techniques such as one-hot encoding, label encoding, making them suitable for analysis by machine learning algorithms. Feature Scaling: After the process of encoding, perform the scaling of the features using standardscaler and minmaxscaler.
