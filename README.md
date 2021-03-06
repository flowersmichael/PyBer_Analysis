# PyBer Analysis
Ridesharing Data Analysis and Visualization

## Overview
For this project, we've been taking a close look at ridesharing datasets, and creating charts that tell a compelling story about the data. In particular, we're examining the relationship between city type (urban, suburban, rural), the number of drivers and passengers, and total fares. Our analysis and visualizations are intended to help the (fictional) company "PyBer" improve ridesharing access and affordability for underserved communities.

This exercise focuses on the last part of the project, in which we've created a summary DataFrame of the ridesharing data by city type. We've also created a multiple-line graph that shows total weekly fares for each city type during the first four months of 2019. Below, we'll describe the differences in the data across city types, and make recommendations to the CEO that might address these disparities. 

## Resources
* Data Sources:  
    city_data.csv  
    ride_data.csv  

* Software:  
    Python 3.7.6  
    Pandas library  
    Matplotlib version 3.2.2  
    Anaconda Jupyter notebook (server version 6.0.3)  

## Results
Earlier in our analysis, it quickly became clear that of our city types, urban communities had the highest ride counts, followed by suburbs, then finally rural areas. This isn't surprising given the relative population density of these city types, but the disparity is striking. The urban areas with the lowest ride counts are on par with the highest-ride-count rural areas.

![Ride Count Data (2019)](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig2.png)

It would be helpful to join our data with city/community population figures and then generate "drivers per capita" figures to get a better feel for the relative ridesharing access for different city types. That said, even without that data, we can draw pretty good conclusions about access and affordability from fare data.

![Ride Fare Data(2019)](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig3.png)

From the chart above it's apparent that PyBer is most affordable for urban passengers, followed by suburban and finally rural riders. This suggests that driver supply is not meeting rider demand in rural areas, and to a lesser extent, suburban areas, as well as it is meeting demand in urban communities.

The table below shows the average fares per ride and driver...

![Average Fares](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Average%20Fares.png)

Here are a few key observations:
* There are more total drivers than rides in urban areas.
* Average fares per ride are highest in rural areas, followed by suburban cities, and finally urban communities.
* Note the *extremely* wide gap between average fares for urban drivers versus rural drivers.

The bubble chart below plots each city's average fare against total rides, with bubble sizes adding a third dimension by expressing driver counts. This visualization highlights the inverse relationship (observe how the data form a downward sloping line, and how the bubble sizes increase, from the top left of the chart to bottom right) between average fares on one hand, and rides/drivers on the other.

![Ride-Sharing Data (2019)](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/2019%20City%20Type%20Rides%20v%20Fares%20Bubble%20Chart.png)

We also looked closely at the first four months of 2019. See the line chart below: 
![Total Fare by City Type line](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

This subset of the data demonstrates that the total fares of each city type, relative to each other, generally didn't change much on a week-to-week basis between January and April of 2019.

## Summary and Recommendations

From our analysis of PyBer's ridesharing data from 2019, it's clear that rural passengers' average fares are highest, followed by suburban passenger fares and finally urban riders. One key piece of data that we don't have is the length and duration of each ride. The average fares might be higher in rural areas because the rides tend to be longer in distance and duration. Based on the data we have, however, I would make the following recommendations to the CEO:

1. Adjust ride rates in rural areas, and/or provide discounts and incentives for passengers in rural areas. The higher fares up to this point have possibly discouraged people from trying PyBer, and/or continuing to use PyBer.

2. Recruit drivers in rural areas, either by incentivizing urban drivers to work in rural areas, or recruiting new drivers in rural areas. Current drivers in rural areas are likely happier with their income than urban and suburban drivers. They are enjoying significantly higher average fares than their urban counterparts in particular. This is good for rural drivers, but the data suggests that PyBer needs to increase the supply of rural drivers in order to make rides more affordable for passengers. Perhaps PyBer can incentivize urban drivers that live somewhat close to rural areas to target rural areas. It also might be wise to offer strong referral bonuses to rural drivers, as they know who among their contacts might be good driver candidates in their communities.

3. Adopt these rural-area recommendations for suburban areas as well, but to a lesser extent.

