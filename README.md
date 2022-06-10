# MechaCar_Statistical_Analysis
The MechaCar dataset contains mpg test results for 50 prototype MechaCars. They were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, including; vehicle length, vehicle wieght, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using R, I have designed a linear model that predicts the mpg of MechaCar prototypes. 

### Resources
R, MechaCar_mpg.csv, suspension_Coil.csv

## Linear Regression to Predict MPG
![6columns](https://user-images.githubusercontent.com/99093289/172077224-6e322aa2-c6d4-4e33-8c7d-c11dfc827a7c.PNG)

![p-value_r-squared](https://user-images.githubusercontent.com/99093289/172077222-f48d9fcf-1f47-472a-8d4b-fe5f2bfeacc1.PNG)

According to the linear model, vehicle length and ground clearance provide a non-random amount of variance to the mpg values in the dataset. The p-value is 5.34e-11, and smaller than the significance level of .05. This indicates that the slope is not zero. This linear model does predict mpg effectively, as the r-quared value of .7149 means that there is a strong correlation between the variables.

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![total summary_coil](https://user-images.githubusercontent.com/99093289/172078447-e6a0f88b-d531-494b-a9f6-b94eda2a9d42.PNG)

![lot_sumary](https://user-images.githubusercontent.com/99093289/172078629-a0caf9dc-65fb-412f-a3e6-966f686787b8.PNG)

According to the total summary, the variance of the suspension coils is less than 100 pounds per square inch, but when we look at the individual lots, we can see that lot 3 has a variance of 170. This does not meet the design specification on the individual lot. 

## T-Tests on Suspension Coils
These tests were used to determine if the PSI is statistically different from the population mean of 1500 pounds per square inch. 
### All manufacturing lots
The p-value is 1 and is significant. The null hypothesis can be accepted.

![all lots t-test](https://user-images.githubusercontent.com/99093289/172079590-c8f96b51-287c-4077-a65d-98ecbc4146cd.PNG)

### Lot 1
The p-value is 1 and is greater than .05. The null hypothesis can be accepted.

![lot 1 ttest](https://user-images.githubusercontent.com/99093289/172970622-eb3df915-bcb1-4b26-9bf8-309552649ca3.PNG)


### Lot 2
The p-value is .6072 and issignificant. The null hypothesis can be accepted. 

![lot 2 ttest](https://user-images.githubusercontent.com/99093289/172970633-5c5c85e2-aad8-469f-9c00-32109a38ca90.PNG)

### Lot 3
The p-value is .04168 and is not significant. The null hypothesis can be rejected. 

![lot 3 ttest](https://user-images.githubusercontent.com/99093289/172970641-5e2e831c-fe9c-45d0-a448-a97cdb8fc6d0.PNG)

## Study Design: MechaCar vs Competition
MechaCard should test highway fuel efficiency. Are MechaCars as fuel efficient as the competitor? The null hypothesis would be, "do MechCars average more miles per gallon than the competitor?". This would be tested with a t-test because it will tell us if there is a statisitical difference in the means for the average fuel efficiency. The data we would need is the distance travelled per unit volume of fuel used.
