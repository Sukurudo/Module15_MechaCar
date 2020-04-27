# Challenge 15
## MechaCar Analysis


## MPG Regression

-Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The Data set correlation analysis shows that two variables provided a non random amount of variance to the MPG values: These variables were Vehicle Length, and Ground Clearance

The other variables did not provide a significant amount of variance.


-Is the slope of the linear model considered to be zero? Why or why not?

The slope of the linear model is not zero; This is because we have predictors that are considered significant (Vehicle Length and Ground Clearance) and thus the slope is not Zero.


-Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The Linear Model can be used to predict MPG of MechaCar because the adjusted R-squared value is high; However we might be able to get better results by removing the non-significant values, as this reduces the P-Value of the model and can give better and more accurate results.


## Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per inch. Does the current manufacturing data meet this design specification? Why or why not?

The variance of the entire lot of suspension coils falls within the 100 PSI variance limit; however once you separate the data by lot, you will notice that Lot 3 has fallen out of spec.

Lot 1 has a variance of .98, Lot 2 has a variance of 7.47, well within spec.
Lot 3 has a variance of 170, which falls far out of the 100 limit.

Further investigation needs to happen to see what changes were made in Lot 3 that can contribute to the failure.


## Suspension Coils T-Test

Based on a two sided T-test on the PSI of the suspension coils, our results show that the sample tested with a mean of 1498.78, which are very close to the mean results of 1500. The P-value of 0.06 shows that results are not statistically different.


### Further Analysis:

In order to continue to review MechaCar against the market, there are quite a few analysis that can be worked upon. Items such as MPG comparison to comparable cars, Number of color options, or comparison of drive train, are all important options. Two of the studies that I feel could be most  relevant are: MSRP (Cost of the vehicle to the consumer) and Number of technological upgrades available.

MSRP (Manufactures suggested retail price) determines what type of consumer the vehicle will appeal to. How does MechaCar compare to the MSRP of cars with similar features? Is MechaCar more or less expensive than comparable cars. The first question to ask would be what features would be relevant in the comparison: Examples would be number of doors, weight, Drive Train, MPG, etc.. Once the factors have been determined, then we can compare the MSRP of those vehicles to the MechaCar.

Question: is there a statical difference between the mean prices of the samples
H0: Is MechaCar's MSPR greater than the MSRP of similar cars on the market?
Ha: MechaCar's MSRP is less than or equal to the MSRP of similar cars on the market.
Testing method: Two Sample T-Test


The second question deals with the cabin and options available for the car. How could the technological offerings of the MechaCar affect its popularity? In order to understand this, we would first need to make a list of technological offerings available in current cars that could be significant to the consumer: Examples of this would be Car/Android Play, GPS, USB chargers, Seat Warmers, Climate Control, Cameras, etc. Once a list has been determined, then we can compare the sales of vehicles that have and don't have these features, and use the sales records to determine their impact on the market.

Overall we can use a simple linear regression to compare number of available options to sales: and we can refine our analysis by doing independent studies on some of the individual options.

Question: Is there a correlation between number of options to sales in a year?
H0: There is no correlation between number of options and sales
Ha: there is a correlation between number of options and sales
Testing Method: Simpel Linear Regression


