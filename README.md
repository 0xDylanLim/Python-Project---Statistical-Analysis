You are a member of an analytics team for the United States Environmental Protection Agency (EPA). The data includes information about more than 200 sites, identified by state, county, city, and local site names. One of your main goals is to determine which regions need support to make air quality improvements. Given that carbon monoxide is a major air pollutant, you will investigate data from the Air Quality Index (AQI) with respect to carbon monoxide.

This project involves the use of Python to perform statistical analysis on AQI.

- Z scores
- Best fits Data
- outlier detection
- sampling techniques
- Confidence intervals
- Hypothesis testing
- Visualisations on various state AQIs


----- DESCRIPTIVE STATISTICS -----

.head function displays the first 10 rows of the data.

![Screenshot 2023-06-26 171815](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/aaaca5c5-be64-4352-b69c-7cf387aa2c68)

.describe shows the statistics of the data.

![Screenshot 2023-06-26 171926](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/a7dc1dfb-cfe2-4747-81b8-25e2303d3c6b)

The count row shows that for the aqi column, there are 260 values. We can individually code for these values using .mean, .median, .min, .max, .std, 

----- PROBABILITY DISTRIBUTIONS -----

The code for this section involves a modified version of the original AQI data.

![Screenshot 2023-06-26 172358](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/88c253ca-ec59-4754-b1cb-9d7288bff88a)

By creating a histogram or qq_plot of the aqi_log column, we can see that it follows a normal distribution.

![Screenshot 2023-06-26 172525](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/51bc0e88-49e0-43dc-a855-4317c92ea5c2)

![Screenshot 2023-06-26 172557](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/ddc9788f-7ad8-4e99-90e8-b691659c9805)

Let's perform a statistical test on this data. First, define two variables to store the mean, standard deviation, lower limit, and upper limit.

limits = mean - 1 * std

We can calculate the percentage of data within each standard deviation (1-3) by increasing the standard deviation.

About 76.15% of the data falls within 1 standard deviation of the mean.
About 95.77% of the data falls within 2 standard deviations of the mean.
About 99.62% of the data falls within 3 standard deviations of the mean.

----- SAMPLING -----

First, we can define the population mean, then create a sample from the entire dataset. This will allow us to run statistical tests in the future. Let's test the central limit theorem, by reiterating the sampling test 10,000 times. We will see that the sample mean should roughly equal the population mean as more random samples are taken. This sampling test involves sampling with replacement. A histogram helps visualize this by creating a new data frame of the mean of the sum of the mean of each sampling test.

![Screenshot 2023-06-26 174304](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/4f568ef7-6137-4e18-9ebe-bdc0a73205d1)

The standard error of a statistic is the standard deviation of the sampling distribution associated with the statistic. It is a measure of sampling variability.

![Screenshot 2023-06-26 174630](https://github.com/0xDylanLim/Python-Project-Statistical-Analysis-on-Air-Quality-Pollution/assets/98394792/456e0b85-9c8d-492f-99cc-e10ac416d843)

----- CONFIDENCE INTERVAL -----



















