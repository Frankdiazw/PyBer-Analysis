# PyBer-Analysis:iphone::taxi:

## Overview of the analysis:mag:
In this challenge an exploratory analysis was performed on some "csv" files for a company called PyBer. Performing data visualizations to show the relationship of the type of city, number of drivers and passengers, as well as the total percentage of fares, drivers and passengers by type of city. Graphs and data analysis were conducted to help improve shared transportation services and accessibility for underserved neighborhoods.

## Results:oncoming_taxi::round_pushpin:
- For the deliverable 1, Pandas groupby () function with the count () and sum () methods were used on the PyBer DataFrame columns, to obtain the total number of trips, the total number of drivers and the total fares for each type of city. The average fare per trip and the average fare per driver were then calculated for each type of city. Finally, this data was added to a new DataFrame, to format the columns.

![](https://github.com/Frankdiazw/PyBer-Analysis/blob/main/Resources/Deliverable%201.png)

- Figure 1. PyBer's ride-sharing summary DataFrame by city type.

- For the deliverable 2, the main goal was to create a multiple-line chart of total fares for each city type. For this a new DataFrame was created using groupby() function and then using the pivot() function to create a pivot table from the DataFrame to showcase the fare for the datetime of each city type. Subsequently, a new DataFrame by using the loc method on the date range of 2019-01-01 through 2019-04-28. Then, the resample() method was used to reset the index of the DataFrame created with the loc method to a datetime data type. To verify that the code was propertly used, the data_frame.info() method was used. Finally,  another DataFrame was created by applying the resample() function, in order to resample the data in weekly bins, subsequently to apply the sum() method to get the total fares for each week. The resulting DataFrame is shown below:

![](https://github.com/Frankdiazw/PyBer-Analysis/blob/main/Resources/Deliverable%202.1.png)

- Figure 2. Resampled DataFrame for the sum of fares for each city type on specific dates.

- Finally, the resampled DataFrame from Figure 2 was graphed using the object-oriented interface method and the df.plot() method, as well as the Matplotlib "fivethirtyeight" graph style code. The resulting graph is shown below:

![](https://github.com/Frankdiazw/PyBer-Analysis/blob/main/Resources/Deliverable%202.2.png)

- Figure 3. Resulting graph from the resample DataFrame.

- The graph in Figure 3, shows 3 lines that move from the first day of January to the last day of April 2019. The great differences between the fares of each city type can be observed, giving place to urban cities with the highest fares and the rural ones with the lowest rates. This is due to the fact that rural areas do not circulate much vehicles that can offer the ride-share service, while in more modernized areas this type of service is more easily offered.

## Summary:chart_with_upwards_trend:

Based on the outputs shown during the analysis, 3 business recomendations can be given to the CEO of PyBer. The recomendations are the following:

- We can see in figure 1, that urban cities remain with the highest total number of rides with 1625 total rides, however there is an even greater number of total drivers with 2405. This creates an inequality leaving some drivers without trips, wasting money from the company. It is recommended to lower that number of drivers to satisfy the ratio between the total number of trips and drivers.

- Little has been said with the suburban cities, we can see in Figure 2, that along the date range from January to April, urban cities almost doubles up in the sum of fares and rides to suburban cities. In order to activate this sector, we need to open more job opportunities to hire more drivers in this city type. With that, not only will the amounts of rides be increased, but the rates will be lowered to save more money for the company and at the same time generate more money.

- The rural cities, due to their small size and little traffic, are perfect for active mobility. Walking or cycling should be the first option to move within the municipality. But there comes a time when it is necessary to leave town, either to work, to go to the institute, to the doctor, to shop, or for leisure. Due to these factors, it can be observed in Figure 1, how rural areas remain in last place in almost everything. Analyzing the situation, two ideas are raised to activate this sector: The first would be to hire more drivers, this will cause the average fare per ride rates to decrease, making it more accessible to customers to use this service.
The second would be to add some type of shared ride so that in the same way, customers can access this service more frequently.
