# Practical Application Assignment 11.1: What Drives the Price of a Car?

Assignment 11.1 is a python project showing my ability to apply the full CRISP=DM framework to a business problem.  


## Contact 
If you want to contact me you can reach me at contactbethford@gmail.com

## Files
* 11.1.ipynb - Main python script with full charting and data
* Ridge Coefficients Greater Than .25.png - Bar graph that shows top drivers of price
* Ridge Coefficients Less Than -.1.png - Bar graph that shows top detractors of price
* README.md

## Objective
In this project we are looking to understand what factors make a car more or less expensive

## Methodology

As the objective was to make recommendations to used car dealerships, I first removed cars that were considered luxury, with the average proce of a Lamborghini being $222K.

I then only looked at cars that were 2014 and older as technology and features in cars has changed so drastically from more than 10 years ago.

The data quality was lacking.  With descriptive fields like color with so many missing values, they were removed from the data set.

**Modeling:**
- 151,550 records
- Seven fields (price, age, odometer_log, fuel, transmission, type, manufacturer, drive)
- I ran feature selection with Lasso to see what features had zero coefficients
- I ran a GridSearchCV and found that alpha=10 was the best parameter and for Lasso, 0.01
- I ran three types of regression models (Linear, Ridge and Lasso) with the best hyperparameters
- Cross validation of scores returned very similary results as test


**Overall Findings**
- Ridge model was the best performing model, indicating that the larger price values may need to be handled differently
- The R2 was only .3186 indiacting that this model may only be identifying approximately one-third of the drivers for this model.

**Coefficients**
- Top luxury manufacturers like ferrari and porsche drove the highest price.  When not looking at manufacturers, convertibles had the largest coefficient great than .6
- Harley Davidson drove the lowest price but this is most likely due to the harley being a motorcycle so inherently less expensive than a car
- Fuel type was also not a driver of price with coefficients less than -0.5

## Recommendations
- Keep more Trucks and Convertibles in stock as this will increase your the dealer's prices.  See image "Ridge Coefficients Greater than .25".png
-  Rear Wheel Drive (RWD) is a stronger driver than Front Wheel Drive (FWD) See image "Ridge Coefficients Less Than -.1".png
- Car manufacturer is key.
- The created field 'age' might have had multicolinearity with the odometer log, but age had a much higher negative impact than odometer. 
- Ask the client specifics on types of manufacturers they will have on their lot.  This may get rid of some luxury vehicles examined for better results.
- Data quality was an issue here with alot of nulls.  Try running some models on smaller data sets that have more fields to consider in the regression models.
