# PyBer_Analysis
## Overview of the Analysis
This new analysis was created in order to determine rider, driver, and fare data based on city type. The first step was to combine the data frames for the ride data and city data. This new data frame was then filtered down, setting the date as the index, and eventually showed a data table separated by city type that included every ride on every date between 1/1/2019 and 4/28/2019. After this additional filtering was completed, a line chart was created in order to provide a clearer visual representation of the number of rides for each type of city. The charts created helped visualize the successes and disparities between city types and will help inform the CEO to address any issues the company might have.

- To perform the analysis, I used Pandas and Matplotlib in the Jupyter Notebook application.

## Results
After combining the data and filtering it down to the desired specifications, there are a few conclusions that can be made about the ride data based on city type. See below for a chart and a graph of the analysis results:

#### Challenge Results Table

![City_type_table](https://user-images.githubusercontent.com/94764735/151709937-e81cadf7-f137-400e-b8ae-6e677f50b0df.png)

#### Graph of Weekly Fare Data

![City_type_graph](https://user-images.githubusercontent.com/94764735/151709939-c450081f-348c-4141-9adb-828b4459490c.png)

### Conclusions
- There are far more drivers in urban cities than in rural cities, and the number of suburban drivers falls between the two. 
- The total number of rides follows the same order: Rural has the fewest, then suburban, and urban has the most.
- The total fares from each city type again follows this order: urban has the most, then suburban, then rural.
- Interestingly, the order reverses for the average fare per ride and average fare per driver. Rural has the highest averages, followed by suburban and then urban.

Regarding the graph of weekly fare data, it mainly just visualizes what the table tells us about total fares. The total fare revenue is highest for urban cities, second highest for suburban cities, and lowest for urban cities. It is nice to see how the total fares fluctuate week to week, however, this really will only help with future projections and not much else. 

### Interpreting the Results
These results do not really come as a surprise. Considering how supply and demand works, it makes sense that there are more drivers in urban cities than there are in rural cities. In urban cities there are more people, and more people means there are going to be more rides requested. Also, if there are more rides being requested, that means there is a need for more drivers. As a result, having the most drivers and rides means that urban cities are going to have the highest fare total, followed by suburban and then rural. 

Regarding the average fare per ride and per driver, there are a couple of possible explanations as to why the order reverses (rural = highest, suburban = middle, urban = lowest):

 - One possibility is that perhaps the average ride in urban cities is shorter distance-wise than the average ride in rural cities. This would make sense because urban cities are often more condensed. So, when a customer gets a ride somewhere in an urban city, it is more likely that their destination is close by. On the other hand, rural cities tend to be in agricultural areas where houses are normally more spread out. So, if someone were to get picked up at their home in a rural city, their destination is probably a lot farther away than it would be if they lived in an urban area. 
- A second possibility is that rides are just cheaper in urban cities than in rural cities. According to supply and demand, prices are influenced by how much supply of the resource there is. If there is an abundance of said resource, it is not going to be very expensive as it will be easier to come by. However, if it is a scarce resource, it is harder to come by and therefore more valuable. So, applying this to the ride and driver data, it would make sense if the cost of a ride is lower in urban cities that have more drivers and higher in rural cities that have less drivers.
- That being said, there could be a third option that is basically just a combination of the first two. The reason that fares per ride and per driver are lowest in urban cities could be because the average cost of a ride is cheaper there AND the average ride is shorter.

## Summary
### Proven Result
After reviewing the possible explanations for the outcome of this analysis, the second possibility is the only one that can be proven using the data. It must be true that rides are cheaper in urban cities, second cheapest in suburban cities, and the most expensive in rural cities. The ratio of total rides to total drivers in rural cities is about 1.6, meaning that the average driver gave 1.6 rides. In suburban cities, that ratio is just under 1.28, slightly less rides for each driver. However, in urban cities, the ratio doesn’t even surpass 1 (it’s about 0.68). This means that there are several drivers that didn’t even give a single ride over the period that this data was collected. Thus, since there is a surplus of drivers in urban cities, the market response to that surplus would be to lower the price of a ride to make it more attractive to the customer.

### Recommendations
- Due to this apparent surplus, I would recommend focusing on urban cities and fixing the issue. Unfortunately, reducing the surplus might require laying off some of the drivers to reduce ride availability. Alternatively, if there were a way to increase the demand for a ride, that could help solve the problem as well.

- In addition, I would recommend gathering ride duration data to add to this data set. Calculating the average duration of a ride, as well as the average cost per minute of a ride I believe is important to include in an analysis like this. If it is discovered that the average duration of a ride in an urban city is shorter than that in a rural city, it could help explain why the average fare per ride is so much lower in urban cities.

- I would also recommend gathering ride distance data. Much like with ride duration data, we could compare the average distances of rides in rural vs urban cities and see which one is longer. If the rides are longer in rural cities, that would be a contributing factor to the differences in average fare per ride. If the average durations are pretty similar among all city types, the data would then tell us that we might want to weight the fare prices more based on ride duration. 

Using both the ride duration and ride distance data, we could determine a better fare rate for our drivers. We could alter the rates based on city type and try to lessen the gap between rural/urban in the average fare per ride and average fare per driver data.

