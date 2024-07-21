# Practical Application Assignment 11.1: What Drives the Price of a Car?

Assignment 11.1 is a python project showing my ability to apply the full CRISP=DM framework to a business problem.  


## Contact 
If you want to contact me you can reach me at contactbethford@gmail.com

## Files
* AIML_B2C_Coupon.ipynb - Main python script with full charting and data
* CouponByGender.jpg - Bar graph that shows coupons redemption by type and gender
* PassengerTypes.jpg - Visual to show how redeemed coupons decline with a passenger when they do not have time 
* README.md
* Data comes from a used car data set of 426K rows provided from Berkely through coursework for AI/ML originally from Kaggle with 3 million records

## Objective
In this project we are looking to understand what factors make a car more or less expensive

## Findings

**Overall**
- 7210 coupons were redeemed, 56.8% of total coupons
- Drivers that redeem coupons are slightly younger
- More drivers with incomes $100K, used a coupon (57.8%) 
- More coupons are redeemed at 6pm than any other time of day

**Coupon Types & Redemptions**
- When passengers were traveling with friends, kids or a partner, coupon use was strong when they were not in a rush 
![Traveling With Passenger Image](PassengerTypes.jpg "Coupons used more when not in a rush")
- Fine dining is the least popular coupon overall
- People that are alone redeem more coupons
- Most popular coupon for females is takeaway, followed by casual dining
- Males also prefer takeaway, but have a significant preference for bar coupons
![Redemption by Gender](CouponByGender.jpg "Males prefer bar, females takeaway and casual")

**Bar Coupons**
- 41% of bar coupons were redeemed
- The younger that the driver is and the more on their own, the more they redeem bar coupons
- Bar coupons are successful in getting people who have never been to a bar to redeem

**Carry Away Coupons**
- Most Carry Out coupons are used for breakfast
- The least popular time is 2pm

**Coffee Coupons**
- Most coupons are redeemed at 10am, but very few redeemed when it is below freezing
- Coffee houses have the most coupons that expire quickly in 2 hours (962) 

**Fine Dining ($20-50)**
- Fine dining coupons are used the most in warmer temperatures
- 75.7% of all coupons expire in 24 hours

**Casual coupons ($20)**
- 6pm and 80 degrees is the most popular time
- Coupons that are geolocated more than 25 minutes, are not very successful, in this case only 101 redeemed


## Recommendations
- Drivers are not redeeming coupons that are greater than 15 minutes from their location.  Increase reinvestment for drivers that are not in a rush and more than 15 minutes away 
- Carry out is successful in the morning.  Look at a campaign that targets drivers on the way home from work to get dinners for their families. 
- Try to increase spend for drivers with high income that use coupons by pointing them to higher cost items
- Change bar coupon creative to target bar coupons to females
- Update coffee house creative to highlight hot drinks at coffee house to warm drinks in cold weather
