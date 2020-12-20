# PyBer_Analysis
Ridesharing Data Analysis and Visualization

## Overview
For this project, we've been taking a close look at ridesharing datasets, and creating charts that tell a compelling story about the data. In particular, we're examining the relationship between city type (urban, suburban, rural), the number of drivers and passengers, and total fares. Our analysis and visualizations are intended to help the (fictional) company "PyBer" improve ridesharing access and affordability for underserved communities.

This exercise focuses on the last part of the project, in which we've created a summary DataFrame of the ridesharing data by city type. We've also created a multiple-line graph that shows total weekly fares for each city type during the first four months of 2019. Below, we'll describe the differences in the data across city types, and make recommendations to the CEO for addressing these disparities. 

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
Earlier in our analysis, it quickly became clear that of our city types, urban communities had the highest ride counts, followed by suburbs, then finally rural areas. This isn't surprising given the relative population density of these city types, but the disparity is striking. The urban areas with the lowest ride counts are on par with the highest-ride count rural areas.

![Ride Count Data (2019)](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig2.png)

It would be helpful to join our data with city/community population figures and then generate "drivers per capita" figures to get a better feel for the relative ridesharing access for different city types. That said, even without that data, we can draw pretty good conclusions about access and affordability from fare data.

![Ride Fare Data(2019)](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig3.png)

From the chart above it's apparent that PyBer is most affordable for urban passengers, followed by suburban and finally rural riders. This suggests that driver supply is not meeting rider demand in rural, and to a lesser extent, suburban areas, as well as it is in urban communities.

The bubble charet below highlights the inverse relationship between average fares on one hand, and rides/drivers on the other. 

![Ride-Sharing Data (2019)](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/2019%20City%20Type%20Rides%20v%20Fares%20Bubble%20Chart.png)


* <br/>
<br/>
<br/>
![Average Fares](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Average%20Fares.png)

![Total Fares by City Type](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig5.png)

![Total Rides by City Type](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig6.png)

![Total Drivers by City Type](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/Fig7.png)

![Total Fare by City Type line](https://github.com/flowersmichael/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

## Summary



### Recommendations
* Provide incentives for drivers and passengers in rural areas
* Provide incentives for drivers and passengers in suburban areas
