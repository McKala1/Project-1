# Project-1

<a href="https://github.com/McKala1/Project-1.git">Our GitHub Repository</a>

<a href="https://docs.google.com/presentation/d/1Kh3zalNeDSe10xlnWiPzQ218AbuSXv8-if7WtuW2eWU/edit?usp=sharing">Our Presentation</a>


## Zestimate Overview
*Antonio
*Using the zillow estimate dataset, I wanted to see what home prices were like in the year 2000 in the city of Ohio. I found that the average home price was estimated at around 89k. This introduced my curiosity of the value of homes in 2023. I wanted to know how much homes have appreciated in the last 23 years.

*The first visualization shows the average home price in 2000, and the second visualization showcases the average home price in 2023. The third visualization shows both the average of homes in 2000, and the average price of homes in 2023 which shows a clear appreciation in value of roughly 100%.

*Next Steps: To get an idea of what homes will be like in 20 years, we’ll use the prophet linear regression model to generate some hypothetical home prices for Ohio.


## Home Forecast Values Overview
*Ishak
* Zillow provides a month-ahead, quarter-ahead, and year-ahead forecast of the Zillow Home Value Index. This data is called Home Value Forecasts. The Zillow Home Value Index is an estimation of the typical value for a given geographic area based on Zillow’s valuation model. It’s calculated based on various data points. These include location, market conditions, and property attributes.

* First I cleaned up the data by dropping any rows that had any null values. There were also irrelevant columns in the dataframe, like Region ID, we did not necessarily need this information. Other columns that we didn’t need either were the Size Rank, Region Type, a separate column telling the name of the state, and the Base Date.

* I first plotted using a line graph, but this didn’t really give us any information, and it was hard to read. So instead I decided to use a bar graph. There were a lot of cities in the dataframe. This made the bar graph hard to read. 

* Instead, I narrowed down the data to only plot the forecast for cities in Ohio. The cities are in order of size rank based on Zillow. From the biggest shown on the left, decreasing as you go to the right. This bar graph shows the forecast of the value of homes for cities in the state of Ohio for the coming month, quarter, and year. As it can be seen, medium-sized cities, toward the center of the graph, have a very large negative Zillow Home Value Index. A negative Zillow Home Value Index typically indicates a decrease in home values within a specific area over a particular period. It suggests that, on average, the houses in that area will depreciate in value.

* I wanted to narrow down the graph further by viewing only the city of Cincinnati to further investigate its home value forecast. As you can see, this bar graph shows the forecast of the value of homes in Cincinnati for the coming month, quarter and year. Initially, there is no change to the home value a month into the future, followed by a considerable decrease in home value a quarter into the future, followed by a slight increase in home value a year into the future. Overall, there will be a decrease in home value in the future.


## New Construction Sales Overview 
* McKala
* For this section, I picked apart the “new construction” sales csv file in pandas. First, I originally wanted to compare the “Metro Sales” and the “New Construction” sales csv with each other so I made a merged dataset. However, when I made my graphs I was only pulling from the “new construction” dataset. So being the efficient human I am, I just went with it and analyzed the new construction sales data. First, I made a bar plot to show the different new construction sales in January, April, August, and November in 2023. It was interesting to see how Columbus, OH had more sales than Cincinnati, OH. Also, I noticed that April is the best time to buy a house because no matter the city the “Spring” purple line in the bar graph surpassed every other season. Then, I looked at the historical data from 2018, all the way to 2023 in the month of January. It was interesting to see how drastic the drop off point was once 2019 hit, most likely due to covid. Then you start to see it pick back up in 2022. For the “Spring” graph you can clearly see the drop off point in 2020 for all the cities. There is a huge spike in 2022 where the new construction housing sales picked back up. The “Summer” sales graph was interesting because there was a spike in 2021, then a slight decline for following years except in 2022 there was another peak for the cities of Cleveland, OH and Akron, OH. The last graph I did was for the historical prices in the month of November. House sales are historically a little lower than usual for this time of year compared to others. In 2021, there was a huge peak in Columbus, OH most likely people cooped up from covid wanted to finally get out and buy a house, or sellers finally feeling comfortable to have people tour their home and put their house on the market. 2022 Fall is when Akron, OH really saw a spike in new construction home sales. Then there is a huge dip in 2023 for Akron, OH I feel like this is because of interest rates being so high. Over all, when looking to buy a new construction house I feel that the graphs I created can help people know what cities are good to look at new homes in. Also, when house shopping if you want to live in a newer development/houses these graphs are great for narrowing in on cities that had new development. Buying a newly built home can be hard to find and that is why I created these graphs so people can have a bit easier time pinpointing locations with homes they want. If you want to buy a new construction house the magical month of April is the ideal time due to motivated sellers from being cooped up all winter, and the great weather. 

## Sales Overview
* Nick
* In my analysis I wanted to explore the correlation (if any) between the Covid Lockdown period and housing sales, which led me to work primarily off of the “metro sales” csv that we had sourced as a group from Zillow. The original scope of the project was supposed to focus on Hamilton County (Ohio) but as the aptly named csv file suggests, my data set only considered the one metropolitan area in Hamilton County, which would be the city of Cincinnati. 

* After cleaning the data, I filtered out the Ohio cities and graphed them to explore any general trends and noticed right away seasonal spikes in home purchases. After isolating the Cincinnati data so that I could use it for a bar graph I considered comparing it to a major metropolitan area to explore not only if the seasonal spike was universal but if it also applied to a much more heavily populated city. In this regard I landed on Los Angeles, which has a population of roughly 13 million people (compared to Cincinnati’s population of a little over 300k). Another factor in the decision was the length of Ohio’s Stay at Home order (lasting only from March 2020 to May 2020) compared to California’s lengthy order (which lasted from March 2019 to January 2021).

* Upon exploring the data I realized that the seasonal spikes were in fact universal, with sharp increases of houses sold around May, a steady peak through the summer months with a small decline into September and a sharp drop in December/January/February. The effect of the covid lockdowns were minimal, even in LA where the lockdown was almost twice as long as in Cincinnati. The biggest difference between the pre-covid data and the post-lockdown data was a stagnation in housing sales in the late spring/ early summer months (April through June) at different times in each city. In Cincinnati you see a stagnation in housing sales in April and May of 2020. Where as in LA, the housing market didn’t start to stagnate until Spring of 2020, almost a year after the city had gone into lockdown. Interestingly, there is a spike in Spring of 2021 sales that surpass pre-covid levels.

* Next steps: If given more time I would have delved deeper into the other factors that affect housing sales in LA like rising interest rates on mortgage loans, lay-offs/unemployment levels (from Covid related lay-offs), increases in house prices, etc. 


## Citations

* Housing Data. Zillow. (2023, April 25). https://www.zillow.com/research/data/ 

