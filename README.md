# Project Overview
The results of the analysis were requested to make a presentation about the research to the CEO. 
Values for January, February, March and April 2019 are included in the study.
The analysis includes statistical summaries, plots of analytical results, and the recommendations based on them.

## Resources

•	Datasets:
* city_data.csv
* ride_data.csv

•	Software: 
* Python 3.9.12
* Jupyter Notebook 6.4.8
* Pandas 1.4.2
* Numpy 1.21.5
* Matplotlib 3.5.1
           
# Overview of the Analysis
We have two data sets. One of them is city_data_csv and the other is ride_data_csv. First of all, both tables are examined separately and the total number of rides and drivers for each city type is determined. Likewise, the total fare values for each city type and the average fares per drivers and rides were also examined. Then, by examining the date-based index, a time-dependent change graph of wage ranges and multiple value ranges was created.

# Results

### Table 1. City Type for Rides & Drivers and 
<img width="613" alt="D1_Step6_Output" src="https://user-images.githubusercontent.com/26927158/195757525-c86c49b9-bb2b-4330-9ad8-3f9bcaa9f953.png">

If the analysis results for Table 1 are to be interpreted, the city types are rural, suburban and urban. And for these city types, we have total rides, total drivers, total fares, average fare per ride and average fare per driver columns. However, it seems that no currency is used for the columns total fare, average fare per ride, and average fare per driver, and this will be analyzed in table 2.

### Table 2. PyBer Summary Data Frame 
 <img width="610" alt="D1_Step8_Output" src="https://user-images.githubusercontent.com/26927158/195757541-b79c14ba-6206-49a2-96f1-eb3a3ef1a84e.png">

In the above table, the values for table 1 will be examined in detail. When commenting on City type rural;
- 125 of the total number of rides,
- 78 of the total number of drivers,
- Total fares $4,327.93,
- Average fare per ride is $34.62 and
- The average fare per driver is $55.49 in the table.

When commenting on City type suburban;
- 625 of the total number of rides,
- 490 of the total number of drivers,
- Total fares $19,356.33,
- Average fare per ride is $30.97 and
- The average fare per driver is $39.50 in the table.

When commenting on City type urban;
- 1,625 of the total number of rides,
- 2,405 of the total number of drivers,
- Total fares $39,854.38,
- Average fare per ride is $24.53 and
- The average fare per driver is $16.57 in the table.
In general, if the table is to be interpreted, it is observed that as the number of population increases in the context of the city, that is, as the transition from rural to urban, the number of people and total fares increase, but the average fares per ride and driver decrease. The reason for this is that the probability of finding vehicles in rural city types is less, and the average ride and driver fares are high. However, no matter how small the number of people, the average ride and driver fares are quite high, even if the overall earnings are low.

### Table 3. Date and City Types w/NaN
<img width="311" alt="D2_Step3_Output" src="https://user-images.githubusercontent.com/26927158/195757584-4540b90c-62f7-4587-8e96-6682e1bb534f.png">

 
Looking at this pivot table, data for rural, suburban and urban city types are shown as of the beginning of 2019. To create this table, date is set as index, city types are set as columns values, and fare is set for values. However, the special situation that draws attention in the above table is that there are too many lost data, namely NaN values, especially when talking about rural city type. This situation can greatly affect the results of the analysis.

### Table 4. City Types for Dates 
<img width="267" alt="D2_Step7_Output" src="https://user-images.githubusercontent.com/26927158/195757653-9a1fe8cf-fcd6-4e0d-b771-0ba8dd0da32e.png">

To comment on Table 4, all columns have been rearranged on a weekly basis. Based on these data, all weekly data from the 1st week of 2019 until 28 March 2019 are shown in the table. The most important situation in the table is that the urban values are higher than the suburban values and the rural appears as the city type with the lowest total fare values. Across the whole table, the highest value for the rural city was $501.24 per week in the week of 2019-04-07.
$1,412.74 per week has been calculated for Suburban city type on 2019-02-24. For the urban city type, the weekly fare value was calculated to be the highest as $2,470.93 on 2019-03-10.

Graph 1. PyBer Fare Summary
![PyBer_fare_summary](https://user-images.githubusercontent.com/26927158/195757709-21491c61-d9bf-446a-9fd5-f1a16d731f4d.png)

In the chart above, the total fees suitable for city types are expressed in $. 
Yellow color indicates urban, red color indicates suburban, and blue color indicates rural city. 
- First of all, if we write for the rural city type with the lowest value in the table, the most obvious value range seen is between $0-$500. However, it saw the highest value in April.
- Since the red line belongs to the suburban city type, the most obvious interpretation is that total fare values between $500-$1500 were observed.
- When it is necessary to write for the urban city type, the total fares value range is $1500-$2500. It sees the highest value close to March and after March.

# Summary

Some inferences can be made based on the above features. First of all, the urban urban city type has the largest share overall, but the average fare per driver is observed to be quite low. The point to consider here is people's preferences. When the Rural city type is examined, compared to the urban city type, the departure distance may be long and the number of drivers may be less. For someone who earns their economy by driving in urban city types, if the driving distance is short, their earnings may decrease. First of all, these city types can be researched and the distribution of drivers suitable for urban settlement can be made accordingly.

In particular, positive features that will guide the society to use PyBer will be determined and efforts will be made to increase the use even in low-population regions by ensuring customer satisfaction.

However, it should be noted that it may not be right to make any comments based only on the values of 2019. Because, as more years and value are provided, reliability rates can be determined more accurately. The only thing that can be written here is that more accurate analysis can be done with more data.
