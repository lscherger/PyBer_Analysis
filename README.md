# PyBer_Analysis
Analyze PyBer ride-share data using Python 3.9.6 and Jupyter Notebook 6.3.0

## Overview of Project

### Background
As an introduction to Matplotlib, this project utilizes plots in Pandas DataFrames with Python to analyze PyBer ride-sharing data. In the original project, I analyzed ride-sharing data from January 2019 through April 2019, and created plots to visualize the difference in total fares and total rides for each city type (urban, suburban and rural) in bubble plots, box-and-whisker plots, and pie charts.

### Purpose
The CEO of PyBer, V.Isualize, additionally requested a new analysis, including a summary and line plot to show how fares changed over time for each city type. The purpose of this analysis is to identify differences in ride-sharing data among the different city types, then make recommendations to address disparities among the city types.


## Results

### Deliverable 1: _A ride-sharing summary DataFrame by city type_

**Image 1: Ride-sharing data includes the total rides, total drivers, total fares, and average fare per ride and driver.**

<img width="494" alt="Screen Shot 2021-07-20 at 12 05 38 PM" src="https://user-images.githubusercontent.com/85946042/126365962-dc357978-6a9c-49dd-9814-cbb448f59a53.png">

Total ride counts increase as city population size increase; rural cities had 125 total rides, suburban cities had 625 total rides, and urban cities had 1625 rides. 
Total ride counts for urban cities were 13 x the total ride counts for rural cities. 

The total fares increase with total ride counts; total ride fare was $4,327.93 for rural cities, $19,356.33 for suburban cities, and $39,854.38 for urban cities. Total fares for urban cities were over 9 x the total fares for rural cities.

Still, the average fare per ride is highest in rural cities. Average fare per ride decreases as city population size increases; rural cities averaged $34.62 per ride, suburban cities averaged $30.97 per ride, and urban cities averaged $24.53 per ride. Average fare per ride for urban cities was about 71% of that of rural cities.

Total driver counts increase as city population size increase; rural cities had 78 total drivers, suburban cities had 490 total drivers, and urban cities had 2405 drivers. Total driver counts for urban cities were over 30 x the total driver counts for rural cities. 

Still, the average fare per driver is highest in rural cities. Average fare per driver decreases as city population size increases; rural cities averaged $55.49 per driver, suburban cities averaged $39.50 per driver, and urban cities averaged $16.57 per driver. Average fare per driver for urban cities was about 30% of that of rural cities.

Finally, it it important to recognize that in rural and suburban cities, total ride count is larger than total driver count, which suggests that some drivers make multiple trips in rural and suburban cities. In urban cities, there is a higher number of total drivers than total rides, which suggests that some drivers in urban cities did not make trips during this time period. 


### Deliverable 2: _A multiple-line chart of total weekly fares for each city type_
**Image 2: The line plot shows total weekly fare by city type over the months of January through April 2019.**
<img width="829" alt="Screen Shot 2021-07-20 at 12 23 15 PM" src="https://user-images.githubusercontent.com/85946042/126368313-2bf5e083-dc73-4bbd-a7fb-67b03d7a9cc7.png">


Image 2 illustrates how the total weekly fare by city type, defined in Image 1, changes over time from January through April 2019. The total weekly fares of city type do not overlap at any point in the time frame, suggesting that there is a major difference in fares between the three, as was seen in the total fares column in Image 1. By viewing the chart, total suburban city weekly fares stay an estimated $500 - $1200 greater than total rural city weekly fares. Additionally, via the chart, total urban city weekly fares stay an estimated $700- $1700 greater than total suburban city weekly fares. The weekly fares by city type individually only seem to fluctuate by at most $800 roughly. 

All city types have a spike in weekly fares in late February, but other than that, do not follow the same trends as time passes. The lack of a similar trend from each city type might suggest that PyBer popularity and usage differs based on city type; people may not be taking PyBer for the same reasons, such as events or holidays, as other people in other city types. This means there are other confounding variables, such as weather patterns or festival events, for instance, that need to be analyzed to understand the motivators for taking PyBer rides in different city types.

## Summary
The results show that there is a difference in PyBer ride-sharing total fares between different city types. Because the different city types' total fares do not overlap over the time frame, there is evidence to suggest there are other factors that are creating disparities among the city types that need to be explored. While I can suggest recommendations for _addressing_ disparities among the city types by looking for other relationships in the data, it is difficult to recommend program implementations without knowing the direction that the company wants to take, i.e. making fares lower or higher across the board to match fares of one city type, etc.

Firstly, I would analyze the average ride duration, both by minutes and miles, for each city type. This is important to understand why rides in different city types are resulting in different total fares. For this recommendation, there are other questions to consider: 
* Is the fare calculated by ride duration by time or distance?
* How do gas prices change by different city type?
* Does highway usage during rides change by different city type?
* Does the fare calculation factor-in traffic to account for gas used for short but crowded routes?
* Is there an incentive to drive in a certain city type because ride fare is larger or covers gas costs more fairly?

Secondly, I would analyze the proportion of rides to drivers for each city type. This is important to understand if there is a difference in demands for rides or drivers between city types. For this recommendation, there are other questions to consider:
* If there is an excess of drivers in the city, is demand lower? Are drivers able to make money in larger cities if there are less ride requests compared to drivers available? Are some drivers not driving because there are not enough rides being requested?
* If there are more rides than drivers, like in rural and suburban cities, are drivers incentivized by more rides being available? Is it necessary to recruit more drivers in rural areas so it is easier to get a ride? Are rides more expensive in rural cities because they are more spread out and require longer rides, or because there are less drivers, creating a larger demand and price for a ride?

Thirdly, I would analyze the frequency of ride counts in each time frames of the day for each city type. This is important to understand _why_ people are taking PyBers in the first place. PyBer should study this information so that they can brief drivers when they start so they can be most successful and plan for how many people they expect to onboard in different city types. For this recommendation, there are other questions to consider:
* Are more people using PyBer for daytime functions (work, school, etc.) or nighttime functions (attending restaurants, bars or concerts)? How does the ride frequency by time frame change by city type? 
* Does the average amount of bars in a city affect the ride count? 


By exploring data in different ways with each of these recommendations, PyBer may find confounding variables that are affecting fares by city type significantly. Finding confouding variables that affect fares can help them make decisions on how to reduce disparities among city types. 
